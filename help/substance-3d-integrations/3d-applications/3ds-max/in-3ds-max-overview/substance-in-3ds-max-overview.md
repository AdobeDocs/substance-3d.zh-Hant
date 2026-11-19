---
helpx_url: "https://helpx.adobe.com/tw/substance-3d-integrations/3d-applications/3ds-max/substance-in-3ds-max-overview.html"
breadcrumb-title: ""
description: 了解 3ds Max 的 Substance 外掛，以及如何匯入和使用 Substance 材質在您的專案中。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > 3ds Max > Substance in 3ds Max Overview
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 3ds Max 中的 Substance 概覽
user-guide-description: ""
user-guide-title: ""
source-git-commit: a167bcd2c2f0af70b3a4dc37eafc85145c79c590
workflow-type: tm+mt
source-wordcount: '332'
ht-degree: 0%
---

# 3ds Max 中的 Substance 概覽

## 外掛程式概覽

## 開啟物質

1. 開啟 Slate 編輯器，搜尋 Substance，並將 Substance2 節點拖曳到檢視中。
1. 雙擊 Substance 節點以啟用屬性，並在 Substance 套件瀏覽器下載入 Substance。

   >[!NOTE]
   >
   > 您也可以將 .sbsar 檔案拖放到 Slate 編輯器中，自動建立節點並匯入 sbar。

1. 如果一個實體包含多個圖表，您可以在「已選圖表」下拉選單中選擇想要輸出為材質的圖表。

   ![](../../../assets/max1.png)

1. 選取 Substance 節點後，前往 Substance 選單並選擇支援的渲染器。 材料會被製作完成，並準備好應用於物件上。 Substance 貼圖會直接連接到渲染材質中。

>[!NOTE]
>
> 選取「Substance2」節點後&#x200B;**，您需要先**&#x200B;點擊「載入物質...**」以選擇 sbsar 檔案，然後從頂方選單選擇支援的渲染器（例如「Substance to Arnold**」）。
>
>支援的渲染器包括 Arnold、V-Ray、Corona 和 Octane。 [了解 3DS Max 中的工作流程，了解如何使用 OpenPBR 材質。](../using-workflows-3ds-max/using-workflows-in-3ds-max.md)

![](../../../assets/max3.png)

## 變更解析度

1. 在「物質輸出設定」中設定計算出的 Substance 貼圖所需的解析度。
1. 若要支援最高 8K 解析度，請確認你使用的是 GPU 引擎，這在 Substance 設定[&#128279;](../../../3d-applications/3ds-max/settings-1/substance-settings.md)中設定。

   ![](../../../assets/max6.png)

## 變更參數

1. 雙擊 Substance 節點，以在參數視窗中載入 Substance 參數。
1. 更改參數以自動更新 Substance 貼圖。

   ![](https://helpx-prod.scene7.com/is/image/HelpxProd/max4?$png$&jpegSize=200&wid=1276){width="500px"}

## 設定輸出預覽

你可以為 Substance 節點的縮圖設定特定通道。

1. 在「輸出預覽」下拉選單中，選擇您想用作節點縮圖的通道。

   ![](../../../assets/max7.png)

## 瓷磚材料

你可以使用 Coordinates 屬性來平鋪 Substance 貼圖並設定 Map Channels。

![](../../../assets/max10.png)
