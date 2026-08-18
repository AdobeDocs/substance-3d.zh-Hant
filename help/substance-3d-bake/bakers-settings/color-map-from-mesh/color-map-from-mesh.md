---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/bakers-settings/color-map-from-mesh.html"
breadcrumb-title: ''
description: 將高多邊形網格的色彩屬性投射到材質中，烘焙多邊形塗料或材質 ID，用於選取遮罩。
helpx_creative_field: ""
helpx_description: bakers > Bakers Settings > Color Map from Mesh
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 從網格取得色彩映射
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '203'
ht-degree: 0%

---


# 從網格取得色彩映射

這個來自 mesh baker 的色彩貼圖，將高解析度網格的色彩屬性投影到貼圖中。 它可以用來烘焙多重色或材質 ID，以建立選取遮罩。

**提供：**

* 物質設計師
* 物質自動化工具包
* 物質畫家

## 參數

| *參數* | *描述* |
| --- | --- |
| **色彩來源** | 控制色生成應該基於高多邊形網格的屬性。可能的數值：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>頂點顏色：讀取頂點顏色並將其</strong>存入貼圖中。 顏色從一個頂點插值到另一個頂點。</li><li data-preserve-html="true"><strong>材質顏色</strong>：讀取分配給多邊形面的材質顏色。</li><li data-preserve-html="true"><strong>網格 ID</strong>：為每個找到的物件分配顏色。</li><li data-preserve-html="true"><strong>多重組 / 子網格 ID</strong>：為子物件（也稱為元素）指派顏色。</li></ul> |
| **色彩產生器** | 定義當 **色彩來源** 設定為 **網格 ID** 或 **多重組/子網格 ID** 時，顏色的產生方式。可能的值：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>隨機</strong>：每個物體或子物體都被隨機生成的顏色所著色。</li><li data-preserve-html="true"><strong>色相移：</strong>每個物體或子物體都以基於色相的獨特顏色著色。</li><li data-preserve-html="true"><strong>灰階</strong>：每個物體或子物體都以獨特的灰階值著色。</li></ul> |
