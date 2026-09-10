---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/common-issues/baking-failed-with-color-map-from-mesh.html"
breadcrumb-title: ''
description: 透過檢查網格色彩屬性和 UV 映射，解決網格烘焙失敗的色彩映射。
helpx_creative_field: ""
helpx_description: bakers > Common Issues > Baking failed with Color Map from Mesh
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 用 Mesh 的 Color Map 烘焙失敗
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '140'
ht-degree: 0%

---


# 用 Mesh 的 Color Map 烘焙失敗

>[!WARNING]
>
> **子嗣**
> 
> 可能的錯誤訊息：
> 
> &#x200B;> > > 
> 
> [ 烘焙中 ]烘焙失敗（來自 Mesh 的色彩映射）\
> 找不到頂點顏色

>[!NOTE]
>
> **說明**
> 
> 從網格[&#128279;](../../bakers-settings/color-map-from-mesh/color-map-from-mesh.md)的色彩貼圖預設設定是將高多邊形網格頂點顏色烘焙成基於網格 UV 的貼圖。然而，高多邊形網格通常沒有任何頂點顏色資訊。 因此，麵包師無法寫出不存在的資訊。

>[!NOTE]
>
> **解法**
> 
> 有不同的解決方案可避免此錯誤訊息：
> 
> * 使用帶有頂點顏色的高多邊形網格
> * 用不同設定從 Mesh Baker 設定色彩貼圖
> * 如果你不需要 Mesh baker 的色彩貼圖，就不要用它
