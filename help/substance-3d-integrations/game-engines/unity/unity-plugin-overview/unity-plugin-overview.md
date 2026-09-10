---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unity/unity-plugin-overview.html"
breadcrumb-title: ''
description: 了解 Unity 的 Substance 3D 外掛，包括版本支援、功能及整合能力。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Unity Plugin Overview
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Unity 外掛概述
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '279'
ht-degree: 0%

---


# Unity 外掛概述

## Unity 版本支援

Adobe Substance 3D for Unity 插件版本 3.0.0 目前支援 Unity 2020 LTS 及以上版本。

## 下載物質套件

1. 該外掛可從 Unity 資產商店下載： <https://assetstore.unity.com/packages/tools/utilities/substance-3d-for-unity-beta-213208>

## 物質進口

1. 在專案視窗中右鍵點擊，選擇匯入資產，或將你想匯入的物質材料拖曳到專案檢視面板。
1. 瀏覽你想匯入的物質資料。 Substance Materials 的副檔名是「.sbsar」。
1. Substance 材質會匯入你的 Unity 專案。

   1. sbsar 資產會建立一個主匯入檔和一個資料夾，裡面有輸出材質和產生的 Unity 材質。
1. 接著你可以在場景檢視中拖放材質到網格上，再在檢查器中編輯參數。

   ![](../../../assets/window-overview.png){width="1000px"}

>[!NOTE]
>
> **法線貼圖轉換**
> 
> Unity 中的 Substance 插件會自動將 DirectX 轉換成 OpenGL。 使用Substance Source[&#128279;](https://source.substance3d.com/)的材質時，不需要將法線方向改成OGL。如果你在 Substance Designer 裡自己製作材質，務必使用預設的 DirectX 著色器，因為外掛會自動處理正常的轉換。 欲了解更多資訊，請參閱「在 Unity 中處理法線」相關資訊。

## 參數變更

參數與解析度可在檢查器視窗中設定。 請參閱 [「參數變更](../../../game-engines/unity/changing-parameters/changing-parameters.md)」。

[團結_tweaking\_parameters.mp4](https://helpx.adobe.com/content/dam/help/en/substance-3d/documentation/download/attachments/186056716/unity-tweaking-parameters.mp4)

## Unity 渲染管線支援

Substance 3D 外掛支援 HDRP 和 URP。 更多資訊將很快公布。

## 教學教學方法
