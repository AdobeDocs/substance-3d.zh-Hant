---
helpx_url: "https://helpx.adobe.com/tw/substance-3d-integrations/game-engines/unity/rendering-color-space.html"
breadcrumb-title: ''
description: 請設定 Unity 的色彩空間設定，以確保 Substance 材質能以實體為基礎的著色器正確呈現。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Rendering Color Space
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 渲染色彩空間
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '102'
ht-degree: 0%

---


# 渲染色彩空間

Substance 貼圖是設計來搭配物理基礎著色器使用。 為了獲得最佳效果，你應該在 Unity Player 設定中將色彩空間設為線性。

1. 前往編輯>專案設定>球員
1. 在渲染區塊，將色彩空間改為線性。 （Unity 預設是伽瑪空間，這不正確，會導致材質顏色看起來不對）。

   >[!NOTE]
   >
   > **資訊**
   > 
   > 如果 Unity 的色彩空間設定設為 Gamma 時，sRGB 材質選項將被停用

   ![](../../../assets/rendering-4.png){width="600px"}
