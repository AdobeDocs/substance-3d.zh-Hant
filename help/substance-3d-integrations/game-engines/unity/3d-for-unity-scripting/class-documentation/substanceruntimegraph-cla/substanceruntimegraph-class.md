---
helpx_url: "https://helpx.adobe.com/tw/substance-3d-integrations/game-engines/unity/substance-3d-for-unity-scripting/class-documentation/substanceruntimegraph-class.html"
breadcrumb-title: ''
description: Unity 中用於執行時圖操作的 SubstanceRuntimeGraph 類別參考文件。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Substance 3D for Unity Scripting > Class Documentation > SubstanceRuntimeGraph Class
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: SubstanceRuntimeGraph 類別
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '290'
ht-degree: 0%

---


# SubstanceRuntimeGraph 類別

## Adobe.Substance.Runtime.SubstanceRuntimeGraph 類別參考

提供執行時功能，可修改輸入並渲染實體圖，讓 Substance←GraphSO 能在執行時產生其資產。

Adobe.Substance.Runtime.SubstanceRuntimeGraph 的繼承圖：

![](../../../../../assets/image2022-10-14-17-53-23-1.png)

### 公眾會員職能

```
• void AttachGraph (SubstanceGraphSO graph)
```


將一個新的圖形物件附加到這個執行時處理器。

```
• void SetInputFloat (string inputName, float value)
```


更新物質浮子輸入

```
• float GetInputFloat (string inputName)
```


取得 Substance Float 輸入

```
• void SetInputVector2 (string inputName, Vector2 value)
```


更新物質向量2輸入

```
• Vector2 GetInputVector2 (string inputName)
```


取得Substance Vector2輸入

```
• void SetInputVector3 (string inputName, Vector3 value)
```


更新物質向量3輸入

```
• Vector3 GetInputVector3 (string inputName)
```


取得物質向量3輸入。

```
• void SetInputVector4 (string inputName, Vector4 value)
```


更新物質向量4輸入

```
• Vector4 GetInputVector4 (string inputName)
```


取得Substance Vector4輸入

```
• void SetInputColor (string inputName, Color value)
```


更新物質顏色輸入

```
• Color GetInputColor (string inputName)
```


取得 Substance Color

```
• void SetInputBool (string inputName, bool value)
```


更新 Substance 布林輸入

```
• bool GetInputBool (string inputName)
```


取得 Substance 布林輸入。

```
• void SetInputInt (string inputName, int value)
```


更新物質 int 輸入

```
• int GetInputInt (string inputName)
```


獲取物質情報輸入

```
• void SetInputVector2Int (string inputName, Vector2Int value)
```


更新物質向量2int輸入。

```
• Vector2Int GetInputVector2Int (string inputName)
```


取得2個智力的陣列。

```
• void SetInputVector3Int (string inputName, Vector3Int value)
```


更新物質向量3int輸入。

```
• Vector3Int GetInputVector3Int (string inputName)
```


取得 3 個 int 的陣列（Vector3Int 的 x、y 和 z 值）

```
• void SetInputVector4Int (string inputName, int x, int y, int z, int w)
```


更新物質向量4Int輸入

```
• int[ ] GetInputVector4Int (string inputName)
```


取得 4 個 int 的陣列（Vector4Int 的 x、y、z 和 w 值）

```
• void SetInputString (string inputName, string value)
```


更新物質字串輸入。

```
• string GetInputString (string inputName)
```


取得 Substance 字串輸入。

```
• SubstanceInputDescription GetInputDescription (string inputName)
```


回傳目標輸入名稱的完整輸入描述。

```
• void SetInputTexture (string inputName, Texture2D value)
```


更新 Substance Texture2D 輸入。

```
• Vector2Int GetTexturesResolution ()
```


回傳實例貼圖輸出解析度。

```
• void SetTexturesResolution (Vector2Int size)
```


設定實例貼圖輸出解析度。

```
• bool HasInput (string inputName)
```


若該實體實例有帶有特定名稱的輸入，則回傳為真。

```
• List< Texture2D > GetGeneratedTextures ()
```


回傳包含該物質實例所有輸出紋理的清單。

```
•  Texture2D GetOutputTexture (string outputName)
```


回傳給定輸出名稱的輸出紋理。

```
• void Render ()
```


會同步渲染物質實例。

```
• Task RenderAsync ()
```


非同步渲染物質實例。

```
• void LoadPreset (string presetXML)
```


使用預設的 XML 來設定圖形輸入參數。

```
• string CreatePresetFromCurrentState ()
```


將當前圖形狀態儲存為預設的 XML。

## 公開屬性

```
• SubstanceGraphSO GraphSO
```


目標物質實例。

## 受保護會員職能

```
• void Awake ()
```


在 awake 時，SubstanceRuntime 會被用來建立 substanceGraphSO 在 substance 中建立一個實例

SDK。

```
• void Update ()
```


請檢查渲染 ConcurrentQueue 的渲染結果。

```
• void OnDestroy ()
```


丟棄 substance SDK 處理器。

## 屬性

```
• Material DefaulMaterial [get]
```


物質實例產生的主要素材。
