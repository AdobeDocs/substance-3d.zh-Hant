---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/common-issues/normal-texture-looks-faceted.html"
breadcrumb-title: ''
description: 透過平滑網格法線和調整平滑群組設定來修正法線貼圖中的多面呈現。
helpx_creative_field: ""
helpx_description: bakers > Common Issues > Normal texture looks faceted
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 一般材質看起來像多面體
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '201'
ht-degree: 0%

---


# 一般材質看起來像多面體

>[!WARNING]
>
> **子嗣**
> 
> 法線貼圖看起來像是多面體，或者烘焙後網格的每個面都可見。
> 
> ![](../../assets/normal-faceted.jpg)

>[!NOTE]
>
> **說明**
> 
> 烘焙法線會產生這種結果的主要原因是低多邊形網格法線設定不正確。 每個面的每一邊都是硬邊，使得與高多邊形網格匹配時的光線投影忽略鄰居資訊，反而產生接縫或無意識資訊。 雖然在網格上看起來沒問題，但這可能會導致日後的陰影問題，應該要解決。

>[!NOTE]
>
> **解法**
> 
> 主要解決方案是重新設計頂點法線或低多邊形網格，具體命名取決於 3D 建模軟體：
> 
> * 在 Maya 和 Houdini 裡使用 **平均法線** 。
> * 在 3DS Max 裡只用 **一個平滑群組** 。
> * 用 Blender 裡的 **Smooth shade** 。
> * 從 zBrush 匯出的網格總是會被分面處理，應該在其他軟體中清理。
> 
> 請注意，這可能不夠：確保設定在匯出網格時也能儲存或產生頂點法線或著色資訊。
