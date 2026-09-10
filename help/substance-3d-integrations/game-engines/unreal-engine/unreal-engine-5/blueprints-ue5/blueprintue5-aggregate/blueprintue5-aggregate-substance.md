---
helpx_url: "https://helpx.adobe.com/tw/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-5/blueprints-ue5/blueprintue5-aggregate-substance.html"
breadcrumb-title: ''
description: 在 Unreal Engine 5 中，使用藍圖聚合節點在執行時合併多個 Substance 材質，以實現進階工作流程。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 5 > Blueprints - UE5 > Blueprint(UE5) Aggregate Substance
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Blueprint（UE5） 聚合實質
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '258'
ht-degree: 0%

---


# Blueprint（UE5）：Aggregate Substance

1. 使用「建立聚合物質工廠」節點，設定輸出與投入工廠。 輸出工廠應該有一個貼圖，作為輸入工廠參數中的輸入影像使用。
1. 為每個作為輸入的輸出紋理建立 SubstanceConnection 物件，並包含對應值的名稱（輸出圖的輸出名稱與輸入圖的輸入參數名稱）
1. 新增一個 Create Graph Instance 節點，並將「Create Aggregate Substance Factory」節點的結果插入 Factory 輸入，並附上一個母材質作為範本（這可以是插件預設_substance材質之一）。
1. 建立一個 Substance Graph 實例變數，並儲存前一個節點的結果。
1. 可選：設定任意物質參數（此範例為設定圖形輸出的新解析度）。
1. 建立一個非同步或同步渲染節點，並將要渲染的實例連接到 Substance Graph 實例變數。
1. 使用圖形實例中的「取得動態材質實例」功能來建立或取得一個現有的實例。 將名稱和「在母素材中」留空，將使用步驟 3 中產生實例時使用的參數。
1. 新增一個 Set Material 節點，並將 MID 變數的值設為 Material 輸入。 目標設定為你想要套用材質的物件。
