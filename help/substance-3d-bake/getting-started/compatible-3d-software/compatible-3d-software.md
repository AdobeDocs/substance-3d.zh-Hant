---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/getting-started/compatible-3d-software.html"
breadcrumb-title: ''
description: 了解哪些 3D 軟體與 Substance Bakers 相容，並學習如何準備網格以達到最佳烘焙效果。
helpx_creative_field: ""
helpx_description: bakers > Getting Started > Compatible 3D software
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 相容的 3D 軟體
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 1%

---


# 相容的 3D 軟體

大多數 3D 軟體都能與 Substance Baker 相容，只要它們能以應用程式支援的多邊形格式匯出網格幾何。

不過，並非所有軟體在匯出這些網格時，在功能和品質上都達到同等水準。 這就是為什麼正確清潔網格並確保它能與烘焙師相容非常重要。 想了解更多如何準備網格的資訊，請參閱各種 [指南](../../guides/performances-and-opt/performances-and-optimizations.md)。

## 軟體相容性

以下是一些常見的3D軟體及其與烘焙師的相容性清單：

| *名稱* | *現況* |
| --- | --- |
| **攪拌機** | 相容性：匯出前需要先將修飾符壓平。 |
| **瑪雅** | 相容：匯出前需要凍結、變換並刪除歷史紀錄。 |
| **3DS Max** | 相容性：匯出前需重置 xForm。 |
| **MODO** | 相容：建議使用 Game Tab 匯出器設定為「Unreal Static Mesh」。 |
| **Cinema 4D** | 相容性：匯出前需要先將修飾符壓平。 |
| **zBrush** | 不相容：低多邊形網格需要先在其他 3D 應用程式中處理和清理。 相容：烘焙用的高多邊形網格。 |

## 檔案格式

烘焙幾何時，也要考慮所使用的檔案格式。 檔案格式會定義網格中將儲存的資訊量。

資訊過多有時會造成傷害，導致錯誤。 我們通常建議在錯誤發生時嘗試不同的檔案格式，因為這能輕鬆排除問題，判斷問題出在烘焙機本身還是來自 3D 軟體。

Bellow 簡要介紹了烘焙師們最常支援的兩種檔案格式：

| 檔案格式 | 資訊 |
| --- | --- |
| **FBX** | Autodesk FBX（Filmbox）是 Autodesk Software 主要使用的檔案格式，可以文字或二進位格式撰寫。  它支援：<ul data-preserve-html="true"><li data-preserve-html="true">UV（多重集合）</li><li data-preserve-html="true">頂點、切線與雙正規性</li><li data-preserve-html="true">頂點顏色</li><li data-preserve-html="true">三角形面、四面和N-Gon面</li><li data-preserve-html="true">攝影機</li><li data-preserve-html="true">光源</li><li data-preserve-html="true">網狀細分</li><li data-preserve-html="true">平滑群</li><li data-preserve-html="true">材質資訊（例如顏色）</li><li data-preserve-html="true">位圖</li></ul> |
| **OBJ** | Wavefront OBJ 是一種非常簡單的文字檔案格式，支援：<ul data-preserve-html="true"><li data-preserve-html="true">UV（僅一組）</li><li data-preserve-html="true">頂點法線</li><li data-preserve-html="true">頂點顏色（僅限從 Pixologic zBrush 匯出時）</li><li data-preserve-html="true">三角形面、四面和N-剛面</li><li data-preserve-html="true">材質顏色（如果 <strong>有 mtl</strong> 檔案）</li></ul> |
