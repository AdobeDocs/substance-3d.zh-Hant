---
helpx_url: "https://helpx.adobe.com/tw/substance-3d-integrations/game-engines/unity/substance-3d-for-unity-scripting/class-documentation/substanceruntime-class.html"
breadcrumb-title: ''
description: SubstanceRuntime 類別用於 Unity 執行時 Substance 材質操作的參考文件。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Substance 3D for Unity Scripting > Class Documentation > SubstanceRuntime Class
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: SubstanceRuntime 類別
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '134'
ht-degree: 1%

---


# SubstanceRuntime 類別

## Adobe.Substance.Runtime.SubstanceRuntime 類別參考

Singleton 類別負責 Substance 引擎初始化，並用來取得原生處理器到 Substance 實例。\
Adobe.Substance.Runtime.SubstanceRuntime 的繼承圖：

![](../../../../../assets/image2022-6-22-14-35-28.png)

### 公眾會員職能

```
• SubstanceNativeGraph InitializeInstance (SubstanceGraphSO substanceInstance)
```


為特定的 SubstanceGraphSO 建立一個 Substance SDK 的 handle 。

### 屬性

```
• static SubstanceRuntime Instance [get]
```


單例。

### 詳細說明

Singleton 類別負責 Substance 引擎初始化，並用來取得原生處理器到 Substance 實例。

### 成員功能文件

#### InitializeInstance（）

```
SubstanceNativeGraph Adobe.Substance.Runtime.SubstanceRuntime.InitializeInstance  

( SubstanceGraphSO substanceInstance ) [inline]
```


為特定的 SubstanceGraphSO 建立一個 Substance SDK 的 handle 。

**參數**

|  |  |
| --- | --- |
| 實例 | 目標物質圖SO |


**回歸**

Handle 會與 Substance SDK 通訊

### 財產文件

#### 執行個體

```
SubstanceRuntime Adobe.Substance.Runtime.SubstanceRuntime.Instance [static], [get]
```


單例。

全域單例實例。

>[!NOTE]
>
> NativeGraph.InRenderWork 僅供內部使用，僅用於與 Substance 引擎通訊，不應用於自訂工作流程。
