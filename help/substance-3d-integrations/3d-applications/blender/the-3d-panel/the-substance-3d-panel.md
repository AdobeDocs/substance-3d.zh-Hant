---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/blender/the-substance-3d-panel.html"
breadcrumb-title: ''
description: 學習如何在 Blender 中使用 Substance 3D 面板來管理材質、參數和輸出。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > Blender > The Substance 3D Panel
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 物質3D面板
user-guide-description: ''
user-guide-title: ''
source-git-commit: 4a060ee1aaa1731c04e70d5512e3271cd63d0381
workflow-type: tm+mt
source-wordcount: '465'
ht-degree: 0%

---


# 物質3D面板

![](../../../assets/blender-substance3dpanel.png)

## 面板控制

**Create** - 打開檔案瀏覽器以選擇 Substance 3D 材質。 預設情況下，這會用 .sbsar 檔案產生的材質來建立 blender 材質。

**套用** - 將選中的 Substance 3D 材質附加到選取的物件上，並置於新的材質槽中。 這不會覆蓋物件上先前的材料分配。

**Substance 3D 社群資產** - 在網頁瀏覽器中開啟 Substance 3D 社群資產頁面。

**Substance 3D 資產** - 在網頁瀏覽器中開啟 Substance 3D 資產原始碼頁面。

**複製選取的物質3D材質** ——載入所選物質3D材質的新實例。 同一物質材料的不同實例的參數可以獨立調整。

**刷新** - 重新載入 Substance 3D 材質

>[!WARNING]
>
> **警告：**
> 
> 使用重新整理按鈕會撤銷使用者對著色器圖的任何更改。 在刷新前複製任何使用者新增的節點，然後在刷新後將它們貼上到圖表中。

**移除** - 從面板中移除選取的物質 3D 材料。

>[!NOTE]
>
> Blender 用 Substance 材料製成的材料會保留在專案中。 它可以手動刪除或移除物件。

**載入的 3D 物質材質** - 顯示已載入 .blend 檔案的物質材質清單。

## 圖參數

**輸出解析度** - 有 with 和高度解析度的下拉選單。 這些參數可以拆開連結，分別調整數值。

**隨機化與隨機種子** ——隨機化按鈕會產生新的隨機種子值，以改變可用隨機值的參數。 隨機種子也可以手動設定。

## 使用預設

SBSAR 檔案可以與預設一起發佈，預設可在預設下拉選單中找到。 要自己做預設，請依需求調整參數並使用 **儲存** 按鈕。 還有額外選項可以將所選預設匯出成 .sbsprs 檔案，或是從下拉選單中刪除所選預設。 **載入**&#x200B;按鈕可以用來從 .sbsprs 檔案匯入預設。

## 物質參數

在 Substance Designer 中暴露的參數可以透過 Substance 參數控制項進行調整。 這些參數由物質材料的創造者設定，且會因材料而異。 調整這些參數會更新產生的貼圖，根據「載入 3D 物質材質」區塊中材質名稱旁的處理圖示所示。

輸出材質的檔案格式可以透過下拉選單切換和更改。

欲了解更多資訊，請參閱 [Designer 文件頁面的「暴露參數](https://experienceleague.adobe.com/en/docs/substance-3d-designer/using/substance-graphs/manage-parameters/exposing-a-parameter) 」。

## 技術參數

物質材料可能有一套技術參數。 這些是用於色彩校正及其他材質調整的額外控制。
