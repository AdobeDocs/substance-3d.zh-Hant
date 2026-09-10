---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unity/optimization-guidelines.html"
breadcrumb-title: ''
description: 遵循優化指引，在 Unity 中平衡 Substance 材質的複雜度與渲染效能。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Optimization Guidelines
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 優化指引
user-guide-description: ''
user-guide-title: ''
source-git-commit: 4a060ee1aaa1731c04e70d5512e3271cd63d0381
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 0%

---


# 優化指引

你的物質材質越複雜，渲染所需的運算能力就越大。 因此 **，物質材料必須在複雜度與渲染速度**&#x200B;之間取得平衡。 這點對於&#x200B;*用於即時圖形應用（如遊戲）尤其*&#x200B;重要。

在建立自訂物質素材時，務必查看以下優化指引。

[Substance Designer 優化指引](https://docs.substance3d.com/display/SDDOC/Performance+Optimization+Guidelines)

一個主要的注意事項是絕對解析度達 4K 或以上的節點。

>[!WARNING]
>
> **請仔細注意解析度和親屬解析度設定！**\
> 高數值會嚴重影響效能，因此請考慮材料可能的使用方式，以及是否能減少資料量。
>   
> Substance CPU 引擎能以 4K 計算，但速度非常慢，可能導致整合卡頓或當機。

在以下範例中， [圖塊取樣器](https://experienceleague.adobe.com/en/docs/substance-3d-designer/using/substance-graphs/nodes-reference-for-substance-graphs/node-library/texture-generators/patterns/tile-sampler) 節點的輸出大小設定為 [絕對](https://experienceleague.adobe.com/en/docs/substance-3d-designer/using/substance-graphs/output-size) 4096。 它會讓下游多個節點以 4K 計算，然後再降頻以達到最終的 2048 輸出解析度。

![](../../../assets/absolute.png){width="1000px"}
