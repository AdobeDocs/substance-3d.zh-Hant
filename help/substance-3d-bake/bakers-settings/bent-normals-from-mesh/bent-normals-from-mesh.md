---
helpx_url: "https://helpx.adobe.com/tw/substance-3d-bake/bakers-settings/bent-normals-from-mesh.html"
breadcrumb-title: ''
description: 計算彎曲法線貼圖，描述高多邊形網格環境光照的平均方向。
helpx_creative_field: ""
helpx_description: bakers > Bakers Settings > Bent Normals from Mesh
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Mesh 的彎曲法線
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 0%

---


# Mesh 的彎曲法線

mesh baker 的彎曲法線計算出描述環境光照平均方向的紋理。 這個烘焙器是從 [Mesh](../../bakers-settings/ambient-occlusion-from/ambient-occlusion-from-mesh.md) Baker 的環境遮蔽技術衍生而來。

**提供：**

* 畫家
* 設計師
* 自動化工具包

## 參數

| *參數* | *描述* |
| --- | --- |
| **次級射線** | 閉塞射線的數量。 較高的數值會產生較少雜訊，但計算時間會較長。 |
| **最小遮擋距離** | 遮蔽射線會接觸到高多邊形幾何的最小距離。 |
| **最大閉塞距離** | 遮蔽射線會到達高多邊形幾何的最大距離。 |
| **相對於邊界盒** | 啟用時，射線距離計算基於低多邊形網格的正規化空間（0 到 1）。 若關閉，射線距離計算將基於匯出時低多邊形網格中指定的單位（公尺、公分等）。 |
| **擴散角** | 遮蔽射線的最大擴散角。 預設是180度。 |
| **分布** | 遮蔽射線的角分布。可能的數值：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>餘弦</strong> （預設值）</li><li data-preserve-html="true"><strong>制服</strong></li></ul> |
| **忽略背面** | 啟用時，遮蔽射線會忽略背面的命中（如果高多邊形法線朝向與射線發射方向相反）。 大多數情況下，這個設定應該開啟以避免雜訊。 |
| **自我遮蔽** | 閉塞射線的名稱匹配。 指示烘焙師如何匹配低多邊形與高多邊形。 它可以用來過濾烘焙過程，而不需要手動拆開（爆炸）網格。可能的數值：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>永遠（</strong> 預設）：低多邊形網格會與所有高多邊形網格匹配。</li><li data-preserve-html="true"><strong>依網格名稱</strong>：依網格名稱篩選，以避免與不想要的幾何體匹配。</li></ul>想了解更多關於匹配幾何的資訊，請參見： [以名稱](../../features/matching-by-name/matching-by-name.md)匹配。 |
| **地圖類型** | 定義輸出材質的類型。可能的數值：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>世界空間</strong></li><li data-preserve-html="true"><strong>切空間</strong> （預設）</li></ul> |
| **正常方向** | 若 **Mat Type** 設為 Tangent Space，則控制輸出材質的正常格式。可能值：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>OpenGL</strong> <strong> <br/></strong></li><li data-preserve-html="true"><strong>DirectX</strong> （預設）<strong> <br/></strong></li></ul> |
