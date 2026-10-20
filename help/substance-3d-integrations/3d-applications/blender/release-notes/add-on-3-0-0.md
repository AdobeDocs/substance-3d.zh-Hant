---
title: Blender 附加元件 3.0.0+
description: Substance 3D Blender 插件的發行說明列表。
source-git-commit: aa5acd016cd1a55ab230d36352c4d3aa5514012a
workflow-type: tm+mt
source-wordcount: '211'
ht-degree: 0%
---

# 附加元件 3.0.0+

**附加元件 3.1.0**。*發布日期：2026 年 10 月 12 日*

**Blender 附加元件：**

* &lbrack;Bug&rbrack;修正函式庫路徑無法運作
* &lbrack;Bug&rbrack;修正多執行緒中的上下文問題，導致 SBSAR 無法載入/更新
* &lbrack;Bug&rbrack;固定材質匯出格式被忽略
* &lbrack;性能&rbrack;多項性能改進

**Substance 整合工具（Substance Remote Engine）：**

* &lbrack;Feature&rbrack;已更新至 Substance Engine 9.6.1
* &lbrack;Performance&rbrack;更新相依關係及多項效能改進

**附加元件 3.0.1**。*發布日期：2026 年 2 月*

**Blender 附加元件：**

* &lbrack;固定&rbrack;參數最小/最大值無法運作
* &lbrack;固定&rbrack;實體尺寸無法與自訂場景縮放相符
* &lbrack;固定&rbrack;物理尺寸無法與非公制單位相容
* &lbrack;Fixed&rbrack;透明塗層地圖無法在 Blender 4+ 上運作
* &lbrack;Fixed&rbrack;著色器中缺少透明塗層色彩貼圖
* &lbrack;固定&rbrack;附加元件定義中標籤錯誤
* &lbrack;Fixed&rbrack;Substance 會隨機當機 SRE（帶有顏色 float4 值）
* &lbrack;固定&rbrack;影像輸入未顯示於參數列表中
* &lbrack;固定&lbrack;關閉再重開 blender 後影像輸入無法運作

**Substance 整合工具（Substance Remote Engine）：**

* 升級至 3.0.1 版本
* 移除 C++11 ABI 以支持新的 Linux 編譯