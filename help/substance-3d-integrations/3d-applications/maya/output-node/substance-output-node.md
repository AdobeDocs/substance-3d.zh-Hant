---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/maya/substance-output-node.html"
breadcrumb-title: ''
description: 了解 Substance 輸出節點在 Maya 中如何運作，將計算出來的貼圖連接到著色器網路。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > Maya > Substance Output Node
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 物質輸出節點
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '137'
ht-degree: 0%

---


# 物質輸出節點

Substance 輸出節點是對 Substance 引擎計算出的貼圖的參考。 它連接到物質節點。 當 Substance 節點產生輸出時，Substance 引擎會計算紋理，並將此資料儲存為 RAM。 若使用 GPU 引擎，資料會在 GPU 上計算，並透過 Substance GPU Blend 引擎回傳記憶體。 物質節點未被啟動的輸出不會被計算。

![](../../../assets/outputnode.png)

在這個節點上，你可以在 Substance Designer 的輸出中看到輸出資訊，例如識別碼、標籤和使用量設定。 這個節點也允許你在輸出快取區段烘焙貼圖到磁碟。
