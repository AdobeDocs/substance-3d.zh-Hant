---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-5/installing-to-source-builds-ue5.html"
breadcrumb-title: ''
description: 在 Unreal Engine 5 原始碼建置中安裝 Substance 3D 插件，以便自訂引擎修改。
helpx_creative_field: ""
helpx_description: Substance 3D Integrations
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 安裝至原始碼建置 - UE5
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '303'
ht-degree: 0%

---


# 安裝至原始碼建置 - UE5

Substance 外掛可搭配從原始碼編譯的 Unreal Engine 版本使用。 為此，外掛可安裝於 C++project 資料夾或原始碼建置的引擎資料夾中。

>[!NOTE]
>
> 這些方法需要你從市集下載外掛版本。 Substance 插件資料夾可以在電腦與 UE 版本間轉移。

## 安裝到 C++ 專案資料夾

1. 在專案資料夾中，如果還沒有插件資料夾，請建立。
1. 在 Plugins 資料夾裡，建立一個 Runtime 資料夾。
1. 把 Substance 資料夾放進 Runtime 資料夾裡。 LINUX 使用者：步驟 3 後，找到 Substance 資料夾中的「include」資料夾，並將其名稱改為「i」（include > Include）。
1. 啟動 Unreal Engine。
1. 透過啟動器開啟 C++ 專案。
1. 啟動專案後，Unreal Engine 會跳出提示，問你是否想在啟動前重建插件元件，請選擇「是」。 這會透過 Microsoft Visual Studio（Windows、Linux）或 Xcode（Mac）來完成。
1. Unreal Engine 會關閉，但元件會在背景建置。 這個過程大約需要5分鐘。 完成後，專案將正式展開。 如果失敗，你會看到錯誤視窗。

## 安裝到 Engine 資料夾

>[!NOTE]
>
> 必須依上述步驟重建外掛 Binaries 資料夾，才能將外掛安裝到 Engine 資料夾中。

1. 從執行時> Plugin>s  專案資料夾複製 Substance 資料夾。
1. 打開 Unreal Engine 版本資料夾，然後前往 Marketplace > Engine > Plugins。
1. 貼上物質資料夾。
1. 打開 Unreal Engine 編輯器。 如果需要，可以創建新專案。
1. 打開插件選單，確認 Substance 插件是否啟用。
