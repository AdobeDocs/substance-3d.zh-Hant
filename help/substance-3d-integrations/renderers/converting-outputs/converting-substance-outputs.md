---
helpx_url: "https://helpx.adobe.com/tw/substance-3d-integrations/renderers/converting-substance-outputs.html"
breadcrumb-title: ''
description: 學習如何將 Substance 材質的輸出轉換成符合不同渲染器需求和工作流程的做法。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Renderers > Converting Substance outputs
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 物質輸出轉換
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '161'
ht-degree: 0%

---


# 物質輸出轉換

## 物質畫家

你可以從 Substance Painter 匯出轉換後的地圖。 支援多種渲染預設，只要選擇預設即可轉換貼圖類型。 （轉換依據金屬/粗糙的工作流程進行。）

![](../../assets/convertpainter.png){width="800px"}

## Substance 插件

Substance 插件會產生輸出，並自動為特定工作流程建立材質。 不過，使用 DCC 應用程式和第三方渲染器時，你可能需要手動轉換金屬或粗糙的輸出。 以下整合支援自動渲染工作流程，並在需要時適當轉換任何地圖類型：

* [瑪雅語中的物質](../../3d-applications/maya/using-workflows/using-workflows.md)
* [3ds Max 中的物質](../../3d-applications/3ds-max/3ds-max.md)

## 自訂物質

如果你要做自訂 Substance，可以為渲染器（如 Vray 和 Corona）建立所需的特定輸出。 利用金屬/粗糙度轉換節點（Library>PBR Utilities），你可以輕鬆將基礎色彩、粗糙度和金屬貼圖轉換成特定的渲染器。

![](../../assets/convert-designer.png){width="600px"}
