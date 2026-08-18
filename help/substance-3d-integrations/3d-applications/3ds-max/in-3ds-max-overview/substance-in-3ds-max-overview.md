---
helpx_url: "https://helpx.adobe.com/tw/substance-3d-integrations/3d-applications/3ds-max/substance-in-3ds-max-overview.html"
breadcrumb-title: ''
description: 了解 3ds Max 的 Substance 插件，以及如何匯入和使用 Substance 材質在你的專案中。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > 3ds Max > Substance in 3ds Max Overview
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 3ds Max 中的物質概述
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '296'
ht-degree: 0%

---


# 3ds Max 中的物質概述

## 插件概述：

## 打開物質

1. 打開 Slate 編輯器，搜尋 Substance，然後把 Substance2 節點拖到檢視圖。
1. 雙擊 Substance 節點以啟用屬性，然後在 Substance Package Browser 裡載入 Substance。

   >[!NOTE]
   >
   > 你也可以把 .sbsar 檔案拖放到 Slate 編輯器裡，自動建立節點並匯入 sbar。
1. 如果一個物質包含多個圖表，你可以在「選取圖」下拉選單中選擇想要輸出的圖作為材料。

   ![](https://helpx-prod.scene7.com/is/image/HelpxProd/max8?$png$&jpegSize=100&wid=341)

   ![](../../../assets/max1.png)
1. 選擇 Substance 節點後，前往 Substance 選單，選擇支援的渲染器。 材料會被創造出來，並準備好應用於物件上。 材質貼圖會連接到渲染材質中。

   | 支援的渲染器 |
   | --- |
   | 阿諾德 |
   | 弗雷 |
   | 新冠 |
   | 辛烷值 |

   ![](../../../assets/max3.png)

## 解析度變更：

1. 在 Substance 輸出設定中設定計算出的 Substance 材質所需的解析度。
1. 解析度最高可達 8K，請確保你使用的是 Substance 設定[&#128279;](../../../3d-applications/3ds-max/settings-1/substance-settings.md)中的 GPU 引擎。

   ![](../../../assets/max6.png)

## 參數變更：

1. 雙擊 Substance 節點，在參數視窗中載入 Substance 參數。
1. 更改參數以自動更新 Substance 貼圖。

   ![](https://helpx-prod.scene7.com/is/image/HelpxProd/max4?$png$&jpegSize=200&wid=1276){width="500px"}

## 設定輸出預覽：

你可以為Substance節點的縮圖設定特定通道。

1. 在輸出預覽下拉選單中，選擇你想用作節點縮圖的通道。

   ![](../../../assets/max7.png)

## 瓷磚材料：

你可以用座標屬性來平貼 Substance 貼圖並設定 Map Channels。

![](../../../assets/max10.png)
