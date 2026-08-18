---
helpx_url: "https://helpx.adobe.com/tw/substance-3d-bake/bakers-settings/curvature-from-mesh.html"
breadcrumb-title: ''
description: 利用光線追蹤從高多邊形網格生成精確的曲率紋理，以達到精準的邊緣偵測。
helpx_creative_field: ""
helpx_description: bakers > Bakers Settings > Curvature from Mesh
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 網格曲率
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 0%

---


# 網格曲率

mesh baker 的曲率會從高多邊形網格產生曲率紋理。 它比基礎 [曲率](../../bakers-settings/curvature/curvature.md) 烘焙器慢，但產生更精確的結果。

**提供：**

* 物質設計師
* 物質自動化工具包
* 物質畫家

## 參數

| *參數* | *描述* |
| --- | --- |
| **次級射線** | 讀取附近幾何形狀所需的光線數量。 較高的數值會產生較少雜訊，但計算時間較長。 預設值是32。 |
| **取樣半徑** | 計算幾何表面曲率時，會考慮鄰近幾何形狀的距離。 高值可能產生較強的邊緣，而較低的值可能產生較薄的邊緣，但會漏掉資訊。 |
| **相對於邊界盒** | 定義取樣半徑是相對於網格大小，還是以單位距離定義。 |
| **自交** | 以曲率射線名稱匹配。 指示烘焙師如何匹配低多邊形與高多邊形。 它可以用來過濾烘焙過程，而不需要手動拆開（爆炸）網格。可能的數值：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>永遠（</strong> 預設）：低多邊形網格會與所有高多邊形網格匹配。</li><li data-preserve-html="true"><strong>依網格名稱</strong>：依網格名稱篩選，以避免與不想要的幾何體匹配。</li></ul>想了解更多關於匹配幾何的資訊，請參見： [以名稱](../../features/matching-by-name/matching-by-name.md)匹配。 |
| **自動音色映射邊界** | 控制曲率值如何寫入貼圖。 啟用後，值範圍會根據烘焙過程中的最小值與最大值在 0 到 1 之間標準化。 若停用，則需手動定義最小值與最大值。  **注意：**  烘焙 UDIM 或 UV 圖塊時，應關閉此參數以使色調映射均勻，而非每個圖塊都特定，否則可能會造成材質間的接縫。 要手動找到正確的最小值/最大值，先開啟這個設定烘焙，然後查看主控台或日誌，看看烘焙者輸出了哪些值。 |
| **音色映射最小值** | 如果 **關閉自動色調映射界限** ，則會定義最小值以縮放曲率結果以符合貼圖。 |
| **音色映射 Max** | 如果 **關閉自動色調映射邊界** ，則會定義最大值以縮放曲率結果以符合貼圖。 |
| **法線貼圖** | 一條可選路徑通往普通材質。 可用來取代烘焙者的內部計算。 |
| **世界空間** | 若啟用，法線貼圖會被解讀為世界空間法線，而非切線空間。 |
| **正常方向** | 若位於切線空間，則法線貼圖格式。可能值：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>DirectX</strong> （預設）</li><li data-preserve-html="true"><strong>OpenGL</strong></li></ul> |
