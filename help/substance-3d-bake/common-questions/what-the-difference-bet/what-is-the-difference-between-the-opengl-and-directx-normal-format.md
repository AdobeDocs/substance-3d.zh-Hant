---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/common-questions/what-is-the-difference-between-the-opengl-and-directx-normal-format.html"
breadcrumb-title: ''
description: 了解 OpenGL 和 DirectX 法線貼圖格式的差異，以及何時使用。
helpx_creative_field: ""
helpx_description: "bakers > Common Questions > What is the difference between the OpenGL and DirectX normal format "
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 'OpenGL 和 DirectX 一般格式有什麼不同 '
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '185'
ht-degree: 0%

---


# OpenGL 和 DirectX 一般格式有什麼差別？

>[!WARNING]
>
> **問題**
> 
> OpenGL 和 DirectX 一般格式有什麼差別？

>[!NOTE]
>
> **說明**
> 
> OpenGL 和 DirectX 是兩個圖形 API（函式集合），程式設計師在應用程式中使用它們與 GPU（圖形處理單元）對話。 就法線貼圖而言，差異決定了RGB材質中綠色通道的解讀方式。 OpenGL 預期第一個像素會在底部，而 DirectX 則期望它在頂部。 這也是為什麼在各種技術討論中，建議嘗試反轉法線貼圖的綠色通道，看看它在像素值反轉（從先變成最後）時是否表現更好。 OpenGL 可稱為 **Y+** （自下而上），而 DirectX 則稱為 **Y-** （自上而下）。
> 
> 要知道該用哪種格式，請參考你的貼圖將被使用的目標應用程式。
