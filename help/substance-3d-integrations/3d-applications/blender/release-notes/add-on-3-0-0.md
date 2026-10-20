---
title: Blender 附加元件 3.0.0+
description: Substance 3D Blender 插件的發行說明列表。
source-git-commit: 1488c476be7921c113d2a54f870fee090e6295e9
workflow-type: tm+mt
source-wordcount: '211'
ht-degree: 0%
---

# 附加元件 3.0.0+

**附加元件 3.1.0**。*發布日期：2026 年 10 月 20 日*

**Blender 附加元件：**

* &amp;lbrack;Bug&amp;rbrack;修正函式庫路徑無法運作
* &amp;lbrack;Bug&amp;rbrack;修正多執行緒中的上下文問題，導致 SBSAR 無法載入/更新
* &amp;lbrack;Bug&amp;rbrack;固定材質匯出格式被忽略
* &amp;lbrack;性能&amp;rbrack;多項性能改進

**Substance 整合工具（Substance Remote Engine）：**

* &amp;lbrack;Feature&amp;rbrack;已更新至 Substance Engine 9.6.1
* &amp;lbrack;Performance&amp;rbrack;更新相依關係及多項效能改進

**附加元件 3.0.1**。*發布日期：2026 年 2 月*

**Blender 附加元件：**

* &amp;lbrack;固定&amp;rbrack;參數最小/最大值無法運作
* &amp;lbrack;固定&amp;rbrack;實體尺寸無法與自訂場景縮放相符
* &amp;lbrack;固定&amp;rbrack;物理尺寸無法與非公制單位相容
* &amp;lbrack;Fixed&amp;rbrack;透明塗層地圖無法在 Blender 4+ 上運作
* &amp;lbrack;Fixed&amp;rbrack;著色器中缺少透明塗層色彩貼圖
* &amp;lbrack;固定&amp;rbrack;附加元件定義中標籤錯誤
* &amp;lbrack;Fixed&amp;rbrack;Substance 會隨機當機 SRE（帶有顏色 float4 值）
* &amp;lbrack;固定&amp;rbrack;影像輸入未顯示於參數列表中
* &amp;lbrack;固定&amp;lbrack;關閉再重開 blender 後影像輸入無法運作

**Substance 整合工具（Substance Remote Engine）：**

* 升級至 3.0.1 版本
* 移除 C++11 ABI 以支持新的 Linux 編譯
