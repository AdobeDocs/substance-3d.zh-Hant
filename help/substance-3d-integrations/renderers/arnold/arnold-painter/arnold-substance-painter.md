---
helpx_url: "https://helpx.adobe.com/tw/substance-3d-integrations/renderers/arnold/arnold-substance-painter.html"
breadcrumb-title: ''
description: 使用 Substance Painter 的 Arnold 渲染器輸出範本，搭配 aiStandard 材質來進行物理渲染。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Renderers > Arnold > Arnold - Substance Painter
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 阿諾德 - 物質畫家
user-guide-description: ''
user-guide-title: ''
source-git-commit: 4a060ee1aaa1731c04e70d5512e3271cd63d0381
workflow-type: tm+mt
source-wordcount: '162'
ht-degree: 1%

---


# 阿諾德 - 物質畫家

Substance Painter 2020.1（6.1.0）附帶[&#128279;](https://experienceleague.adobe.com/en/docs/substance-3d-painter/using/getting-started/export/output-templates/export-presets)使用 [aiStandard 材質](https://docs.arnoldrenderer.com/display/A5AFMUG/Standard+Surface)的 Arnold 輸出範本。

![](../../../assets/arnold-export.png){width="800px"}

## Arnold 標準著色器（Arnold 5 及以上）

| 物質畫家出口 | Arnold AiStandardSurface |
| --- | --- |
| 基色 | 底色 / 顏色 |
| 粗糙度 | 鏡面/粗糙度 |
| 金屬性 | 基底 / 金屬感 |
| 正常 | （**Maya**） 幾何體/凹凸貼圖 / bump2d（用作切線空間法線）（**3ds** **max**）法線位圖→ |
| 高度 | （**Maya**） 位移著色器 / 位移（**3ds** **Max**） 物件修改器 → Arnold 屬性 → 位移 → 使用貼圖 |
| 發射體 | 發射/顏色（排放重量 = 1.0） |
| 各向異性層級（不包含在預設的 Arnold 輸出範本中） | （**Maya**）外套/各向異性（**3ds** **Max**）外套/各向異性 |
| 各向異性層級（不包含在預設的 Arnold 輸出範本中） | （**Maya**）外套/旋轉（**3ds** **Max**）外套/旋轉 |

>[!NOTE]
>
> 代表資料的地圖必須被正確解讀。 更多資訊請參閱 [色彩管理](../../../renderers/color-management/color-management.md)頁面。
