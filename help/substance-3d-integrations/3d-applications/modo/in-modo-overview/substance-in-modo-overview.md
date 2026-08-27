---
helpx_url: "https://helpx.adobe.com/tw/substance-3d-integrations/3d-applications/modo/substance-in-modo-overview.html"
breadcrumb-title: ''
description: 了解 MODO 的 Substance 外掛，以及如何在工作流程中匯入和使用 Substance 材質。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > MODO > Substance in MODO Overview
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: MODO 中的物質概述
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '240'
ht-degree: 5%

---


# MODO 中的物質概述

## 概述：

## 打開物質

1. 建立一個素材或選擇一個素材群組。
1. 在材質>Substance中，選擇建立Substance，或使用Substance Kit選項下的Create 按鈕。 這會在著色器樹中建立一個物質材質。
1. 點擊 Load sbsar 來載入 sbsar 檔案。

   ![](../../../assets/load-1.png)

## 產生輸出

使用 **Default - Principled Shading 模式**，你可以用金屬/粗糙度工作流程來建立輸出。

1. 在物質屬性的輸出區塊，點選陰影所需的輸出。 Substance 貼圖會被生成，並以正確的材質層效果加入著色樹。 原則陰影模式需要以下資料：

   | 物質輸出 | 色彩空間 | 材質層效應（原則著色模式） |
   | --- | --- | --- |
   | 基本顏色 | sRGB | 擴散顏色 |
   | 正常 | 線性 | 正常 |
   | 粗糙度 | 線性 | 粗糙度 |
   | 金屬 | 線性 | 金屬 |

   ![](../../../assets/outputs-3.png)

## 解析度/參數變更

你可以更改Substance參數來更新或更改產生的材質。 更改參數會讓 Substance Engine 重新計算輸入 MODO 材質的貼圖。

1. 到物質材質的物質屬性，在調整區塊中更改任何參數。

   ![](../../../assets/params.png)
1. 你可以透過輸出大小下拉選單調整產生材質的解析度。 物質可設定產生最高8K。 [8K 輸出需要 Substance GPU 引擎](../../../3d-applications/modo/modo-switch-engine/modo-switch-engine.md)。
