---
helpx_url: "https://helpx.adobe.com/tw/substance-3d-bake/bakers-settings/world-space-direction.html"
breadcrumb-title: ''
description: 計算世界空間中的向量方向，並將其儲存成材質以進行方向效果和遮罩。
helpx_creative_field: ""
helpx_description: bakers > Bakers Settings > World Space Direction
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 世界太空方向
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '155'
ht-degree: 0%

---


# 世界太空方向

世界空間方向烘焙器允許將世界空間中的向量方向計算成貼圖。

**可於以下媒體取得：**

* 物質設計師
* 物質自動化工具包

## 參數

| *參數* | *描述* |
| --- | --- |
| **輸入方向** | 定義了計算方向的輸入來源。可能的數值：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>從 Texture</strong> 開始：向量方向是由輸入材質定義的。</li><li data-preserve-html="true"><strong>根據 Uniform Vector</strong> （預設）：向量方向由 X、Y、Z 滑桿定義。</li></ul> |
| **正常方向** | 定義輸出貼圖的正常格式。 這會根據格式將綠色通道反轉。可能的數值：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>OpenGL</strong></li><li data-preserve-html="true"><strong>DirectX</strong> （預設）</li></ul> |
| **X Y Z** | 如果 **輸入方向** 設為 **從均勻向量**，則用滑桿來定義方向向量的三個分量。 |
| **方向檔案** | 如果輸入方向設為&#x200B;**「From Texture**」，則 Path 到 Input 貼圖檔來定義方向向量&#x200B;**&#x200B;**。 |
