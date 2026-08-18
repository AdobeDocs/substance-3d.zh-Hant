---
helpx_url: "https://helpx.adobe.com/tw/substance-3d-bake/common-questions/why-is-matching-by-name-not-working-with-ambient-occlusion-thickness.html"
breadcrumb-title: ''
description: 了解為什麼 Matching by Name 無法與環境遮蔽和厚度烘焙器搭配，並尋找替代方案。
helpx_creative_field: ""
helpx_description: "bakers > Common Questions > Why is Matching by Name not working with Ambient OcclusionThickness "
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: '為什麼「以名字匹配」無法與環境遮蔽厚度（Ambient OcclusionThickness）相容 '
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '109'
ht-degree: 0%

---


# 為什麼「依名稱匹配」無法在環境遮蔽/厚度設定中運作？

>[!WARNING]
>
> **問題**
> 
> 我在常用參數[&#128279;](../../bakers-settings/common-parameters/common-parameters.md)中啟用了「按名稱[&#128279;](../../features/matching-by-name/matching-by-name.md)匹配」來篩選和排序低多邊形和高多邊形網格，為什麼環境遮蔽烘焙器會忽略它？

>[!NOTE]
>
> **說明**
> 
> 環境遮蔽、厚度和彎曲法線在計算貼圖時會發射次級光線。 這些光線有自己的「按名字配對」設定。

>[!NOTE]
>
> **解答：物質畫家**
> 
> 解決方案：在烘焙器參數中啟用次級光線的名稱匹配過濾。
