---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unity/substance-3d-for-unity-scripting.html"
breadcrumb-title: ''
description: 在 Unity 中使用 Substance 3D API 撰寫腳本，在執行時更新和更改 Substance 參數。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Substance 3D for Unity Scripting
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Substance 3D 用於 Unity 腳本
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 0%

---


# Substance 3D 用於 Unity 腳本

本文件部分包含我們透過 Unity 的 Substance 3D 外掛提供的 Substance 3D API 詳細資訊。利用 Substance API，你可以寫腳本在執行時更新和更改 Substance 參數。

## API 概述

這個插件分為三個不同的組件。

* Adobe.Substance
* Adobe.Substance.Editor
* Adobe.Substance.執行環境

### Adobe.Substance

包含與 Substance SDK 互動及產生匹配 Unity 物件的共用元件。 它也包含用於 C# 與 Substance SDK C++ API 之間的編組資料結構。

#### Adobe.Substance.Editor

包含編輯器專用的類別，用於處理 Unity Substance 物件資訊的顯示，以及在專案新增 sbsar 檔案時處理匯入管線。SubstanceEditorEngine 類別是一個單例，負責處理 Substance 引擎及其所有受管理實例的生命週期。

#### Adobe.Substance.執行環境

此類別包含元件，可在執行時執行時處理 Substance 物件的建立與管理。 SubstanceRuntime 相當於執行時的 SubstanceEditorEngine 類別。 它會處理物質引擎的初始化，以及任何實體實例的實例化，讓使用者腳本能互動。

## 執行時使用

為了在執行時修改 Substance Instance 的輸入，必須在場景中新增一個 SubstanceRuntime←- Material（理想狀況是加入與 Substance 材質相同的 GameObject）。 此類別作為輔助工具，使用 Adobe.Substance.Runtime.SubstanceRuntime 單例來設定素材，該單例管理執行時 Substance SDK 物件的實例化。

## 程式碼範例

以下範例展示了如何在執行時使用 SubstanceRuntimeGraph 更改輸入參數。

### 參數變更

```
using System.Collections; 

using System.Collections.Generic; 

using UnityEngine; 

using Adobe.Substance.Runtime; 

public class scifiScript: MonoBehaviour { 

  public Adobe.Substance.Runtime.SubstanceRuntimeGraph mySubstance; 

  // Use this for initialization 

  void Start() { 

    UpdateSubstance(); 

  } 

  public void UpdateSubstance() { 

    // panel color 

    mySubstance.SetInputColor("paint_color", new Color(0.237 f, 0.834 f, 0.045 f, 1.0 f)); 

    // panel size 

    mySubstance.SetInputVector2("square_open", new Vector2(0.101 f, 0.209 f)); 

    // wear level 

    mySubstance.SetInputFloat("wear_level", 0.977 f); 

    // Submit async render. 

    mySubstance.RenderAsync(); 

  } 

}
```


你也可以使用 SubstanceRuntimeGraph 來存取關於 Substance Material 的輸入與輸出資訊。

#### 取得輸入資訊

```
using System.Collections; 

using System.Collections.Generic; 

using UnityEngine; 

using Adobe.Substance.Runtime; 

public class scifiScript: MonoBehaviour { 

  public Adobe.Substance.Runtime.SubstanceRuntimeGraph mySubstance; 

  // Use this for initialization 

  void Start() { 

    UpdateSubstance(); 

  } 

  public void UpdateSubstance() { 

    SubstanceInputDescription desc = mySubstance.GetInputDescription("paint_color"); 

    Debug.Log($ "Input: {desc.Identifier}"); 

    Debug.Log($ "Index: {desc.Index}"); 

    Debug.Log($ "Type: {desc.Type}"); 

    Debug.Log($ "Label: {desc.Label}"); 

  } 

}
```


以下範例展示了如何在編輯器中使用 SubstanceEditorTools 建立自訂預設選單。

##### 建立預設控制。

```
using System.Collections; 

using System.Collections.Generic; 

using UnityEngine; 

using Adobe.Substance.Runtime; 

public class scifiScript: MonoBehaviour { 

  public Adobe.Substance.Runtime.SubstanceRuntimeGraph mySubstance; 

  // Use this for initialization 

  void Start() { 

    UpdateSubstance(); 

  } 

  public void UpdateSubstance() { 

    SubstanceInputDescription desc = mySubstance.GetInputDescription("paint_color"); 

    Debug.Log($ "Input: {desc.Identifier}"); 

    Debug.Log($ "Index: {desc.Index}"); 

    Debug.Log($ "Type: {desc.Type}"); 

    Debug.Log($ "Label: {desc.Label}"); 

  } 

}
```
