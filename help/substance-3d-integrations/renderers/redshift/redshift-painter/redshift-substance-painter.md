---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/renderers/redshift/redshift-substance-painter.html"
breadcrumb-title: ''
description: 使用輸出範本和適當的材質設定，匯出 Redshift 渲染器的 Substance Painter 材質。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Renderers > Redshift > Redshift - Substance Painter
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Redshift - 物質畫家
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '142'
ht-degree: 2%

---


# Redshift - 物質畫家

Substance Painter 2020.1（6.1.0）支援用於金屬/粗糙度的 Redshift [輸出範本](https://docs.substance3d.com/display/SPDOC/Export) （rsMaterial）。 你可以直接用 Redshift 模板匯出，產生與 Redshift 材質相容的材質。

![](../../../assets/rs-export.png)

## 紅移材料設置

| 物質畫家出口 | 紅移物質 |
| --- | --- |
| 顏色 | 漫射/色彩 |
| 粗糙度 | 反射/粗糙度（BRDF = GGX） |
| 金屬性 | 反射/金屬性（菲涅爾類型 = 金屬性） |
| 正常 | 整體 / 凹凸貼圖 / rsBumpMap（輸入貼圖類型 = 切線空間法線 - 高度縮放 = 1.0） |
| 位移高度場 | Displacement Shader / rsDisplacement TexMap（Map Encoding = 高度欄位） |
| 發射色 | 總體 / 排放量（排放重量 = 1.0） |

>[!NOTE]
>
> 代表資料的地圖必須被正確解讀。 更多資訊請參閱 [色彩管理](../../../renderers/color-management/color-management.md)頁面。

## Maya / Redshift 範例

![](https://helpx-prod.scene7.com/is/image/HelpxProd/maya-example?$pjpeg$&jpegSize=300&wid=1583){width="800px"}
