---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/common-questions/texture-baked-outside-of-substance-software-looks-incorrect.html"
breadcrumb-title: ''
description: 排除為什麼 Substance 軟體外烘焙的貼圖看起來不正確，並學習如何修復色彩空間問題。
helpx_creative_field: ""
helpx_description: bakers > Common Questions > Texture baked outside of Substance software looks incorrect
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Substance 軟體外烘焙的貼圖看起來不對
user-guide-description: ''
user-guide-title: ''
source-git-commit: 4a060ee1aaa1731c04e70d5512e3271cd63d0381
workflow-type: tm+mt
source-wordcount: '169'
ht-degree: 0%

---


# Substance 軟體外烘焙的貼圖看起來不對

>[!WARNING]
>
> **問題**
> 
> 為什麼我用外部塗抹而非 Substance Bakers 烘焙的紋理在 Substance Painter 中看起來不正確？

>[!NOTE]
>
> **解法**
> 
> 此問題目前尚無立即解決方案，因為多種因素可能造成：
> 
> * 確認 Substance 軟體與外部應用程式之間的正常格式是否相同。 OpenGL 是 [X+， Y+， Z+]，DirectX 是 [X+， Y-， Z+]
>   * 在 Substance Painter 中，可以在專案設定[&#128279;](https://experienceleague.adobe.com/en/docs/substance-3d-painter/using/interface/project-configuration)中更改正常格式。
>   * 在 Substance Designer 中，可以在專案偏好設定[&#128279;](https://experienceleague.adobe.com/en/docs/substance-3d-designer/using/workspace/preferences/project-settings)中更改一般格式。
> * 在烘焙並匯入 Substance 軟體前，請確認網格是否已被三角定位。 更多資訊請參見 [此頁面](../../guides/triangulating-before-bak/triangulating-before-baking.md) 。
