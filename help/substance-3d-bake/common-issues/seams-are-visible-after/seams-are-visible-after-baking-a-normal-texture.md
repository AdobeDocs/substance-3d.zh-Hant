---
helpx_url: "https://helpx.adobe.com/tw/substance-3d-bake/common-issues/seams-are-visible-after-baking-a-normal-texture.html"
breadcrumb-title: ''
description: 透過調整填充、抗鋸齒和 UV 佈局，消除烘焙法線貼圖中可見的接縫。
helpx_creative_field: ""
helpx_description: bakers > Common Issues > Seams are visible after baking a normal texture
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 烘烤正常紋理後，接縫線可見
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '227'
ht-degree: 0%

---


# 烘烤正常紋理後，接縫線可見

>[!WARNING]
>
> **子嗣**
> 
> 即使乾淨烘焙後，網格的 UV 邊界仍可見法線貼圖接縫。

>[!NOTE]
>
> **說明**
> 
> 即使烘烤完美，接縫仍可能看得見。 主要原因是法線將表面資訊近似化成紋理。 有時候貼圖不夠精準，或是低多邊形和高多邊形之間要補償太多，才能達到準確度。 在其他情況下，幾何體與法線貼圖的調整方式會影響畫面的好壞。

>[!NOTE]
>
> **解法**
> 
> 可以嘗試以下幾種可能的解決方案來降低法線貼圖接縫強度：
> 
> * UV 通常沒有對齊像素，導致鋸齒並產生接縫。 更多資訊請參見 [此頁面](../../common-issues/aliasing-on-uv-seams/aliasing-on-uv-seams.md) 。
>   * 提高材質解析度可以減少這種效果。
>   * 將 UV 邊界對齊像素也是減少這種效果的另一種方法。
> * 提高著色器 **品質** 設定。 著色器品質會影響鏡面反射的計算方式。 如果旋轉某些 UV 島，且此參數過低，可能會產生可見接縫。 更多資訊請參見 [此頁面](https://helpx.adobe.com/tw/substance-3d/unlisted/documentation/spdoc/pbr-metal-rough-172818827.html) 。
