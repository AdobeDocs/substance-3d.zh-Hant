---
helpx_url: "https://helpx.adobe.com/tw/substance-3d-bake/common-issues/mesh-parts-bleed-between-each-other.html"
breadcrumb-title: ''
description: 使用「按名稱匹配」或調整距離，避免網格零件在烘焙過程中互相滲透。
helpx_creative_field: ""
helpx_description: bakers > Common Issues > Mesh parts bleed between each other
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 網狀零件會彼此滲出
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '131'
ht-degree: 0%

---


# 網狀零件會彼此滲出

>[!WARNING]
>
> **子嗣**
> 
> 網格幾何會在其他部分滲出並產生瑕疵。
> 
> ![](../../assets/bleed-example.png)

>[!NOTE]
>
> **說明**
> 
> 烘焙過程會從低多邊形網格表面發射光線，照射到高多邊形網格以產生匹配。 有時光線會射得太遠，碰到錯誤的幾何結構，造成出血和瑕疵。

>[!NOTE]
>
> **解法**
> 
> 有幾種解決方案可以避免此問題：
> 
> * 使用 [「依名稱](../../features/matching-by-name/matching-by-name.md) 匹配」功能來隔離網格
> * 用 [籠](https://helpx.adobe.com/tw/substance-3d/unlisted/documentation/bake/cage-projection-172822982.html) 子來限制光線距離。
> * 在通用烘焙設定中將預設光線距離調低。
