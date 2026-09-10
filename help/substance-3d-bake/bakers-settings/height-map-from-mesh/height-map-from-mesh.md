---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/bakers-settings/height-map-from-mesh.html"
breadcrumb-title: ''
description: 從高多邊形網格建立高度貼圖，捕捉表面細節和幾何資訊以進行貼圖。
helpx_creative_field: ""
helpx_description: bakers > Bakers Settings > Height Map from Mesh
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 網格高度圖
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '111'
ht-degree: 0%

---


# 網格高度圖

mesh baker 的 Height Map 允許你從高多邊形網格建立高度圖。**提供：**

* 畫家
* 設計師
* 自動化工具包

## 參數

| *參數* | *描述* |
| --- | --- |
| **&#x200B;**&#x200B;正規化&#x200B;**&#x200B;** | 定義了如何將數值的高度範圍儲存到貼圖中。可能的數值：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>相對於光線距離</strong>：</li><li data-preserve-html="true"><strong>相對於低多邊形網格（每個 UV 圖塊）（</strong> 預設值）</li><li data-preserve-html="true"><strong>相對於最小/最大值（每個UV圖塊）</strong></li><li data-preserve-html="true"><strong>手排</strong></li></ul> |
| **縮放除子** | 定義高度值應該乘多少或除多少。只有當 **正規化** 設定為 **手動**&#x200B;時才可用。 |
