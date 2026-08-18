---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/modo/working-with-normals.html"
breadcrumb-title: ''
description: 在 MODO 中設定法線貼圖方向設定，以確保 Substance 材質的法線貼圖渲染正確。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > MODO > Working with Normals
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 與法線合作
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '151'
ht-degree: 0%

---


# 與法線合作

處理法線資料 - 設定正確方向

庫存物質是為了使用 DX 正常方向而設計的。 不過，MODO 使用 OGL。 你可以把法線格式參數設為 1.0 來反轉法線。 Substance 插件只會解讀 Substance 中設定的參數。 你可能會遇到沒有「normal\_format」參數的物質，因為由該物質的作者自行為自訂物質加上這個控制。 如果你遇到沒有這個參數的 Substance，你可以翻轉法線貼圖的 Texture Layer 上的綠色通道來固定方向。

>[!NOTE]
>
> 只有當 Substance 的法線方向錯誤，且作者沒有建立控制來在 Substance 參數中翻轉法線時，才會翻轉綠色通道

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

![](../../../assets/normal-1.png)

</td>
<td style="border: 0;" valign="top">

![](../../../assets/invert-2.png)

</td>
</tr>
</table>
