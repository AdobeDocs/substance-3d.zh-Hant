---
helpx_url: "https://helpx.adobe.com/tw/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-5/physical-size-ue5.html"
breadcrumb-title: ''
description: 在 Unreal Engine 5 中，使用實體尺寸設定根據真實世界的尺寸來縮放物質材質。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 5 > Physical Size - UE5
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 實體尺寸 - UE5
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '163'
ht-degree: 0%

---


# 實體尺寸 - UE5

物質材料的物理尺寸允許根據材料在世界中的大小進行縮放。 這個數值會在 Substance Designer 設定，然後透過材質模板系統讀取到 Unreal。\
[母體中的 Substance\_Triplanar\_Template](../../../../game-engines/unreal-engine/unreal-engine-5/material-template-usage/out-the-box-material-tem/out-of-the-box-material-templates.md) 材質包含了一個範例，說明如何利用物理尺寸來縮放 Unreal 材質。



不管網格上的放大值如何，材質都會根據它們在世界中佔據的公分大小來鋪磚。 以岩石材料為例（圖片1），每次測量的厚度約為1.8公尺（180公分）。

![](../../../../assets/rock-material-parameters.png)

包含物理尺寸資料的物質材料，其數值會被複製到任何現有的材料向量參數節點，該節點名為 physicalsize。



由於 UE5 中材料沒有位移值，實體尺寸模板會將三平面地圖的值複製為 X、Y、X。
