---
helpx_url: "https://helpx.adobe.com/tw/substance-3d-bake/common-questions/should-i-enable-compute-tangent-space-per-fragment.html"
breadcrumb-title: ''
description: 了解何時啟用每個片段的切線空間計算，以及它如何影響你的烘焙結果。
helpx_creative_field: ""
helpx_description: bakers > Common Questions > Should I enable
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 我應該啟用嗎
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '172'
ht-degree: 0%

---


# 我應該啟用「計算每個片段的切線空間」嗎？

>[!WARNING]
>
> **問題**
> 
> 「計算每個片段的切線空間」這個設定是什麼意思？它的用途是什麼？

>[!NOTE]
>
> **說明**
> 
> 啟用此設定後，該設定會指示烘焙者在片段著色器（亦稱像素著色器）中執行切線空間計算，而非頂點著色器。 這表示計算將以像素為單位進行，而非從一個頂點插值到另一個頂點。 這些設定是法線貼圖烘焙器用來判斷如何編碼材質的。 它以前也會用著色器讀取貼圖。
> 
> 啟用或停用此參數通常需要重新烘焙貼圖，以與 3D 視口及渲染引擎（如 Iray）同步。

>[!NOTE]
>
> **解法**
> 
> 根據渲染材質的軟體或遊戲引擎，此設定可能會被停用或啟用：
> 
> | *軟體* | *計算每個片段的切空間* |
> | --- | --- |
> | **虛幻引擎4** | 啟用 |
> | **統一** | 失能 |
