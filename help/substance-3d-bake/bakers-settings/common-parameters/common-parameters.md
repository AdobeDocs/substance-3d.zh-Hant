---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/bakers-settings/common-parameters.html"
breadcrumb-title: ''
description: 了解適用於所有烘焙師的共通參數，以及如何配置以達到最佳的紋理生成。
helpx_creative_field: ""
helpx_description: bakers > Bakers Settings > Common Parameters
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 常見參數
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '1068'
ht-degree: 0%

---


# 常見參數

所有烘焙師都適用這些共同的參數。 這些參數通常決定烘焙師如何操作高多邊形網格，但最終材質的生成方式。 這些參數中有些可以被特定的烘焙師覆蓋。

雖然這些參數大多在所有軟體（包括 Substance Automation Toolkit）中皆可取得，但其行為可能略有差異;或部分參數因軟體工作流程與實作而無法使用。

## 一般參數

這些參數會影響烘焙者產生貼圖的方式。

| *名稱* | *描述* |
| --- | --- |
| **大小**（預設大小或輸出大小） | 控制烘焙輸出的材質解析度（以像素為單位）。可用值：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>32</strong></li><li data-preserve-html="true"><strong>64</strong></li><li data-preserve-html="true"><strong>128</strong></li><li data-preserve-html="true"><strong>256</strong></li><li data-preserve-html="true"><strong>512</strong></li><li data-preserve-html="true"><strong>1024</strong></li><li data-preserve-html="true"><strong>2048</strong> （預設）</li><li data-preserve-html="true"><strong>4096</strong></li><li data-preserve-html="true"><strong>8192</strong></li></ul>也支援非平方解析度，例如：2048x1024（2：1 比例）。 在 Substance Designer 中，這個參數可以被烘焙者本身覆寫。 |
| **節目形式** | 烘焙材質的檔案格式。*Substance Painter 無法提供。* 參見： [如何匯出烘焙的地圖](../../common-questions/how-export-the-baked-maps/how-to-export-the-baked-maps.md)。 |
| **抗鋸齒** | 控制抗鋸齒，提升烘焙材質品質並減少不同幾何體連接處的鋸齒。欲了解更多鋸齒相關資訊，請參閱： [UV 縫隙](../../common-issues/aliasing-on-uv-seams/aliasing-on-uv-seams.md) 鋸齒及 [維基百科](https://en.wikipedia.org/wiki/Aliasing)鋸齒。可用數值：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>無</strong> （預設）</li><li data-preserve-html="true"><strong>2x2 子取樣</strong></li><li data-preserve-html="true"><strong>4x4 子取樣</strong></li><li data-preserve-html="true"><strong>8x8 子取樣</strong></li></ul>  **注意：**  啟用抗鋸齒會大幅增加烘焙時間，因為抗鋸齒是先以較高解析度計算貼圖，再縮小回原始選取大小。 這表示 2K 材質搭配 2x2 子取樣，實際上會計算出 4K 材質。有時增加烘焙爐中的射線數量比增加子取樣更為可取。 這樣可以不用拖太久就能取得更好的效果。 |
| **UV 集合** | 控制低多邊形網格中哪些 UV 將用於計算烘焙貼圖。*Substance Painter 無法提供。* |
|  |  |
| **擴張（px）** | 將UV外或其邊界的像素放大/延長，依據給定的像素數。 此操作可避免當 UV 邊界未完全對齊貼圖像素或材質解析度降低（例如：mipmaps）時產生接縫。 這是烘焙後的後續處理。 有時也稱為「填充」。想了解更多關於膨脹的資訊，請參考： [UV 接縫](../../common-issues/aliasing-on-uv-seams/aliasing-on-uv-seams.md) 的鋸齒與 [填充](https://helpx.adobe.com/substance-3d/unlisted/documentation/spdoc/padding-134643719.html)。 |
| **施加擴散** | 啟用後，UV 外圍會根據 UV 邊界填充平滑漸層色。 這個過程確保當貼圖大小縮小時，它能保持穩定，不會產生過於明顯的接縫（例如：mipmaps）。 這是烘焙後的後續處理。 |
| **平均常態** | 啟用時，會計算頂點的平均法線，以知道在網格匹配烘焙過程中該向哪個方向傳送光線。 如果停用，光線會遵循網格的原始頂點法線。 |

## 高多邊形參數

以下參數控制高多邊形到低多邊形網格烘焙（「從網格」烘焙器）。

| *名稱* | *描述* |
| --- | --- |
| **高解析度網格** | 包含高多邊形網格的檔案（或 Substance 套件資源）清單。 當烘焙過程開始計算不同資訊並將網格資訊存入貼圖時，烘焙者會將這些資料載入記憶體。 如果啟用「**使用低畫質作為高畫質**」，此清單會被忽略。 |
| **用低解析度當高解析度** ，或 **用低多邊形網格當作高多邊形網格** | 啟用後，提供給烘焙者的高多邊形網格清單會被忽略，低多邊形網格會被烘焙到自己身上。這個參數在直接處理高多邊形網格時非常有用。 例如，當為高多邊形汽車烘焙環境遮蔽貼圖時，啟用此設定時，光線距離會被忽略，烘焙器會產生完美的烘焙效果（沒有射線未命中或幾何不匹配）。 |
|  |  |
| **用籠** 子設定距離或 **用籠子** | 指示烘焙過程中是否使用籠狀網格檔案，而非光線距離值。 籠子控制射線的最大距離與方向。 |
| **籠子檔案** | 通往包含籠子的網格檔案路徑。 |
| **正面值** 或 **最大正面距離** | 控制射線應該在低多邊形表面以上開始尋找路徑上的高多邊形幾何體。*使用此設定在使用籠子時不影響。* |
| **後方距離** 或 **最大後方距離** | 控制射線應該停在低多邊形表面以下，尋找路徑上的高多邊形幾何體。*使用此設定在使用籠子時不影響。* |
| **相對於邊界盒** | 若啟用，光線距離及其他基於尺寸的計算將基於低多邊形網格的正規化空間。 若關閉，射線距離計算將基於匯出時低多邊形網格中指定的單位（公尺、公分等）。有時關閉此設定並在物件有精確測量時手動輸入射線距離會很有用。 |
|  |  |
| **比賽** | 指示烘焙師如何匹配低多邊形與高多邊形。 它可以用來過濾烘焙過程，而不需要手動拆開（爆炸）網格。可能的數值：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>永遠（</strong> 預設）：低多邊形網格會與所有高多邊形網格匹配。</li><li data-preserve-html="true"><strong>依網格名稱</strong>：依網格名稱篩選，以避免與不想要的幾何體匹配。</li></ul>想了解更多關於匹配幾何的資訊，請參見： [以名稱](../../features/matching-by-name/matching-by-name.md)匹配。 |
| **匹配後綴** 或 **高多邊形網格後綴** **低多邊形網格後綴** | 網格名稱後綴用來識別並組合幾何體，使用「按名稱匹配」功能。 可用後綴：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>低多邊形網格</strong>：用來辨識場景中低多邊形網格的後綴</li><li data-preserve-html="true"><strong>高多邊形網格</strong>：用來辨識場景中高多邊形網格的後綴</li><li data-preserve-html="true"><strong>忽略背面：</strong>用來標示特定烘焙者應該忽略的網格（例如 [網格](../../bakers-settings/ambient-occlusion-from/ambient-occlusion-from-mesh.md)環境遮蔽）</li></ul>欲了解更多關於匹配幾何的資訊，請參見： [以名稱](../../features/matching-by-name/matching-by-name.md) 匹配。 |
|  |  |
| **使用斜向校正** | 啟用後，射線方向會根據 **輸入貼圖從平均法線** 或原始幾何法線計算。 貼圖中的黑色值使用計算出來的平均法線，而白色值則使用原始網格法線。*Substance Painter 無法提供。* |
| **斜圖** | 用於偏斜光線投影的貼圖檔案路徑。 |
| **逆偏修正** | 反轉輸入紋理的讀數（黑色變白，白變黑）。 |
