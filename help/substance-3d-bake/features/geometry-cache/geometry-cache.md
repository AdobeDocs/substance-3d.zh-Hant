---
helpx_url: "https://helpx.adobe.com/tw/substance-3d-bake/features/geometry-cache.html"
breadcrumb-title: ''
description: 使用幾何快取來保存預處理的網格資料，並大幅加快後續烘焙作業。
helpx_creative_field: ""
helpx_description: bakers > Features > Geometry Cache
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 幾何快取
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '148'
ht-degree: 0%

---


# 幾何快取

烘焙時，網格會先經過預處理以清理乾淨，並轉換成與烘焙過程相容的格式。 幾何快取是一種能快速重新載入這些預處理幾何體的方法，避免日後重做此操作（除非來源網格改變）。

* 在 Substance Designer **中**，幾何快取會在執行第一次烘焙後建立。快取會被保存在記憶體中，直到 baker 視窗關閉。
* 在 Substance Painter **中**，幾何快取會在第一次烘焙後，將檔案儲存為副檔名 **assbin** 的檔案。

重複使用幾何快取能大幅加快烘焙過程，尤其是在調整烘焙設定以達到完美效果時。
