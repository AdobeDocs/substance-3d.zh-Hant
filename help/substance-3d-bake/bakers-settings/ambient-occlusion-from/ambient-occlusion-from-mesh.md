---
helpx_url: "https://helpx.adobe.com/tw/substance-3d-bake/bakers-settings/ambient-occlusion-from-mesh.html"
breadcrumb-title: ''
description: 利用光線追蹤技術從高多邊形網格烘焙出精確的環境遮蔽紋理，以提升真實感。
helpx_creative_field: ""
helpx_description: bakers > Bakers Settings > Ambient Occlusion from Mesh
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 來自 Mesh 的環境遮蔽
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '531'
ht-degree: 0%

---


# 來自 Mesh 的環境遮蔽

mesh baker 的環境遮蔽可以從高多邊形網格烘焙出環境遮蔽貼圖。 它比基礎 [環境遮蔽](../../bakers-settings/ambient-occlusion/ambient-occlusion.md) 烘焙器慢，但產生更精確的結果。

**提供：**

* 物質設計師
* 物質自動化工具包
* 物質畫家

## 參數

| *參數* | *描述* |
| --- | --- |
| **次級射線** | 閉塞射線的數量。 較高的數值會產生較少雜訊，但計算時間較長。 預設值是64。 |
| **最小遮擋距離** | 遮蔽射線會接觸到高多邊形幾何體的最小距離。 預設值為 0.00001。 |
| **最大閉塞距離** | 遮蔽射線會到達高多邊形幾何的最大距離。 預設值是 0.1。 |
| **相對於邊界盒** | 啟用時，單位相對於物件的邊界框（1.0 是邊界框的對角長度）。 如果關閉，匯出網格時定義的最小和最大遮蔽距離單位（公尺、公分或匯出場景的單位）。 |
| **擴散角** | 遮蔽射線的最大擴散角。 預設是180度。 |
| **分布** | 遮蔽射線的角分布。 定義了光線如何在與擴散角大小相等的錐體內散射。可能的數值：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>餘弦</strong> （預設）：現實，但在非常薄且遮蔽的區域會出現白線。 比較適合陰影和光線。</li><li data-preserve-html="true"><strong>均勻</strong>：有助於產生線性漸層。 比較適合做層遮罩和其他過濾。</li></ul> |
| **忽略背面** | 此參數定義了遮蔽射線是否會忽略背面的命中（若高多邊形法線面向與射線發射方向相反）。 大多數情況下，這個設定應該開啟以避免雜訊。 可能的數值：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Nevers</strong> （預設）：背面面永遠不會被忽略</li><li data-preserve-html="true"><strong>永遠</strong>：背面永遠被忽略</li><li data-preserve-html="true"><strong>依網格名稱</strong>：背面僅忽略與後綴關鍵字相符的網格。 請參閱 [常見參數](../../bakers-settings/common-parameters/common-parameters.md)。</li></ul> |
| **自我遮蔽** | 閉塞射線的名稱匹配。 指示烘焙師如何匹配低多邊形與高多邊形。 它可以用來過濾烘焙過程，而不需要手動拆開（爆炸）網格。可能的數值：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>永遠（</strong> 預設）：低多邊形網格會與所有高多邊形網格匹配。</li><li data-preserve-html="true"><strong>依網格名稱</strong>：依網格名稱篩選，以避免與不想要的幾何體匹配。</li></ul>想了解更多關於匹配幾何的資訊，請參見： [以名稱](../../features/matching-by-name/matching-by-name.md)匹配。 |
| **法線貼圖** | 一條可選路徑通往普通材質。 可用來取代烘焙者的內部計算。 |
| **世界空間** | 若啟用，法線貼圖會被解讀為世界空間法線，而非切線空間。 |
| **正常方向** | 若位於切線空間，則法線貼圖格式。可能值：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>DirectX</strong> （預設）</li><li data-preserve-html="true"><strong>OpenGL</strong></li></ul> |
| **衰減** | 定義了遮蔽如何因遮擋距離而衰減。可能的數值：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>無</strong>：沒有衰減。</li><li data-preserve-html="true"><strong>線性</strong> （預設）：漸進衰減。</li><li data-preserve-html="true"><strong>平滑</strong>：柔和衰減。</li></ul> |
| **接地平面** | 如果啟用了，模擬一個位於 XZ 軸網格邊界框下方的平面，讓它與次要光線碰撞。 這模擬了來自隱形平面圖的陰影效應。 |
| **接地平面偏移** | 允許將計畫從網格移開，以降低效果強度。 這個數值是絕對的，而不是相對於網格大小。 |
