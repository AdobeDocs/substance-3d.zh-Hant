---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/bakers-settings/transferred-texture-from-mesh.html"
breadcrumb-title: ''
description: 根據 UV 在網格間傳輸貼圖，包括支援法線貼圖轉換。
helpx_creative_field: ""
helpx_description: bakers > Bakers Settings > Transferred Texture from Mesh
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 從網格轉移貼圖
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '238'
ht-degree: 0%

---


# 從網格轉移貼圖

從 mesh baker 轉過來的材質允許將材質從一個網格轉換到另一個，根據它們各自的 UV。 此烘焙器同時支援傳輸或法線貼圖（需特殊轉換）。 要運作，兩個網格都需要 UV 定義。

**可於以下媒體取得：**

* 物質設計師
* 物質自動化工具包

## 參數

| *參數* | *描述* |
| --- | --- |
| **貼圖檔案** | 將要傳輸的輸入貼圖檔案路徑。 |
| **UV 集合** | 用在高多邊形網格上的網格 UV，讀取貼圖並將其投影到低多邊形網格上。 |
| **過濾模式** | 定義了貼圖像素插值應該如何進行。可能的數值：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>最近</strong>：無插值，使用與指定位置最近的像素。 雖然精準，但可能會產生鋸齒。</li><li data-preserve-html="true"><strong>雙線性</strong> （預設）：使用與指定位置最近的四個像素。 沒有鋸齒，但可能會模糊。</li></ul> |
| **法線貼圖** | 如果啟用，會指示烘焙師要轉移的輸入貼圖是法線貼圖。 這表示烘焙者要對貼圖進行特殊轉換，使其與目標網格相容。 |
| **地圖類型** | 定義輸入貼圖的法線貼圖類型。可能的數值：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>世界空間</strong></li><li data-preserve-html="true"><strong>切空間</strong> （預設）</li></ul> |
| **正常方向** | 若 **Map Type** 設為 **切線空間**，則定義輸入貼圖的法線格式。可能的值：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>OpenGL</strong></li><li data-preserve-html="true"><strong>DirectX</strong> （預設）</li></ul> |
