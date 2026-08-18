---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/features/tangent-space.html"
breadcrumb-title: ''
description: 學習 Substance Bakers 如何處理切線空間計算，並根據您的工作流程自訂演算法。
helpx_creative_field: ""
helpx_description: bakers > Features > Tangent Space
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 切空間
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '330'
ht-degree: 0%

---


# 切空間

Substance Baker 可以載入低多邊形網格上的切線和雙法線，或重新計算它們。 在重新計算時，可以定義一個自訂的切空間演算法（預設為 MikkTSpace）。

## 切線空間插件列表

## 物質畫家

在 Substance Painter 中，Tangent Space 外掛無法更改，永遠是 **MikkTSpace**。 不過有一個參數可以稍微調整其行為，使其與其他應用程式相容：

| *參數* | *相容**應用* |
| --- | --- |
| **計算每個片段的切空間：已停用** | 相容於 xNormal、Unity 5.3 或更新版本。 |
| **計算每個片段的切空間：啟用** | 相容於 Unreal Engine 4、Blender 及 Unity HDRP 工作流程。 |

## 物質設計師

Substance Designer 支援以下演算法：

| *檔案名稱* | *描述* |
| --- | --- |
| **mikktspace.dll** | MikkTSpace，基於Morten S. Mikkelsen研究的切線空間演算法。相容於 xNormal、Unity 5.3 或更新版本。 |
| **mikkunrealtspace.dll** | MikkTSpace，基於Morten S. Mikkelsen研究的切線空間演算法。相容於 Unreal Engine 4、Blender 及 Unity HDRP 工作流程。 |
| **unitytspace.dll** | 基於 Unity 4 的切空間演算法。 |

>[!NOTE]
>
> 可以寫自訂的切空間外掛。 一個名為 **tangentspaceplugin.h** 的標頭檔可在安裝資料夾的 **Substance Designer/SDK/tangentspace** 下取得，並可作為介面使用。

## 設定自訂切線空間

## 物質畫家

Substance Painter 目前不支援自訂的 Tangent Space 插件。 這表示如果低多邊形網格（用於創建專案）中沒有切線和雙法線，則會根據 MikkTSpace 演算法重新計算。

## 物質設計師

要在 Substance Designer 中設定切空間演算法，請遵循以下步驟：

1. 選擇 **編輯** > **偏好設定**。

   ![](../../assets/sd-edit-pref.png)
1. 點擊專案&#x200B;**&#x200B;**。

   ![](../../assets/sd-pref-projects.png)
1. 進入 **「一般** 」標籤。 往下滑直到看到 3D 場景&#x200B;**區**&#x200B;塊。

   ![](../../assets/sd-tab-general.png)
1. 點擊 **三個點** （...） 載入自訂插件。

## 物質自動化工具包

在使用 Automation Toolkit 烘焙時，可以指定 Tangent Space 外掛並指定特定的命令列參數：

```
sbsbaker normal-from-mesh --tangent-space-plugin "C:/Substance Designer/plugins⁄tangentspace⁄mikktspace.dll" ...
```
