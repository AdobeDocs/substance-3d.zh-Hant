---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/common-issues/black-shading-cross-are-visible-on-the-mesh-surface.html"
breadcrumb-title: ''
description: 透過修正切線空間和法線計算，修正網格表面上可見的黑色著色瑕疵。
helpx_creative_field: ""
helpx_description: bakers > Common Issues > Black shading cross are visible on the mesh surface
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 黑色陰影十字架可見於網格表面
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '174'
ht-degree: 0%

---


# 網格表面上可見黑色陰影十字

在光照下，網格多個區域會出現黑色陰影偽影。

![](../../assets/black-shading-cross.jpg)


## 說明

黑色陰影叉通常表示法線貼圖與網格不符，通常是因為網格幾何形狀改變或以與烘焙者計算的方式不同。 舉例來說：網格的三角剖分在烘焙器和渲染網格及其法線貼圖的視窗之間是不同的。

## 解法

確保顯示網格和法線貼圖的應用程式與材質烘焙方式同步。 這意味著：

* 確認觀察者與烘焙者之間的切線空間是否相同。
* 確認視圖與烘焙者之間的標準格式是否相同。
* 確認觀看者與烘焙師之間的三角定位是否一致。 更多資訊請參見[此頁面](../../guides/triangulating-before-bak/triangulating-before-baking.md)。
