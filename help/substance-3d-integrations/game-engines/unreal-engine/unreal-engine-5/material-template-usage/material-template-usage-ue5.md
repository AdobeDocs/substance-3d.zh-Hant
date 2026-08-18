---
helpx_url: "https://helpx.adobe.com/tw/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-5/material-template-usage-ue5.html"
breadcrumb-title: ''
description: 在 Unreal Engine 5 中建立並使用材質範本，來定義 Substance 輸出節點如何連接到材質輸入。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 5 > Material Template Usage - UE5
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 材質範本使用 - UE5
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '197'
ht-degree: 0%

---


# 材質範本使用 - UE5

材料範本允許使用者建立物質的基礎材料，作為連接其輸出節點與材料輸入的範本。\
與材料輸入名稱和類型相同的輸出會自動使用。 這個 Parent Material 範例有一個「baseColor」材質樣本節點，如果 Substance 有同樣名為「baseColor」的材質輸出，該節點會被填滿。\
![](../../../../assets/parent-material-sample.png)

Substance 輸出支援更新材質、單一浮點數或整數數值，以及向量（2-4）值。 要在執行時使用 float 或整數輸出，必須從圖取得 dynamicMaterialInstance，因為 constantMaterialInstances（編輯器產生的任何材質）在執行時無法更改純量值。

![](https://helpx-prod.scene7.com/is/image/HelpxProd/scalar-value?$png$&jpegSize=100&wid=245)

實例會嘗試在建立時填補所有相關的輸出值。

![](https://helpx-prod.scene7.com/is/image/HelpxProd/screen-shot-2022-04-01-at-4-38-31-pm?$png$&jpegSize=200&wid=1076)
