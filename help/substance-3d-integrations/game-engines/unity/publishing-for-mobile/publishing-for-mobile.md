---
helpx_url: "https://helpx.adobe.com/tw/substance-3d-integrations/game-engines/unity/publishing-for-mobile.html"
breadcrumb-title: ''
description: 在 Unity 中調整設定與材質解析度，優化行動平台的 Substance 材質。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Publishing for Mobile
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 行動出版
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '226'
ht-degree: 0%

---


# 行動出版

>[!NOTE]
>
> **行動裝置上的貼圖大小**
> 
> Unity 編輯器中材質集的解析度會是應用程式二進位檔中發佈的大小。 降低 Substance 材質的解析度會產生檔案大小較小的貼圖。

## 月台

## Apple iOS

1. 請確保 iOS 模組是為對應的 Unity 版本下載的。
1. 在 Unity 裡，將建置目標改成 iOS。
1. 打開玩家設定，將「識別 - 組合識別碼」欄位改成更獨特的欄位。 （例如：com.Adobe.iosProject）
1. 打造並執行遊戲。
1. 在 Xcode 中，點選 iOS 裝置，將「簽署 - 團隊」下拉選單改成你的開發團隊 ID。
1. 在 iOS 裝置上，點選「設定 - 一般 - 裝置管理」，然後點擊出現的開發團隊 ID 上的「信任」。
1. 點擊「建置並執行目前方案」按鈕（播放按鈕）重新執行 Xcode 建置。
1. 遊戲應該能在 iOS 裝置上運行。

## Android 作業系統

1. 請確認 Android 模組是為對應的 Unity 版本下載的。
1. 在 Unity 裡，將建置目標改成 Android。
1. 打開玩家設定，將「識別 - 組合識別碼」欄位改成更獨特的欄位。 （例如：com.Adobe.androidProject）
1. 打造並執行遊戲。
1. 遊戲應該能在 Android 裝置上運行。
