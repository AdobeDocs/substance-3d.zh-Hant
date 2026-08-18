---
helpx_url: "https://helpx.adobe.com/tw/substance-3d-integrations/3d-applications/maya/settings.html"
breadcrumb-title: ''
description: 透過 Substance Shelf 或選單在 Maya 中設定 Substance 插件的設定，以自訂行為。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > Maya > Settings
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 設定
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 1%

---


# 設定

物質設定選單可以透過物質架或物質選單進入。 此選單的設定儲存在可編輯的設定檔「substance.cfg」中。

>[!NOTE]
>
> **設定檔位置**
> 
> **視窗**：\
> C：\使用者\\文件\maya\\內容\\
> **MacOS**：\
> /使用者//函式庫/偏好設定/Autodesk/maya//substance/\
> **Linux**：\
> /家//Maya//物質/

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

## 預設解析度

在載入 sbsar 檔案時，設定 Substance 節點的預設解析度。

## 渲染工作流程

設定 Substance 節點的預設渲染工作流程。

## 物質引擎

設定專屬於 Substance Engine 的偏好設定，並全域設定到所有 Substance 節點。 Substance 引擎用於計算 Substance 的貼圖。

### 引擎類型

Substance Engine 提供 CPU 與 GPU 兩種引擎版本。 切換引擎需要重新啟動 Maya。 GPU 引擎會比 CPU 引擎提供更高的解析度。

>[!WARNING]
>
> CPU 和 GPU 引擎之間可能有計算差異，因此為了穩定的結果，最好將類型設成 Substance Designer 中使用的同一個引擎。

CPU 核心與引擎記憶體是設定 Substance 引擎允許使用的資源量。

### 定型渲染

這個選項可以設定 Substance 引擎的運算是否會阻擋 Maya UI 的程序。 啟用後，Substance 引擎會優先並阻擋 Maya UI 的程序。 停用後，Maya UI 程序不會被 Substance 引擎的計算阻擋。

## 快取輸出至磁碟

設定專案中所有新建立 Substance 節點的預設快取位置、檔案類型及快取資料夾。

## 渲染擴充

啟用渲染擴充功能，讓 Substance 輸出直接搭配 Arnold 著色器使用。

## 實際大小

啟用是否預設在載入 SBSAR 檔案時使用實體大小，以及重新載入 SBSAR 時是否應該重新計算。

</td>
<td style="border: 0;" valign="top">

![](../../../assets/settings-35.png)

</td>
</tr>
</table>
