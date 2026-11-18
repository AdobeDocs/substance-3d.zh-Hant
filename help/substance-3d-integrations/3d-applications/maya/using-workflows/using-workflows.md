---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/maya/using-workflows.html"
breadcrumb-title: ""
description: 在 Maya 中為 Substance 輸出建立並使用渲染預設，以自動為不同渲染器產生著色器網路。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > Maya > Using Workflows
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 使用工作流程
user-guide-description: ""
user-guide-title: ""
source-git-commit: 28a9d8cf7a4eed4163f99e8158c9cb8f9da88302
workflow-type: tm+mt
source-wordcount: '568'
ht-degree: 0%
---

# 使用工作流程

在「工作流程」中，您可以選擇或建立 Substance 輸出的渲染預設。 這些預設是像 Arnold 或 Vray 這類渲染器的著色器網路。

>[!NOTE]
>
> **工作流程預設位置**
>
> **Windows**：
> C：\Users\\Documents\maya\2022\substance\workflows\generated
> **MacOS**：
> /使用者//資料庫/偏好設定/Autodesk/maya//substance/workflows/generated
> **Linux**：
> /home//maya//substance/workflows/generated

![](../../../assets/maya-max-v3-1/maya-all-presets.png)

若要使用工作流程，只需從清單中選擇預設值，然後點擊「建立網路」按鈕即可。

![](../../../assets/workflow.gif)

## 建立工作流程

您可以建立自己的工作流程並將其加入渲染器工作流程清單。 新增工作流程時，Substance 節點之後建立的任何節點都會儲存在工作流程中。 這讓你可以建立任意數量的著色節點，建立完整的自訂著色器網路，並可儲存為預設工作流程。

![](../../../assets/saved-workflow.png)

## 管理工作流程

### 儲存自訂工作流程

1. 手動建立 Substance 輸出，並將其連接到像 aiStandardSurface 這樣的材質。
   1. 你可以使用任何 Maya 或渲染特定節點來建立著色器網路。
1. 點選「 **建立工作流程** 」按鈕，並輸入工作流程預設的名稱。

### 複製工作流程

您可以點擊 **「複製工作流程** 」按鈕來複製工作流程。

### 重新命名與覆寫工作流程

您可以使用「重新命名&#x200B;**」與**「覆寫&#x200B;**所選」按鈕，重新命名現有工作流程，並用更新後**&#x200B;的資料覆蓋工作流程。

### 移除工作流程

您可以使用「移除工作流程」按鈕來移除現有的工作流程。

## OpenPBR 工作流程

Workflows 清單中有兩種 OpenPBR 工作流程： **OpenPBR** 和 **OpenPBR - V-Ray**。 這些工作流程專為使用 Substance 3D Designer 或 Sampler 中 OpenPBR 材質模型撰寫的 SBSAR 檔案而設計（OpenPBR 自 Designer V16.0+ 與 Sampler V6.0+ 起即為預設模型）。

### 什麼是 OpenPBR

OpenPBR 是一個由 Adobe 與 Autodesk 開發的開放、物理基礎材質著色模型，並對 Academy Software Foundation（ASWF）有所貢獻。 它提供統一的材質定義，且可在不同渲染器間相容。 欲了解更多資訊，請參閱 [OpenPBR 文件](https://experienceleague.adobe.com/en/docs/substance-3d/general-knowledge/openpbr/openpbr-overview)。

### 何時使用 OpenPBR 工作流程

當您的 SBSAR 檔案是使用 Substance 3D Designer 或 Substance 3D Sampler 中 OpenPBR 材質模型製作時，請使用 OpenPBR 工作流程。 如果您的 SBSAR 是使用 Adobe 標準材質模型（ASM）製作的，請使用與您的渲染器相容的舊有工作流程（Arnold、V-Ray 或 V-Ray 6）。

>[!NOTE]
>
> 如果您對 ASM 材料套用 OpenPBR 工作流程，或對 OpenPBR SBSAR 套用標準工作流程，外掛程式只會連接兩個材質模型共有的輸出。 結果可能不完整。

### 可用的 OpenPBR 工作流程

**OpenPBR**

使用原生 Maya openPBRSurface 節點。 與 Arnold 和 V-Ray 相容。 這是大多數在 Maya 中使用 OpenPBR 材質的使用者所建議的工作流程。

**OpenPBR - V-Ray**

在 OpenPBR 模式下使用 V-Ray 材質（VRayMtl）。 建議專為以 V-Ray 材質設定為核心的管線使用者使用。

### 如何套用 OpenPBR 工作流程

1. 使用「載入物質」按鈕將 SBSAR 檔案載入外掛程式。
1. 在工作流程清單中，選擇 **OpenPBR** 或 **OpenPBR - V-Ray**。
1. 點選&#x200B;**「建立網路**」以在 Hypershade 材質編輯器&#x200B;**中**&#x200B;建立著色器網路。
1. 外掛程式會自動將 SBSAR 輸出連接到 OpenPBR 節點的對應輸入端。
1. 像平常一樣將材質指派到你的網格上。

![](../../../assets/maya-max-v3-1/maya-openpbr-overview.png)
