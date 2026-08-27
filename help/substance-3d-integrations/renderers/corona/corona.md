---
helpx_url: "https://helpx.adobe.com/tw/substance-3d-integrations/renderers/corona.html"
breadcrumb-title: ''
description: 在 3ds Max 中使用 Substance 材質搭配 Corona 渲染器，使用鏡面/光澤的工作流程和所需的貼圖。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Renderers > Corona
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 新冠
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '154'
ht-degree: 1%

---


# 新冠

用 Corona 渲染時，你可以使用 Substance Painter 或 Substance 插件匯出的貼圖。 Corona 採用 Specular/Glossiness 工作流程，並搭配 1/IOR 映射。 你需要以下地圖：

* 擴散
* 反射（鏡面）
* 光澤度
* 1/IOR（改裝）

1/IOR 的貼圖只能從金屬/粗糙度工作流程轉換，而金屬/粗糙度工作流程是 Substance Designer 和 Substance Painter 的預設工作流程。

1. 使用 Corona 預設從 Substance Painter 匯出地圖。
1. 對於自訂物質，你可以用 basecolor\_metallic\_roughness 轉換節點設定為 Vray 預設來建立自訂輸出。
1. 對於 3ds Max 和 Cinema 4D，你會用分層的 Corona 材質來處理金屬和介電材料，這樣就不用轉換 1/IOR 的地圖了。

## 目錄

* [3ds Max 版 Corona](../../renderers/corona/corona-for-3ds-max/corona-for-3ds-max.md)
* [Corona - 物質畫家](../../renderers/corona/corona-painter/corona-substance-painter.md)
