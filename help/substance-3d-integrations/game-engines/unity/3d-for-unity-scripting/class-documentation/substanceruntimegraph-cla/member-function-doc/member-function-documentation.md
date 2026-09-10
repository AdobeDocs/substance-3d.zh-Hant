---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unity/substance-3d-for-unity-scripting/class-documentation/substanceruntimegraph-class/member-function-documentation.html"
breadcrumb-title: ''
description: Unity腳本中SubstanceRuntimeGraph類別所有成員函式的詳細文件。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Substance 3D for Unity Scripting > Class Documentation > SubstanceRuntimeGraph Class > Member Function Documentation
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 成員功能文件
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '662'
ht-degree: 0%

---


# 成員功能文件

## AttachGraph（）

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.AttachGraph  

( SubstanceGraphSO graph ) [inline]
```


將一個新的圖形物件附加到這個執行時處理器。

**參數**

|  |  |
| --- | --- |
| 圖表 | 目標物質圖表。 |

### CreatePresetFromCurrentState（）

```
string Adobe.Substance.Runtime.SubstanceRuntimeGraph.CreatePresetFromCurrentState ( ) [inline]
```


將當前圖形狀態儲存為預設的 XML。

**回歸**

預設是利用圖形輸入目前狀態建立的。

### GetGeneratedTextures（）

```
List< Texture2D > Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetGeneratedTextures ( ) [inline]
```


回傳包含該物質實例所有輸出紋理的清單。

**回歸**

輸出貼圖。

### GetInputBool（）

```
bool Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetInputBool ( string inputName ) [inline]
```


取得 Substance 布林輸入。

**參數**

|  |  |
| --- | --- |
| 輸入名稱 | SBSAR 中輸入的名稱。 |


**回歸**

目前輸入值。

### GetInputColor（）

```
Color Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetInputColor ( string inputName ) [inline]
```


取得 Substance Color

**參數**

|  |  |
| --- | --- |
| 輸入名稱 | SBSAR 中輸入的名稱 |


**回歸**

目前輸入值。

### GetInputDescription（）

```
SubstanceInputDescription Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetInputDescription ( string inputName ) [inline]
```


回傳目標輸入名稱的完整輸入描述。

**參數**

|  |  |
| --- | --- |
| 輸入名稱 | 目標輸入名稱。 |


**回歸**

目標輸入的完整描述。

### GetInputFloat（）

```
float Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetInputFloat ( string inputName ) [inline]
```


取得 Substance Float 輸入

**參數**

|  |  |
| --- | --- |
| 輸入名稱 | SBSAR 中輸入的名稱 |


**回歸**

目前輸入值。

### GetInputInt（）

```
int Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetInputInt ( string inputName ) [inline]
```


獲取物質情報輸入

**參數**

|  |  |
| --- | --- |
| 輸入名稱 | SBSAR 中輸入的名稱 |


**回歸**

目前輸入值。

### GetInputString（）

```
string Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetInputString ( string inputName ) [inline]
```


取得 Substance 字串輸入。

**參數**

|  |  |
| --- | --- |
| 輸入名稱 | SBSAR 中輸入的名稱 |


**回歸**

輸入電流值。

### GetInputVector2（）

```
Vector2 Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetInputVector2 ( string inputName ) [inline]
```


取得Substance Vector2輸入

**參數**

|  |  |
| --- | --- |
| 輸入名稱 | SBSAR 中輸入的名稱 |


**回歸**

目前輸入值。

### GetInputVector2Int（）

```
Vector2Int Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetInputVector2Int ( string inputName ) [inline]
```


取得2個智力的陣列。

**參數**

|  |  |
| --- | --- |
| 輸入名稱 | SBSAR 中輸入的名稱 |


**回歸**

目前輸入值。

### GetInputVector3（）

```
Vector3 Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetInputVector3 ( string inputName ) [inline]
```


取得物質向量3輸入。

**參數**

|  |  |
| --- | --- |
| 輸入名稱 | SBSAR 中輸入的名稱 |


**回歸**

目前輸入值。

### GetInputVector3Int（）

```
Vector3Int Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetInputVector3Int ( string inputName ) [inline]
```


取得 3 個 int 的陣列（Vector3Int 的 x、y 和 z 值）

**參數**

|  |  |
| --- | --- |
| 輸入名稱 | SBSAR 中輸入的名稱 |


**回歸**

目前輸入值。

### GetInputVector4（）

```
Vector4 Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetInputVector4 ( string inputName ) [inline]
```


取得Substance Vector4輸入

**參數**

|  |  |
| --- | --- |
| 輸入名稱 | SBSAR 中輸入的名稱 |


**回歸**

目前輸入值。

### GetInputVector4Int（）

```
int[] Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetInputVector4Int ( string inputName ) [inline]
```


取得 4 個 int 的陣列（Vector4Int 的 x、y、z 和 w 值）

**參數**

|  |  |
| --- | --- |
| 輸入名稱 | SBSAR 中輸入的名稱 |


**回歸**

目前輸入值。

### GetOutputTexture（）

```
Texture2D Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetOutputTexture ( string outputName ) [inline]
```


回傳給定輸出名稱的輸出紋理。

**參數**

|  |  |
| --- | --- |
| outputName | 輸出名稱。 |


**回歸**

輸出貼圖。

### GetTexturesResolution（）

```
Vector2Int Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetTexturesResolution ( ) [inline]
```


回傳實例貼圖輸出解析度。

**回歸**

電流輸出解析度。

### HasInput（）

```
bool Adobe.Substance.Runtime.SubstanceRuntimeGraph.HasInput ( string inputName ) [inline]
```


若該實體實例有帶有特定名稱的輸入，則回傳為真。

**參數**

|  |  |
| --- | --- |
| 輸入名稱 | 輸入名稱。 |


**回歸**

若實例的輸入與該名稱相同，則為 TRUE。

### LoadPreset（）

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.LoadPreset ( string presetXML ) [inline]
```


使用預設的 XML 來設定圖形輸入參數。

**參數**

|  |  |
| --- | --- |
| presetXML | 預設的 XML 資料。 |

### RenderAsync（）

```
Task Adobe.Substance.Runtime.SubstanceRuntimeGraph.RenderAsync ( ) [inline]
```


非同步渲染物質實例。

**回歸**

這個任務會在渲染完成後完成。

### SetInputBool（）

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.SetInputBool ( string inputName, 

bool value ) [inline]
```


更新 Substance 布林輸入

**參數**

|  |  |
| --- | --- |
| 輸入名稱 | SBSAR 中輸入的名稱 |
| 價值 | 用於更新參數的值 |

### SetInputColor（）

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.SetInputColor ( string inputName, 

Color value ) [inline]
```


更新物質顏色輸入

**參數**

|  |  |
| --- | --- |
| 輸入名稱 | SBSAR 中輸入的名稱 |
| 價值 | 用於更新參數的值 |

### SetInputFloat（）

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.SetInputFloat ( string inputName, 

float value ) [inline]
```


更新物質浮子輸入

**參數**

|  |  |
| --- | --- |
| 輸入名稱 | SBSAR 中輸入的名稱 |
| 價值 | 用於更新參數的值 |

### SetInputInt（）

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.SetInputInt ( string inputName, 

int value ) [inline]
```


更新物質 int 輸入

**參數**

|  |  |
| --- | --- |
| 輸入名稱 | SBSAR 中輸入的名稱 |
| 價值 | 用於更新參數的值 |

### SetInputString（）

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.SetInputString ( string inputName, 

string value ) [inline]
```


更新物質字串輸入。

**參數**

|  |  |
| --- | --- |
| 輸入名稱 | SBSAR 中輸入的名稱 |
| 價值 | 用於更新參數的值 |

### SetInputTexture（）

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.SetInputTexture (string inputName, 

Texture2D value ) [inline]
```


更新 Substance Texture2D 輸入。

**參數**

|  |  |
| --- | --- |
| 輸入名稱 | SBSAR 中輸入的名稱 |
| 價值 | 用於更新參數的值 |

### SetInputVector2（）

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.SetInputVector2 ( string inputName, 

Vector2 value ) [inline]
```


更新物質向量2輸入

**參數**

|  |  |
| --- | --- |
| 輸入名稱 | SBSAR 中輸入的名稱 |
| 價值 | 用於更新參數的值 |

### SetInputVector2Int（）

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.SetInputVector2Int ( string inputName, 

Vector2Int value ) [inline]
```


更新物質向量2int輸入。

**參數**

|  |  |
| --- | --- |
| 輸入名稱 | SBSAR 中輸入的名稱 |
| 價值 | 用於更新參數的值 |

### SetInputVector3（）

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.SetInputVector3 ( string inputName, 

Vector3 value ) [inline]
```


更新物質向量3輸入

**參數**

|  |  |
| --- | --- |
| 輸入名稱 | SBSAR 中輸入的名稱 |
| 價值 | 用於更新參數的值 |

### SetInputVector3Int（）

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.SetInputVector3Int ( string inputName, 

Vector3Int value ) [inline]
```


更新物質向量3int輸入。

**參數**

|  |  |
| --- | --- |
| 輸入名稱 | SBSAR 中輸入的名稱 |
| 價值 | 用於更新參數的值 |

### SetInputVector4（）

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.SetInputVector4 ( string inputName, 

Vector4 value ) [inline]
```


更新物質向量4輸入

**參數**

|  |  |
| --- | --- |
| 輸入名稱 | SBSAR 中輸入的名稱 |
| 價值 | 用於更新參數的值 |

### SetInputVector4Int（）

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.SetInputVector4Int ( string inputName, 

int x, 

int y, 

int z, 

int w ) [inline]
```


更新物質向量4Int輸入

**參數**

|  |  |
| --- | --- |
| 輸入名稱 | SBSAR 中輸入的名稱 |
| x | 用於更新參數的值 |
| y | 用於更新參數的值 |
| z | 用於更新參數的值 |
| w | 用於更新參數的值 |

### SetTexturesResolution（）

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.SetTexturesResolution ( Vector2Int size ) [inline]
```


設定實例貼圖輸出解析度。

**參數**

|  |  |
| --- | --- |
| 規模 |  |
