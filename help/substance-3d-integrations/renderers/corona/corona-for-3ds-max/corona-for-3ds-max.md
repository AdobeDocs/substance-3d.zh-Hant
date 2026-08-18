---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/renderers/corona/corona-for-3ds-max.html"
breadcrumb-title: ''
description: 在 3ds Max 中使用 Substance 材質搭配 Corona 渲染器，使用鏡面/光澤處理流程和所需的貼圖。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Renderers > Corona > Corona for 3ds Max
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 3ds Max 版 Corona
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '194'
ht-degree: 0%

---


# 3ds Max 版 Corona

## Substance 在 Maya 外掛中

![](../../../assets/scene-001v03.jpg)

## 新冠 1.6 - 6

使用[3ds Max 插件](../../../3d-applications/3ds-max/3ds-max.md)，你可以在 Substance 選單中選擇 Corona，自動設定 Corona 材質並輸入 Substance 材質。

![](../../../assets/corona.png){width="500px"}

## 科羅娜7 - 9

對於 Corona render 7 及以上版本，選擇「Substance to Corona」並選擇 Substance2 節點，會為 Corona 實體材料建立網路。

![](https://helpx-prod.scene7.com/is/image/HelpxProd/corona-physical-material?$png$&jpegSize=200&wid=857)

* **LiftGamaGain** 是在基礎色彩輸出與基礎色彩輸入之間建立的。 伽瑪值為0.455用於校正色彩差異。
* **CoronaNormal** 是在 Normal 輸出與 Base bump 輸入之間建立，也在 Coat Normal 輸出與 Clearcoat Bump 輸入之間建立。 設定不會改變，但可以在這裡調整到普通模式。
* **CoronaMix** 是在 Sheen Color 輸出與 Sheen 色彩輸入之間建立的。 基層的混合量設為 0，乘數為 2。 使用者可以調整混合量值以控制光澤。
