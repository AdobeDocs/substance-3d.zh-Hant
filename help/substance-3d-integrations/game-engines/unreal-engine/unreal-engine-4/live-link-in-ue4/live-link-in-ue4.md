---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-4/live-link-in-ue4.html"
breadcrumb-title: ''
description: 在 Unreal Engine 4 使用 Live Link，可以即時同步 Painter 和 UE4 之間的 Substance 材質。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 4 > Live Link in UE4
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: UE4 中的 Live Link（即時連結）
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '289'
ht-degree: 0%

---


# UE4 中的 Live Link（即時連結）

>[!WARNING]
>
> Unreal Engine 中的 Live Link 已不再支援。 使用舊版外掛且使用Live Link的使用者仍可使用此功能。

>[!WARNING]
>
> Live Link 無法支援 UE4 BSP 網格。 你寄出的資產必須是匯入到 UE4 專案的模型檔案

## 建立與 Substance Painter 的連結

1. 開放實質畫家
1. 在內容瀏覽器中右鍵點擊你想寄給 Painter 的資產，然後選擇「送給 Painter」。

   ![](../../../../assets/link1-22.png){width="400px"}
1. 網格會出現在 Substance Painter 裡，你可以開始貼圖。 隨著你工作，貼圖會被送到 UE4 並套用到材質上。 工具列中 UE4 圖示上的綠點表示連結已上線並傳送材質。

   ![](../../../../assets/icon-12.png)

   1. 你可以在外掛的設定選項中暫停資料串流。 到插件>dcc-live-link，選擇配置。 關閉啟用串流以暫停資料傳送到 UE4。

      ![](https://helpx-prod.scene7.com/is/image/HelpxProd/config-6?$png$&jpegSize=100&wid=393)
1. Painter 的材質會出現在內容瀏覽器中，並套用到 UE4 的材質上。

   ![](../../../../assets/link3-11.png){width="500px"}
1. 一個 Substance Painter 專案（.spp）會在 UE4 專案資料夾中標示為「.sp」的資料夾中建立

   ![](../../../../assets/link4-5.png)

## 重新建立與Substance Painter的連結

關閉 Painter 或 Unity 後，你可以從上次停下的地方繼續。

1. 在 Unity 專案>assets>.sp資料夾裡的 Substance Painter 裡開啟 .spp 專案。
1. 在內容瀏覽器中右鍵點擊網格，選擇「傳送給畫家」以重新建立連結。

   ![](../../../../assets/link5-3.png){width="600px"}
