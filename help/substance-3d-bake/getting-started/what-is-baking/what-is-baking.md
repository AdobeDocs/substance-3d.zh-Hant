---
helpx_url: 'https://helpx.adobe.com/substance-3d-bake/getting-started/what-is-baking.html'
breadcrumb-title: ''
description: 了解什麼是烘焙，並學習如何將 3D 網格資訊儲存到材質檔案中，以強化你的 Substance 材質。
helpx_creative_field: ''
helpx_description: 'bakers > Getting Started > What is Baking '
helpx_experience_level: ''
helpx_learn_topic: ''
helpx_tags: ''
title: '什麼是烘焙 '
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0a948aa65b787c0f84e0af681dbe74021e878687
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 0%

---


# 什麼是烘焙？

![](https://upload.wikimedia.org/wikipedia/commons/3/36/Normal_map_example.png)

（鳴謝： [ 保羅·奇尼奧尼](https://commons.wikimedia.org/wiki/File:Normal_map_example.png) - [CC BY-SA 1.0](https://creativecommons.org/licenses/by-sa/1.0)）

烘焙是指將&#x200B;**與** 3D 網格&#x200B;**相關的資訊**&#x200B;儲存到&#x200B;**貼圖**&#x200B;檔案（[位圖](https://en.wikipedia.org/wiki/Raster_graphics)）中的過程名稱。大多數時候，這個過程會涉及另一個網格。 此時，第一個網格的資訊會轉移到第二個網格的 UV，然後儲存成貼圖。

雖然有些應用程式可能支援將資訊烘焙到網格屬性中（例如頂點顏色），但 Substance Baker 只允許將資訊烘焙成貼圖。 不過他們可以讀取網格屬性並將其烘焙成貼圖（像是頂點顏色）。

## 烘焙是必要的嗎？

Substance 軟體會產生貼圖，這些貼圖可以透過利用與網格幾何體相關的資訊來增強。\
許多濾鏡和材質可以透過觀察烘焙的貼圖來適應 3D 網格的特定幾何形狀。 烘焙可以提供環境陰影的位置、幾何形狀的邊緣位置等資訊。

舉例來說：一輛老車底部可能因為一段時間沒動而生鏽。 烘焙位置圖可以讓你知道網格底部的位置，進而供應 Rust 產生器並產生適配的貼圖。

![](../../assets/examples.jpg){width="500px"}

## 烘焙是怎麼運作的？

每位烘焙師會執行特定動作以產生自己的結果，但一般烘焙過程包含兩種可能的方法：

* **烘焙到一個網格** 上 ：依賴當前網格來產生資訊。
* **從一個網格烘焙到另一個** 網格：從一個來源網格計算資訊，並將結果轉移到另一個網格。

這個烘焙過程依賴於網格的特性，因此網格必須乾淨且幾何形狀中沒有可能的缺陷。

## 你可以烘焙什麼樣的資訊？

許多類型的資訊都可以被烘焙成。 不過一般來說只需要特定集合，因為這些集合可以被推演以產生更進階的結果。 這也是為什麼有多種常見的烘焙流程，可以在多種軟體中找到。

舉例來說，Substance 軟體可以輸出以下類型的資訊：

* **環境遮蔽** （環境陰影）
* **法線** 資訊（曲面細節、變化以向量方向儲存）
* **方向** （哪裡是上或下，左還是右等等）
* **曲率** （幾何形狀的邊與腔）
* **位置** （幾何體在正規化立方體內的相對位置）

詳情請參閱 [每位烘焙師](../../bakers-settings/bakers-settings.md) 的文件。

## 「一般」與「網狀」烘焙師的差異

根據製程不同，烘焙師會使用不同的實作方式。 一般來說， **來自網格** 的模型烘焙者會依賴光線追蹤技術來從一個模型擷取並投影到另一個模型的資料。
