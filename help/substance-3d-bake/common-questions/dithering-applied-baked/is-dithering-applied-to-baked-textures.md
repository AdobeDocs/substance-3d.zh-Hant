---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/common-questions/is-dithering-applied-to-baked-textures.html"
breadcrumb-title: ''
description: 了解抖動是否應用在烘焙的貼圖上，以及它如何影響貼圖品質。
helpx_creative_field: ""
helpx_description: "bakers > Common Questions > Is dithering applied to baked textures "
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: '抖動是應用在烘焙的貼圖上嗎 '
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '140'
ht-degree: 0%

---


# 抖動會應用在烘焙的貼圖上嗎？

>[!WARNING]
>
> **問題**
> 
> Bakers 支援貼圖 [抖動](https://en.wikipedia.org/wiki/Dither) 嗎？如果支援，通常在什麼時候使用？

>[!NOTE]
>
> **說明**
> 
> 例如，8位元法線貼圖中會施加抖動以避免條紋現象：
> 
> ![](../../assets/dither.jpg)

>[!NOTE]
>
> **解決方案：Substance Designer**
> 
> 抖動會在以下情況下自動應用：
> 
> * 當 Baker 輸出被儲存成 8 位元的貼圖檔時
> * 當 Baker 輸出被用於設定為 8 位元的圖的位圖節點時，

>[!NOTE]
>
> **解答：物質畫家**
> 
> 抖動是一個可以在匯出過程中啟用或關閉的選項。 僅在匯出為 8bit 檔案格式的 Normal、Displacement 和 Height 通道時才會套用此項。

>[!NOTE]
>
> **解決方案：物質自動化工具包**
> 
> 目前不支援抖動。
