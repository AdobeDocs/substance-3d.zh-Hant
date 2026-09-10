---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/renderers/renderman/renderman-substance-painter.html"
breadcrumb-title: ''
description: 使用 pxrSurface 材質及正確的輸出轉換，匯出 Renderman 的 Substance Painter 貼圖。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Renderers > Renderman > Renderman - Substance Painter
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Renderman - 物質畫家
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '116'
ht-degree: 1%

---


# Renderman - 物質畫家

Substance Painter 2020.1（6.1.0）支援 [**pxrSurface**](https://rmanwiki.pixar.com/display/REN/PxrSurface) 與 pxrDisney [輸出範本](https://docs.substance3d.com/display/SPDOC/Export)。

![](../../../assets/renderman.png)

建議使用 **pxrSurface** 作為輸出。

![](../../../assets/pxrsurface.png)

## Renderman Shader（Maya - RM 23.1）

| 物質畫家出口 | PxrSurface |
| --- | --- |
| 漫光色彩 | 漫射/色彩 |
| 鏡面粗糙度 | 主要鏡面/粗糙度 |
| SpecularFaceColor | 主要鏡面/臉部顏色 |
| 正常 | 全域 / 凸起 / PxrNormalMap → 方向（開放 GL） |
| 置換 | （紅色通道）PxrDispTransform（結果 F） →（純量 Disp） PxrDisplace（出色） →（位移著色器）PxrSurfaceSG |
| 螢光色彩 | 光暈/色彩（增益 = 1.0） |
| 存在感 | 全球聯盟 / 存在感 |

>[!NOTE]
>
> 代表資料的地圖必須被正確解讀。 更多資訊請參閱 [色彩管理](../../../renderers/color-management/color-management.md)頁面。
