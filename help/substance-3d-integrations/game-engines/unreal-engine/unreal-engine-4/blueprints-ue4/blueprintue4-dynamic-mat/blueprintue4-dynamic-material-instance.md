---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-4/blueprints-ue4/blueprintue4-dynamic-material-instance.html"
breadcrumb-title: ''
description: 在 Unreal Engine 4 中，使用藍圖在執行時從 Substance 材質建立動態材質實例。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 4 > Blueprints - UE4 > Blueprint(UE4) Dynamic Material Instance
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Blueprint（UE4） 動態材質實例
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '458'
ht-degree: 0%

---


# Blueprint（UE4）：動態材質實例

你可以建立一個 Substance Graph 實例，在執行時建立動態圖實例。

1. 建立一個 Substance Instance Factory 型別的變數，並將預設值設為 Imported Substance Factory。
1. 新增一個 Create Graph Instance 節點，並將 Substance Instance Factory 接入 Factory 輸入。 設定一個實例名稱。
1. 建立另一個 Substance Instance Factory 型別的變數。 這將包含對動態物質的參考。
1. 將動態物質的變數設定為 Create Graph Instance 節點的回傳值。
1. 建立一個 Material 類型的變數。 這就是素材範本。 在內容瀏覽器中，複製由 Substance 產生的 UE4 素材。 將這份重複的材料設為材料範本變數的輸入。
1. 新增一個建立動態材質實例，並將材質範本變數設為父變數。

   ![](../../../../../assets/rt-01.png){width="800px"}
1. 建立一個 Material 類型的變數。 這就是材質實例動態（MID）。 將動態材質實例的回傳值設為變數。

   ![](../../../../../assets/rt-02.png){width="800px"}
1. 新增一個 Set Material 節點，並將 MID 變數的值設為 Material 輸入。 目標設定為你想要套用材質的物件。
1. 建立一個 Name 型別的變數。 這個變數會保留素材中所設定的通道名稱。 初始化為「NONE」
1. 新增一個 Get Substance Textures 節點，並將圖實例設定為動態圖實例變數。
1. 新增一個 For 迴圈節點。 在這裡你會循環使用物質材質。 以取得物質材質的結果作為輸入陣列。

   ![](../../../../../assets/rt-03.png){width="800px"}
1. 新增一個 Substance Get Channel 節點，輸入是 for 迴圈中的陣列元素。
1. 新增一個序列節點。 這裡我們先執行 Get Channel 節點的結果。
1. 在 ESubChannelType 的序列後面加一個開關，然後以 Get Channel 回傳值作為選擇 0。 這裡我們檢查頻道名稱。
1. 將 MID 名稱變數設為第 5 步複製的 Substance Material 頻道名稱。 *請參考實體圖片。*
1. 在 Sequence Then 1 節點中，你會設定將通道名稱指派給動態素材的流程。
1. 取得 MID 名稱變數，並加入一個等值為「NONE」的字串節點，這個值會初始化變數。
1. 從相等節點加入一個帶有條件的分支節點。
1. 新增一個 Substance Set 的材質參數值。 目標是 MID 變數，參數名稱是 MID 名稱變數。 該值是 ForEachLoop 節點的陣列元素。

![](../../../../../assets/material-1.png){width="800px"}
