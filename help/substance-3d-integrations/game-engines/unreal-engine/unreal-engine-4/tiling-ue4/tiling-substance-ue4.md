---
helpx_url: "https://helpx.adobe.com/tw/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-4/tiling-substance-ue4.html"
breadcrumb-title: ''
description: 在 Unreal Engine 4 中透過為材質加入貼圖座標節點和標量參數來製作 Tile Substance 材質。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 4 > Tiling Substance - UE4
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 平鋪物質 - UE4
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '77'
ht-degree: 0%

---


# 平鋪物質 - UE4

要平貼一個物質貼圖，你需要新增一個貼圖座標節點，並將它乘以純量參數。

<https://docs.unrealengine.com/latest/INT/Engine/Rendering/Materials/ExpressionReference/Coordinates/#texturecoordinate>

要同時為 u 和 V 圖塊建立參數，可以使用 Append Vector，並將此與 TexCoord 相乘。 這讓你可以獨立設定 U 和 V 的方塊數量。

![](../../../../assets/tiling-3.png){width="800px"}
