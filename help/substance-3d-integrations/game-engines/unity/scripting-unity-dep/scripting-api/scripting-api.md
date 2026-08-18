---
helpx_url: "https://helpx.adobe.com/tw/substance-3d-integrations/game-engines/unity/scripting-in-unity-deprecated/scripting-api.html"
breadcrumb-title: ''
description: 關於已棄用的 Substance Unity 腳本 API 的參考文件，用於舊有專案支援。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Scripting in Unity (Deprecated) > Scripting API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 腳本 API
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '1074'
ht-degree: 1%

---


# 腳本 API

## Substance in Unity API - 2.2.0

## 物質材料參數

| 公共方法 | 說明 | 參數 |
| --- | --- | --- |
| public **float &#x200B;***GetInputFloat*（**字串** inputName） | 取得 Substance **Float** 輸入 | **SBSAR 中輸入的字串***輸入名稱* |
| public **int** *SetInputFloat*（**字串** inputName， **float** value） | 更新物質 **浮子** 輸入 | **字串** i nputName *SBSAR **中輸入的名稱 浮點數**&#x200B;**值 用於更新參數的值* |
| public **void** *SetInputVector2*（**字串** inputName， **Vector2** 值） | 更新物質 **向量2** 輸入 | **字串** *輸入名稱* SBSAR **中輸入名稱 向量2** *輸入* 更新參數所使用的值 |
| public **vector2** *GetInputVector2*（**字串** inputName） | 取得Substance **Vector2** 輸入 | **字串** 「inputName」SBSAR 中輸入的名稱 |
| public **void** *SetInputVector3*（**字串** inputName， **Vector3** 值） | 更新物質 **向量3** 輸入 | **字串***輸入名稱* SBSAR **中&#x200B;*輸入的名稱 向量3***&#x200B;用於更新參數的值 |
| public **vector3** *GetInputVector3*（**字串** inputName） | 取得Substance **Vector3** 輸入 | **SBSAR 中輸入的字串***輸入名稱* |
| public **void** *SetInputVector4*（**字串** inputName， **Vector4** 值） | 更新物質 **向量4** 輸入 | **SBSAR**&#x200B;輸入 Vector4 ***值*中輸入的字串** *輸入名稱* 更新參數所使用的值 |
| public **vector4** *GetInputVector4*（**字串** inputName） | 取得Substance **Vector4** 輸入 | **SBSAR 中輸入的字串** 輸入名稱 |
| public **void** *SetInputColor*（**字串** inputName， **Color** value） | 更新物質 **顏色** 輸入 | **SBSAR**&#x200B;顏色&#x200B;**值中輸入的字串**&#x200B;輸入名稱 用於更新參數 |
| public **color** *GetInputColor*（**字串** inputName， **int** dataType） | 取得 Substance **Color** | **SBSAR** Int ***資料型態中輸入的字串*** inputName *名稱* |
| public **void &#x200B;***SetInputBool*（**string** inputName， **bool** value） | 更新 Substance **布林** 輸入 | **字串** *輸入名稱* SBSAR **Bool** *值* 中輸入的名稱 用於更新參數的值 |
| public **bool** *GetInputBool*（**string** inputName） | 取得 Substance **布林輸入** | **SBSAR 中輸入的字串***輸入名稱* |
| public **void &#x200B;***SetInputInt*（**string** inputName， **int** value） | 更新物質 **int** 輸入 | **字串** *輸入名稱* SBSAR **中輸入的名稱 整數***值* 用於更新參數的值 |
| public **int &#x200B;***GetInputInt*（**string** inputName） | 獲取物質 **情報** 輸入 | **SBSAR 中輸入的字串***輸入名稱* |
| public **void** *SetInputVector2Int*（**string** inputName， **int** x， **int** y） | 更新物質 **向量2int** 輸入 | **字串** *inputName* SBSAR **中輸入的名稱 Int** *x* 值用於更新參數 **Int** y 值 用於更新參數 |
| **int[] Substance.Game.SubstanceGraph.GetInputVector2Int**&#x200B;**（字串 inputName） | 取得 2 int 的陣列（Vector2Int 的 x 和 y 值） | &#x200B;** 字串 **&#x200B; *inputName* SBSAR &#x200B;** 中輸入的名稱 Int **&#x200B; *x* 值用於更新參數 &#x200B;** Int** y 值 用於更新參數 |
| **虛無實體。遊戲。實體圖**。*SetInputVector3Int*（字串輸入名稱、整數 x、整數 y、整數 z） | 更新物質向量3Int輸入 | **字串** *輸入名稱* SBSAR **輸入名稱 Int** *x* 用於更新參數 **Int y 值 用於更新參數 Int**&#x200B;**z 值 用於更新參數** |
| **int[] Substance.Game.SubstanceGraph.GetInputVector3Int**&#x200B;**（字串 inputName） | 取得 3 個 int 的陣列（Vector3Int 的 x、y 和 z 值） | &#x200B;** 字串 **&#x200B; *輸入名稱* SBSAR &#x200B;** 輸入名稱 Int **&#x200B; *x* 用於更新參數 &#x200B;** Int y 值 用於更新參數 Int&#x200B;**&#x200B;**&#x200B;z 值 用於更新參數** |
| **虛無實體。遊戲。實體圖**。*SetInputVector4Int*（字串 inputName， int x， int y， int z， int w） | 更新物質向量4Int輸入 | **字串** *輸入名稱* SBSAR **中輸入的名稱 Int** *x* 用於更新參數 **Int y 的值 用於更新參數** Int **z 用於更新參數** Int **&#x200B;**&#x200B;w 的值 用於更新參數 |
| **int[] Substance.Game.SubstanceGraph.GetInputVector4Int**&#x200B;**（字串 inputName） | 取得 4 個 int 的陣列（Vector4Int 的 x、y、z 和 w 值） | &#x200B;** 字串 **&#x200B; *輸入名稱* SBSAR &#x200B;** 中輸入的名稱 Int **&#x200B; *x* 用於更新參數 &#x200B;** Int y 的值 用於更新參數 **&#x200B; Int &#x200B;** z 用於更新參數 **&#x200B; Int &#x200B;**&#x200B;** w 的值 用於更新參數 |
| **虛無實體。遊戲。實體圖**。*SetInputString*（字串 inputName， 字串值） | 更新物質字串輸入 | **SBSAR**&#x200B;輸入中字串 輸入&#x200B;*名稱 用於更新參數的字串&#x200B;***值&#x200B;**&#x200B;** |
| **字串 Substance.Game.SubstanceGraph**。*GetInputString*（字串 inputName） | 取得 Substance 字串輸入 | **SBSAR 中輸入的字串***輸入名稱* |
| **void Substance.Game.SubstanceGraph**。*SetInputTexture*（字串 inputName， Texture2D 值） | 更新 Substance Texture2D 輸入 | **字串** *輸入名稱* SBSAR **Texture2D** *值* 中輸入的名稱，用於更新參數 |
| **Texture2D Substance.Game.SubstanceGraph.GetInputTexture**&#x200B;**（字串 inputName） | 取得 Substance Texture2D 輸入 | &#x200B;** SBSAR 中輸入的字串***輸入名稱* |
| **向量 Int Substance.Game.SubstanceGraph**。*GetTexturesResolution*（） | 取得圖表的目標設定材質解析度（Vector4Int 的 x = 寬度，y = 高度，數值可以是 32、64、128、256、512、1024、2048 和 4096） | 無 |
| **整數 Substance.Game.SubstanceGraph**。*SetTexturesResolution*（向量2Int大小） | 設定圖的目標設定材質解析度（Vector2Int 的 x = 寬度，y = 高度，數值可為 32、64、128、256、512、1024、2048 和 4096）若成功則回傳 0，否則為 -1。 | **用於更新參數的 Vector2Int** *大小* **。 |
| **列表 Substance.Game.SubstanceGraph**。*GetGeneratedTextures*（） | 回傳圖中材質著色器所使用的所有 Substance Texture2D 物件。 | 無 |
| **int Substance.Game.SubstanceGraph.Bake**&#x200B;**（Texture2D texture， string absolutePath） | 為圖形材質著色器中使用的所有 Substance Texture2D 物件產生 .png 檔案。 | 無 |
| Substance。Game。**SubstanceGraph**。*Duplicate*（） | 複製物質圖 | 無 |
| **Substance.Game.SubstanceGraph**。*重複*（字串 newGraphName） | 複製一個物質圖並命名（對應的物質也會有相同名稱） | **字串 newGraphName** |
| Substance.Game。**SubstanceGraph**。*GetInputProperties*（） | 查詢程序式輸入資訊時，會回傳一個「InputProperties」陣列，結構:public 體 InputProperties { 公開字串名稱;// inputName 公共字串標籤;// GUI 公共字串群組中的元件標籤;// GUIpublic string[] componentLabels 中的元件群組;// 用於滑桿（最多 4 個標籤） public string[] enumOptions;// 用於 optionMenupublic InputPropertiesType 類型;public Vector4 最大值;滑桿 public Vector4 最小值;滑桿 公共浮點數步;for sliders }public enum InputPropertiesType { Boolean = 0，// 0 浮點數，// 1 向量2，// 2 向量3，// 3 向量4，// 4 顏色，// 5 枚舉，// 6 紋理，// 7 字串，// 8 無效 = -1// -1 }; | 無 |
| **Bool Substance.Game.SubstanceGraph**。*HasInput*（**字串** inputName）**&#x200B;** | 檢查輸入是否存在於圖中，回傳真/假： | **SBSAR 中輸入的字串***輸入名稱* |
| **bool** **Substance.Game.SubstanceGraph.IsInputVisible**&#x200B;**（**&#x200B;字串 **&#x200B; inputName） | 檢查 visibleif 輸入是否可見，回傳 true/false | &#x200B;** SBSAR 中輸入的字串***輸入名稱* |

## 正在演算

| 公共方法 | 說明 | 參數 |
| --- | --- | --- |
| public **void** *QueueForRender*（） | 將 Substance 圖加入佇列 | 無 |
| mySubstance.** RenderAsync（）* | 非同步渲染所有排隊中的 Substance 圖 | 無 |
| mySubstance.** RenderSync（）* | 同步渲染所有排隊中的 Substance 圖 | 無 |

## 編輯器模式下的腳本：

為了在編輯器模式下讓圖修改永久化，必須重新匯入每個對應的實體。 這是透過以下函數完成的：

```
static void ReImportSubstance(Substance.Game.Substance pSubstance)

{



// Re-import Substance object:

SubstanceImporter importer = AssetImporter.GetAtPath(pSubstance.assetPath) as SubstanceImporter;

importer.CommitSubstanceToImporter(pSubstance); // plugin function

EditorUtility.SetDirty(importer);

importer.SaveAndReimport();



}
```


（使用「CommitSubstanceToImporter」，一個 Substance 外掛函式：將所有修改過的圖形參數和/或輸入複製到 Substance 匯入物件，然後透過 Unity 的匯入機制序列化到磁碟）
