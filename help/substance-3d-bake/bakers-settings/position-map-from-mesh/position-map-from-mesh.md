---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/bakers-settings/position-map-from-mesh.html"
breadcrumb-title: ''
description: 從高多邊形網格計算精確位置圖，以捕捉精確的幾何位置資訊。
helpx_creative_field: ""
helpx_description: bakers > Bakers Settings > Position map from Mesh
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 來自網格的位置圖
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '221'
ht-degree: 0%

---


# 來自網格的位置圖

mesh baker 中的 Position map 會計算高多邊形網格幾何體的位置，並儲存成貼圖。 它與基底位置烘焙器相似，但能產生更精確的結果。

**提供：**

* 物質設計師
* 物質自動化工具包

## 參數

| *參數* | *描述* |
| --- | --- |
| **模式** | 控制哪些資訊會被計算到位置貼圖中。可能的數值：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>所有軸：</strong> 將 X、Y 和 Z 軸的位置烘焙到輸出材質的 RGB 通道中。</li><li data-preserve-html="true"><strong>一個軸：</strong> 將單一軸以灰階影像形式烘焙到輸出材質中。</li></ul> |
| **軸心國** | 定義若&#x200B;**&#x200B;**&#x200B;模式參數設為 **One 軸**，應計算哪個軸。 |
| **正規化類型** | 定義如何依軸縮放位置值。可能的數值：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>BBox：</strong> 根據網格體積（包圍盒長度）來標準化每個軸。</li><li data-preserve-html="true"><strong>BSphere：</strong> 根據網格體積半徑（包圍球體）來正規化所有軸。</li></ul> |
| **正規化尺度** | 定義如何根據網格縮放位置值。可能的數值：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>每個材質</strong>：每個材質（材質集）的數值會調整為 0 到 1 之間。</li><li data-preserve-html="true"><strong>完整場景</strong> （預設）：數值會縮放以考慮整個網格。 這允許物件與材質間連續的位置值（紋理集）。</li></ul> |
