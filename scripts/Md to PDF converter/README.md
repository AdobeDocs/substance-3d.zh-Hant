---
source-git-commit: a517442244806bc6aef0f5bfb165c5d4f67341be
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 0%

---
# 降價轉 PDF 轉換器

此資料夾包含一個預處理與轉換腳本，用於從此儲存庫產生文件頁面的 PDF 版本。

## 為什麼會這樣

文件原始檔案使用 Adobe 平台專屬的標記降語法（手風琴區塊、警示呼叫及影像屬性擴充），標準標記工具無法理解。 此腳本會將語法正規化，並使用 [md-to-pdf](https://github.com/simonhaenisch/md-to-pdf) 將檔案轉換為 PDF，同時壓縮影像以保持輸出檔案大小可控。

## 先決條件

- [Node.js](https://nodejs.org/) （v18 或更新版本）
- 相依關係已經安裝在 `node_modules/`. 如果需要重新安裝，請從這個資料夾執行 `npm ci` 。

## 使用情況

從倉庫根&#x200B;**執行腳本**，並將路徑傳遞到你想轉換的標記檔案：

```
node "scripts/Md to PDF converter/preprocess-for-pdf.js" <path/to/file.md>
```

**範例：**

```
node "scripts/Md to PDF converter/preprocess-for-pdf.js" help/substance-3d-general/openpbr/openpbr-overview.md
```

PDF 會寫入 **與原始檔案**&#x200B;相同的目錄。 在轉換過程中建立的暫存檔案（`*.pdf-ready.md` 和 `_pdf-images/`）會在成功時自動刪除。 若轉換失敗，則保留位置以協助除錯。

## 劇本的作用

| 原始碼語法 | PDF 輸出 |
|---|---|
| `+++Title` / `+++` 手風琴方塊 | `#####` 標題內容始終可見 |
| `>[!NOTE]` 警報呼叫 | 標準加粗 **引用註：** 前綴 |
| `![](path){width="N"}` 影像屬性 | `<img>` 保持指定寬度的標籤 |
| Markdown 影像連結到 `.pdf` 檔案 | 已移除（僅限網頁自下載參考） |
| `hold:` 前備標鍵 | 已移除（僅限平台的元資料） |
| 所有圖片 | 重新調整為最大 1200 像素寬度，重新編碼為 JPEG，品質為 80% |
| 所有表格 | 透過注入的 CSS 移除邊界與背景 |
