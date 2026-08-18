---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-4/blueprints-ue4/blueprintue4-aggregate-substance.html"
breadcrumb-title: ''
description: 在 Unreal Engine 4 中，使用藍圖聚合節點在執行時合併多個 Substance 材質，以實現進階工作流程。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 4 > Blueprints - UE4 > Blueprint(UE4) Aggregate Substance
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Blueprint（UE4） 聚合實質
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 0%

---


# Blueprint（UE4）：Aggregate Substance

新的聚合實體節點允許你在執行時建立兩個實體實例工廠，並建立一個新的實例工廠，用來建立新的圖實例。 這點特別之處在於你可以將其中一個合併圖實例的輸出紋理連接到另一個合併圖實例的輸入影像。 要從這個新工廠建立 substance graph 實例，請參閱我們關於執行時圖實例的文件。 [材質實例定義 - UE4](https://helpx.adobe.com/substance-3d/unlisted/documentation/integrations/material-instance-definition-157352129.html)

1. 進口你想使用的物質。
1. 建立一個變數「AggregateGraphInstance」，型別 **為 Substance Graph Instance**。
1. 建立一個 Material **和** Material Instance Dynamic 型態&#x200B;**的變數**
1. 建立 **一個建立物質連結（Make Substance Connection** ）並設定輸出與輸入識別碼。
1. 建立 **Aggregate Substance 實例工廠** ，並設定輸出與輸入工廠。
1. 建立一個 **圖實例** 並設定實例名稱。
1. 設定 **聚合圖實例** 變數。
1. 在第 7 **步使用 Get Substance Textures** 從 Aggregate Graph 實例取得 Substance Textures。
1. 用步驟 3 的 material 變數作為父變數，建立一個 **動態材質實例** 。
1. 從步驟3開始設定MID變數。
1. 用 **Set Material** 搭配 MID 變數設定網格材質。

   ![](../../../../../assets/a2-3.png){width="800px"}
1. 依照動態材質實例文件中所示（步驟 11-19）設定素材通道\
   [Blueprint（UE4）：動態材質實例](https://helpx.adobe.com/substance-3d/unlisted/documentation/integrations/blueprint-dynamic-material-instance-152535142.html)

   ![](../../../../../assets/a4-3.png){width="800px"}
