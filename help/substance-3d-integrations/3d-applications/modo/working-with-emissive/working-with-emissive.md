---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/modo/working-with-emissive.html"
breadcrumb-title: ''
description: 在 MODO 中設定物質材質的發射屬性，以控制光度量與色彩設定。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > MODO > Working with Emissive
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 與 Emissive 合作
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '201'
ht-degree: 0%

---


# 與 Emissive 合作

## 使用發射體（亮度量與顏色）

物質可以有可選的發射輸出。 你可以在 MODO 裡用這個來做亮度量和顏色。 當你啟用發射輸出時，它會被設定為亮度量效果。 預設情況下，此通道在貼圖影像靜止標籤下被解讀為線性。\
在著色器樹中右鍵點擊材質，選擇複製。 接著，將複製的發射紋理設為 Luminous Color 效果。 接著你可以調整紋理的高低值，驅動亮度效果，進一步強化這個數值。

>[!NOTE]
>
> 對於設定為 Luminous Color 的貼圖，你需要在 Image Still 標籤中將解讀設定為 sRGB。

要取得泛光效果，你需要在渲染面板啟用泛光，並設定閾值和半徑。

![](../../../assets/bloom.png)

對於 Unreal 和 Unity 材質，發射輸出是專門由材質處理的。\
Unreal = Unreal 發射\
單位 = 單位 輸出

Unreal Emissive 和 Unity Emission 的貼圖需要在影像靜態標籤中從 Linear 改成 sRGB。
