---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-5/blueprints-ue5/blueprintue5-node-reference.html"
breadcrumb-title: ''
description: Unreal Engine 5 中所有可用於材質操作的 Substance Blueprint 節點參考指南。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 5 > Blueprints - UE5 > Blueprint(UE5) Node Reference
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Blueprint（UE5） 節點參考
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '947'
ht-degree: 0%

---


# Blueprint（UE5）：節點參考

## 一般物質節點：

| 名稱 | 輸入 | 說明 |
| --- | --- | --- |
| **GetSubstances** | 輸入： **材料** | 回傳一個由材質使用的實體圖實例陣列。 如果你建立一個材質，使用兩個不同圖實例的紋理輸出，這個函式會回傳這兩個圖實例。 |
| **GetSubstanceTextures** | 輸入： **SubstanceGraphInstance** | 回傳來自 Substance Graph Instance 輸入參數的所有啟用及目前已計算的紋理陣列。 |
| **GetGraphName** | 輸入： **SubstanceGraphInstance** | 回傳 Designer 中設定的圖形名稱。 |
| **GetFactoryName** | 輸入： **SubstanceGraphInstance** | 回傳用於建立 **SubstanceGraphInstance 的 GraphInstance** 名稱&#x200B;**，該 SubstanceGraphInstance** 傳遞到該節點。 |
| **取得內容載入進度** | 沒有 | 回傳浮點數介於0到1之間，顯示已滿載物質數量的百分比。 |
| **CreateGraphInstance** | 輸入： **SubstanceInstanceFactory** - 你想建立圖形實例的工廠。輸入： **GraphIndex** （int） - 你想建立的圖形的索引。 輸入： **InstanceName** （FString） - 你希望新實例擁有的名稱。 | 會回傳一個新的獨立圖形實例，該實例會持續存在直到你的應用程式關閉。 |
| **複製圖形實例** | **SubstanceGraphInstance** - 你想要建立副本的圖實例。 | 會回傳一個新的獨立圖形實例，該實例會持續存在直到你的應用程式關閉。 |
| **EnableInstanceOutputs** | Input： **SubstanceGraphInstance** - 包含啟用輸出的圖實例 Input： **OutputInindexes** （int32 陣列）- 你想啟用的輸出指標。 | 若先前停用，則在 SubstanceGraphInstance **中建立 的**&#x200B;紋理輸出。此功能與啟用 SubstanceGraphInstance **編輯器的輸出**&#x200B;相同。*注意：這不會更新你的材質，並加入新建立的材質。 這需要在執行時用新輸出設定取樣器參數來處理。* |
| **DisableInstanceOutputs** | Input： **SubstanceGraphInstance** - 包含用來停用輸出的圖形實例 Input： **OutputIndices** （int32 陣列） - 你想停用輸出的索引 | 如果啟用，會停用並刪除傳入圖物件的貼圖輸出 |
| **複製輸入參數** | 輸入： **SubstanceGraphInstance** - 你想套用值的圖實例 Input： **SubstanceGraphInstance** - 你想從中取得值的圖實例 | 還原 Substance Graph 實例輸入參數中所有變更過的輸入值。 |
| **重置輸入參數** | 輸入：SubstanceGraphInstance | 將 Substance Graph 實例的輸入值重置為預設值 |
| **SetGraphInstanceOutputSize** | 輸入： **SubstanceGraph 實例**&#x200B;輸入：寬度 - X 座標的紋理解析度 輸入：高度 - Y 座標的紋理解析度 | 設定從此圖實例產生的所有輸出的紋理解析度，並從參數中傳入的大小。 註 - CPU 引擎上的 Max 2048 註解 - GPU 引擎上的 Max 4096 |
| **非同步渲染** | **SubstanceGraphInstance** | 重新計算 Substance Graph 實例輸入的輸出紋理。 （非阻塞） |
| **同步渲染** | **SubstanceGraphInstance** | 重新計算 Substance Graph 實例輸入的輸出紋理。 （阻擋聲） |

## 圖實例專屬功能：

只能從圖實例呼叫

| 名稱 | 輸入 | 說明 |
| --- | --- | --- |
| GetDynamicMaterialInstance | 輸入：名稱（字串） | 回傳執行時動態物質實例，或在不存在物質時創建實體。 動態材質實例對於大多數執行時值的變動都被要求，來自實體值輸出。 |
| **取得輸入名稱** | 沒有 | 回傳包含所有輸入參數名稱的字串陣列。 |
| **GetInputType** | 沒有 | 回傳與此輸入相關的資料型別。 |
| **SetInputInt** | 輸入： **識別碼** （字串）輸入： **輸入值** （整數陣列） | 改變由識別碼找到的輸入值。 在遊戲中，必須使用 **AyncRender** 或 **SyncRender** 來渲染內容，才能套用變更。 |
| **SetInputFloat** | 輸入： **識別碼** （字串）輸入： **輸入值** （浮點數陣列） | 改變由識別碼找到的輸入值。 在遊戲中，必須使用 **AyncRender** 或 **SyncRender** 來渲染內容，才能套用變更。 |
| **GetInputInt** | 輸入： **識別碼** （字串） | 回傳一個包含輸入參數當前值的整數陣列。 |
| **GetInputFloat** | 識別碼（字串） | 回傳一個包含輸入參數當前值的浮點數陣列。 |
| **SetInputBool** | 輸入： **布爾** （布林）輸入： **識別碼** （字串） | 會接收一個布林值來指派可切換的輸入值類型。 過去，這只能透過將 int 值設為 1 或 0，並投擲成 bool 來達成。 |
| **GetInputBool** | 輸入： **識別碼** （字串） | 回傳輸入的當前布林值。 |
| **設定色彩** | 輸入： **顏色** （線性色彩）輸入： **識別碼** （FString） | 會接收 FLinearColor 值來指派顏色輸入值類型。 過去，這只能透過設定浮點數值並傳遞一組浮點數來達成。 |
| **GetInputColor** | 輸入：識別碼（FString） | 回傳 UE4 格式的當前色彩值。 |
| **CreateAggregateSubstanceFactory** | 輸入： **輸出工廠** （SubstanceInstanceFactory）*產生輸出的工廠，這些輸出將作為輸入到該工廠。*&#x200B;輸入： **輸出工廠圖索引** （整數）*你想在物質中用來合併的哪個圖形。* 輸入： **輸入工廠** （SubstanceInputFactory）*工廠使用輸出作為輸出工廠的輸入影像。*輸入：**連接**（SubstanceConnections 陣列）*此可透過藍圖節點 Make Array 建立。 物質連結是指你如何讓聚合節點連結哪些輸入連接到哪些輸出。* **&#x200B; Return（SubstanceInstanceFactory）*** 可用來建立新合併實例的圖實例。* | 新的聚合實體節點允許你在執行時取得兩個實體實例工廠，並建立一個新的實例工廠，進而用來建立新的圖實例。 這點特別之處在於你可以將其中一個合併圖實例的輸出紋理連接到另一個合併圖實例的輸入影像。 要從這個新工廠建立 substance graph 實例，請參閱我們關於執行時圖實例的文件。 |
| **SubstanceConnectionStruct** | 輸入： **輸出識別碼** （FString）*將紋理輸出串接成輸入的識別碼。* 輸入： **輸入識別碼** （FString） | Create Aggregate Substance Factory 用來指定如何將每個輸出紋理串接到新的輸入紋理。 |
