---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/maya/using-workflows.html"
breadcrumb-title: ''
description: 在 Maya 中為 Substance 輸出建立並使用渲染預設，自動為不同渲染器生成著色器網路。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > Maya > Using Workflows
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 工作流程的使用
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '250'
ht-degree: 0%

---


# 工作流程的使用

在工作流程中，你可以選擇或建立 Substance 輸出的渲染預設。 這些預設是為 Arnold 或 Vray 這類渲染器設計的著色器網路。

>[!NOTE]
>
> **工作流程預設位置**
> 
> **視窗**：\
> C：\Users\\\Documents\maya\2022\substance\workflows\generated\
> **MacOS**：\
> /使用者//函式庫/偏好設定/Autodesk/maya//substance/工作流程/生成\
> **Linux**：\
> /首頁//maya//substance/工作流程/生成

![](../../../assets/workflows-4.png)

要使用工作流程，只要從下拉選單選擇預設，然後點擊建立著色器網路按鈕即可。

![](../../../assets/workflow.gif)

## 建立工作流程

你可以建立自己的工作流程，並加入渲染器工作流程清單。 新增工作流程時，Substance 節點之後建立的任何節點都會被保存在工作流程中。 這讓你可以建立任意數量的著色節點，建立完整的自訂著色器網路，並可儲存為預設工作流程。

## ![](../../../assets/saved-workflow.png) 管理工作流程

### 儲存自訂工作流程

1. 手動建立 Substance 輸出，並將它們連接到像 aiStandardSurface 這類材質。
   1. 你可以用任何 Maya 或渲染特定節點來建立著色器網路。
1. 點選「 **建立工作流程** 」按鈕，輸入工作流程預設的名稱。

### 複製工作流程

你可以點擊 **「複製工作流程** 」按鈕來複製工作流程。

### 重新命名與覆寫工作流程

你可以透過 **「重新命名** 與 **覆寫** 選取」按鈕，重新命名現有工作流程，或用更新資料覆蓋工作流程。

### 移除工作流程

你可以透過「移除工作流程」按鈕來移除現有工作流程。
