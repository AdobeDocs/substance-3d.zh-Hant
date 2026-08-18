---
helpx_url: "https://helpx.adobe.com/tw/substance-3d-integrations/3d-applications/blender/release-notes/add-on-0-9-1.html"
breadcrumb-title: ''
description: 請參閱 Blender 附加元件 0.9.1 版本的發布說明，了解新功能、改進與錯誤修正。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > Blender > Release Notes > Add-on 0.9.1
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 附加元件 0.9.1
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '463'
ht-degree: 0%

---


# 附加元件 0.9.1

**附加元件版本 0.91+ 的發行說明**

* 注意： *插件版本 0.91+ 與先前版本不相容！*
* 內部程式碼基礎重新架構以提升外掛的效能與穩定性
* 重新設計的使用者介面以提升整體使用者體驗
* 新增 UI 以提供修改預設平鋪的功能
* 新增支援在循環渲染檢視中更新貼圖
* 在控制台新增錯誤處理功能，以通知物質載入失敗
* 更新了浮動選單，加入了快速動作

**偏好設定區：新增/更新：**

* 匯出影像格式參數;當 Blender 產生的影像作為 Substance 材質的影像輸入時，此格式會用來將該影像儲存到 Temporal 資料夾。
* Sbsar 函式庫路徑;指定使用載入按鈕搜尋物質檔案時預設開啟的資料夾。
* 預設的材質匯出路徑（Temporal 資料夾），模擬 Substance 3D Painter 用來處理未儲存檔案匯出的路徑
* 貼圖相對路徑與上述相同，並可選擇使用像 $matName 這類鍵來建立子資料夾
* sbsar 檔案相對於建立一個子資料夾的路徑，該子資料夾會打包你在儲存專案時使用的 sbsar 檔案
* 能在偏好設定中動態設定不同的著色器網路——在著色器網路中，能根據著色器需求設定不同變數
* 在著色器網路的輸出區，你可以設定輸出是否預設啟用
* 能夠設定色彩空間（這將支援 ACES、線性 EXR 和 Blender 的電影工作流程，而不僅限於 srgb）
* 預設的影像格式與位元深度選擇
* 一個通用輸出，用來設定 shader 未定義的輸出使用值，例如你有另一個 Shader 預設不使用的輸出，例如遮罩。
* 一個用來改變輸出類型的過濾器（1 僅啟用輸出，2 所有在著色器和 Substance 中都能有的輸出，3 Substance 中所有可用的輸出）
* 支援自訂捷徑（已編輯）

**Substance 3D 面板區塊：新增/更新：**

* 調整並鎖定平鋪與解析參數值的能力
* 更新的預設介面 - 著色器類型下拉選單，用來更改使用者想要的圖形類型
* 將影像輸入參數改為 Blender 使用的標準影像輸入。 你現在可以使用 Blender 的圖片，而不只是檔案
* 能夠隨時在多個 Blender 實例中運作
* 當 Substance 3D 面板中選取材質時，支援自動高亮材質
