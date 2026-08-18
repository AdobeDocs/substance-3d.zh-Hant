---
helpx_url: "https://helpx.adobe.com/tw/substance-3d-bake/guides/triangulating-before-baking.html"
breadcrumb-title: ''
description: 了解網格三角測量如何影響烘焙結果，並學習準備幾何體的最佳實務。
helpx_creative_field: ""
helpx_description: bakers > Guides > Triangulating before baking
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 烘焙前的三角定位
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '266'
ht-degree: 0%

---


# 烘焙前的三角定位

3D 網格可以用多邊形定義，每個面有多個邊界邊。 通常是四邊形（4 條邊），有時更多（n 邊形）。\
不過軟體後期會把這些多邊形轉換成三角形，因為這樣比較容易管理和執行運算（尤其是在 GPU 上）。

## 三角剖分如何影響網格？

![](../../assets/triangulation.jpg)

目前沒有 **標準的解決方案** 能將四邊形/N邊形轉換成三角形。 如上圖所示，多重選擇是有效的。\
烘焙者不太可能像遊戲引擎那樣三角化網格，因為我們會選擇特定的演算法。

## 為什麼要先三角定位再烘焙？

烘焙過程會讀取幾何體，然後將資訊編碼到貼圖中。\
因為這些資訊是基於 UV，有時也基於網格拓撲，其他軟體如果不像套用貼圖時那樣讀取幾何體，可能會錯誤解碼這些資訊。

在下方的圖片中，你可以看到左上角的低多邊形網格和右上角的高多邊形網格。\
底部是低多邊形，法線貼圖是從高多邊形烘焙而來。 左側的網格使用與 Substance Painter 烘焙時相同的三角剖分。 右邊的網格沒有，顯示黑色的瑕疵。 這是因為法線貼圖的烘焙方式和網格目前的三角定位方式不符。 這可以透過更新網格和/或重新烘焙&#x200B;**來解決**。

![](../../assets/example-triangulation-artifact.jpg)
