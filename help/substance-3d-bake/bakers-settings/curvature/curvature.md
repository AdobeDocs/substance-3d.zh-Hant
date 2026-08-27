---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/bakers-settings/curvature.html"
breadcrumb-title: ''
description: 從網格中提取曲率資訊，製作能凸顯幾何體空洞和邊緣的貼圖。
helpx_creative_field: ""
helpx_description: bakers > Bakers Settings > Curvature
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 曲率
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '150'
ht-degree: 0%

---


# 曲率

曲率烘焙器可提取曲面紋理。 此材質包含與幾何體相關的空腔與邊緣資訊。

紋理屬性定義為：

* 黑色值代表凹面區域。
* 白色值代表凸面。
* 灰色值代表中性區域（主要是平面）。

**可於以下媒體取得：**

* 物質設計師
* 物質自動化工具包
* 物質畫家

## 參數

| *參數* | *描述* |
| --- | --- |
| **演算法** | 定義了如何在網格上計算曲率資訊。 |
| **詳情** | 控制曲率中資訊的強度。 高分數能產生更多細節，但不那麼細膩。 |
| **啟用接縫** | 如果啟用，烘焙者會嘗試透過將邊界的紋素從一側複製到另一側，來減少 UV 島之間的接縫。 |
| **縫隙**&#x200B;**強度** | 如果 **啟用了 Enable Seams** ，這個參數會控制縫線固定的強度。 |
