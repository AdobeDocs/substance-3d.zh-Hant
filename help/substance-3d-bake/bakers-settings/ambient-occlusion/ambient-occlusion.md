---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/bakers-settings/ambient-occlusion.html"
breadcrumb-title: ''
description: 學習如何使用環境遮蔽烘焙器，利用快速的 GPU 加速演算法生成環境陰影紋理。
helpx_creative_field: ""
helpx_description: bakers > Bakers Settings > Ambient Occlusion
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 環境遮擋
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 2%

---


# 環境遮擋

環境遮蔽烘焙器則允許烘焙環境陰影紋理。 這個烘焙器使用一個在 GPU 上執行的快速演算法。

**提供：**

* 物質設計師
* 物質自動化工具包

>[!WARNING]
>
> * 這個烘焙器可能不支援舊 GPU 使用。
> * 在低階或行動顯卡上以高解析度烘焙可能會導致當機。

## 參數

| *名稱* | *描述* |
| --- | --- |
| **法線貼圖** | 輸入法線貼圖檔案，可用於提供網格表面的額外幾何細節，供烘焙計算時考慮。 此參數為可選。 |
| **世界空間** | 若啟用，請指定輸入法線貼圖位於世界空間（World Space），而非切線空間。 若未提供輸入法線貼圖，則忽略或停用此參數。 |
| **逆轉正常** | 計算環境遮蔽圖，使用反法線（可用來產生厚度圖）。 |
| **使用未選取的網格零件** | 使用未選取的網格部分來烘焙環境遮蔽貼圖。 |
| **品質** | 選擇環境遮蔽地圖的品質。 品質越高，計算越慢。可用數值：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>低（</strong> 3次傳球）</li><li data-preserve-html="true"><strong>中等難度</strong> （預設，5 次傳球）</li><li data-preserve-html="true"><strong>高（</strong> 10 次通過）</li><li data-preserve-html="true"><strong>非常高</strong> （16 次通過）</li></ul> |
| **精密偏壓** | 環境遮蔽的精確度。 較低的數值會帶來更高的精度，但可能會產生更大的偽影。 |
| **距離漸遠** | 環境遮蔽的擴散。 |
