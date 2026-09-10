---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/bakers-settings/thickness-map-from-mesh.html"
breadcrumb-title: ''
description: 透過從網格表面向內投射光線來產生厚度貼圖，用於 SSS 著色器和遮罩。
helpx_creative_field: ""
helpx_description: bakers > Bakers Settings > Thickness Map from Mesh
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 從網格取得厚度貼圖
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '387'
ht-degree: 0%

---


# 從網格取得厚度貼圖

網格的厚度貼圖和環境遮蔽烘焙器非常相似，但它會從網格表面投射光線到內部。 此貼圖可用於次表面散射（SSS）著色器或遮罩貼圖。

紋理屬性定義為：

* 黑色值代表模型中較薄的部分。
* 白色值代表模型的厚部分。

**提供：**

* 物質畫家
* 物質設計師
* 物質自動化工具包

## 參數

| *參數* | *描述* |
| --- | --- |
| **次級射線** | 閉塞射線的數量。 較高的數值會產生較少雜訊，但計算時間較長。 預設值是64。 |
| **最小遮擋距離** | 遮蔽射線會接觸到高多邊形幾何體的最小距離。 預設值為 0.00001。 |
| **最大閉塞距離** | 遮蔽射線會到達高多邊形幾何的最大距離。 預設值是 0.1。 |
| **相對於邊界盒** | 啟用時，單位相對於物件的邊界框（1.0 是邊界框的對角長度）。 如果關閉，匯出網格時定義的最小和最大遮蔽距離單位（公尺、公分或匯出場景的單位）。 |
| **擴散角** | 遮蔽射線的最大擴散角。 預設是180度。 |
| **分布** | 遮蔽射線的角分布。可能的數值：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>餘弦</strong> （預設值）</li><li data-preserve-html="true"><strong>制服</strong></li></ul> |
| **忽略背面** | 啟用時，遮蔽射線會忽略背面的命中（如果高多邊形法線朝向與射線發射方向相反）。 大多數情況下，這個設定應該開啟以避免雜訊。 |
| **自我遮蔽** | 閉塞射線的名稱匹配。 指示烘焙師如何匹配低多邊形與高多邊形。 它可以用來過濾烘焙過程，而不需要手動拆開（爆炸）網格。可能的數值：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>永遠（</strong> 預設）：低多邊形網格會與所有高多邊形網格匹配。</li><li data-preserve-html="true"><strong>依網格名稱</strong>：依網格名稱篩選，以避免與不想要的幾何體匹配。</li></ul>想了解更多關於匹配幾何的資訊，請參見： [以名稱](../../features/matching-by-name/matching-by-name.md)匹配。 |
| **自動正規化** | 定義輸出值是否應該調整成 0-1 範圍（最亮點設為純白，最暗點設為純黑）。 |
