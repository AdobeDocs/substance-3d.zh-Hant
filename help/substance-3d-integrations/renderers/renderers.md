---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/renderers.html"
breadcrumb-title: ''
description: 在你的 3D 工作流程中，使用 Substance 材質搭配 Arnold、V-Ray、Redshift 等主要渲染器。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Renderers
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 渲染器
user-guide-description: ''
user-guide-title: ''
source-git-commit: 4a060ee1aaa1731c04e70d5512e3271cd63d0381
workflow-type: tm+mt
source-wordcount: '226'
ht-degree: 0%

---


# 渲染器

Substance Source 提供的 [Substance 材質包含物理基礎著色器的輸出，並支援[金屬/粗糙度（預設工作流程）及鏡面/光澤工作流程](https://academy.substance3d.com/courses/pbrguides)。](https://source.substance3d.com/)了解你的渲染器材質所支援的工作流程非常重要。 根據渲染器不同，你可能能直接使用 Substance 材質的輸出，或者需要轉換輸出材質。 自訂 Substance 材質或你從 Substance Share 下載的材質，可能不包含特定渲染器所需的適當輸出。

![](../assets/outputs.png){width="200px"}

例如用 Arnold 或 Vray Next，你可以直接使用金屬/粗糙度輸出。 然而，使用 Renderman 的 pxrSurface，底色/金屬色輸出需要轉換成漫反射和鏡面色。 如果支援渲染器，Substance 整合外掛會自動處理這些轉換。

使用 Substance Painter，你可以選擇 [一個輸出範本](https://experienceleague.adobe.com/en/docs/substance-3d-painter/using/getting-started/export/export-window/export-window) ，為特定渲染器建立適當的貼圖類型。 如果你的渲染器預設不支援，你也可以建立自訂的輸出範本。

**Substance Painter 輸出範本**

![](../assets/output-template.png){width="500px"}

## 渲染器指南

* [物質輸出轉換](../renderers/converting-outputs/converting-substance-outputs.md)
* [色彩管理](../renderers/color-management/color-management.md)
* [阿諾德](../renderers/arnold/arnold.md)
* [弗雷](../renderers/vray/vray.md)
* [倫德曼](../renderers/renderman/renderman.md)
* [紅移](../renderers/redshift/redshift.md)
* [麥克斯韋](../renderers/maxwell/maxwell.md)
* [新冠](../renderers/corona/corona.md)
* [辛烷值](../renderers/octane/octane.md)
* [關鍵射擊](../renderers/keyshot/keyshot.md)
* [西雅](../renderers/thea/thea.md)
* [獨行俠](../renderers/maverick/maverick.md)
* [工具包](../renderers/toolbag/toolbag.md)
* [循環與伊布](../renderers/cycles-and-eevee/cycles-and-eevee.md)
