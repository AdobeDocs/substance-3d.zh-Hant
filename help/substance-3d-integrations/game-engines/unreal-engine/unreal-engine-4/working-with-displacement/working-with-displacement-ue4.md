---
helpx_url: "https://helpx.adobe.com/tw/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-4/working-with-displacement-ue4.html"
breadcrumb-title: ''
description: 啟用 tessellation，並在 Unreal Engine 4 中使用 Substance 材質的位移貼圖來製作表面細節。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 4 > Working with Displacement - UE4
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 與位移合作 - UE4
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '196'
ht-degree: 0%

---


# 與位移合作 - UE4

要處理位移，你需要在材質上啟用鑲嵌。

![](../../../../assets/tess.png){width="600px"}

要使用高度輸出，你需要在物質工廠實例中雙擊輸出來建立高度。 高度預設是沒有啟用的。 接著你可以把這個高度輸出拖到你的材質裡。

![](../../../../assets/height-1.png){width="800px"}

當你把高度輸出加到材質上後，你需要建立幾個節點來驅動世界位移和細分修改器。

1. 建立兩個標量參數。 一個是距離，另一個是細分的倍數。
1. 將紅色通道從高度乘以距離參數
1. 新增一個 VertexNormalWS 節點，並在步驟 2 中將它與乘法的輸出相乘。
1. 輸入 VertexNormal 與材質世界位移的乘法。
1. 取鑲嵌乘數參數，輸入材料上的鑲嵌乘數。

![](../../../../assets/setup-3.png){width="800px"}

>[!NOTE]
>
> 為了簡化圖表，其他紋理輸出在此圖中省略。 這裡只顯示位移和乘法節點以求清晰。
