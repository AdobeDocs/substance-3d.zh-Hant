---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/common-issues/seam-visible-on-every-face.html"
breadcrumb-title: ''
description: 透過檢查 UV 展開、平滑群組和網格拓撲問題，修正每個面上可見的接縫。
helpx_creative_field: ""
helpx_description: bakers > Common Issues > Seam visible on every face
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 每面都能看到接縫
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '195'
ht-degree: 0%

---


# 每面都能看到接縫

>[!WARNING]
>
> **子嗣**
> 
> 即使沒有紫外線接縫，幾何形狀的幾個邊緣仍可見接縫：
> 
> ![](../../assets/seam-every-face.jpg)

>[!NOTE]
>
> **說明**
> 
> 如果沒有使用 [籠子](https://helpx.adobe.com/substance-3d/unlisted/documentation/bake/cage-projection-172822982.html)，烘焙過程會朝著低多邊形網格頂點法線方向發射光線。 如果每個頂點法線都被分割（也就是每個面和鄰面沒有相同的頂點法線），那麼光線在邊上就不會朝同一個方向傳送。 這會導致分裂，因為邊兩側的資訊不同。
> 
> 這個問題還會因為鋸齒而加劇，正如本頁](../../common-issues/aliasing-on-uv-seams/aliasing-on-uv-seams.md)所解釋[的。

>[!NOTE]
>
> **解法**
> 
> 此處僅有兩種解法：
> 
> * 用 [籠](https://helpx.adobe.com/substance-3d/unlisted/documentation/bake/cage-projection-172822982.html) 子來控制光線方向，而不是讓烘焙師從低多邊形幾何來計算。
> * 將低多邊形網格的頂點法線合併（軟化它們/套用共用的平滑群）。
