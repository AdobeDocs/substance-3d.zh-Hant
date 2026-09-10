---
helpx_url: "https://helpx.adobe.com/tw/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-4/unreal-engine-4-plugin-release-notes/unreal-plugin-4-24-0-3.html"
breadcrumb-title: ''
description: 請參閱 Unreal Engine 4 外掛版本 4.24.0.3 的發行說明，了解新功能、改進與錯誤修正。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 4 > Unreal Engine 4 plugin release notes > Unreal plugin 4.24.0.3
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Unreal 外掛 4.24.0.3
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '167'
ht-degree: 0%

---


# Unreal 外掛 4.24.0.3

Unreal Engine 中的 Substance 經歷了重大重組。 這次重組的一部分帶來對 UTexture2D **的完整支援**，並包含輸入與輸出。有了 **UTexture2D** 支援，該外掛現在可以用來發佈到 Unreal 支援的任何平台，包括行動裝置。 除了新增多平台支援外， **UTexture2D** 也允許原生使用 UE4 中的材質串流系統。

該外掛同時完整支援材質 **實例化** ，並引入由 Substance 引擎支援的數值輸出材料範本工作流程。 材質範本讓你可以精確定義如何在 UE4 中設定 Substance 材質著色器。

![](../../../../../assets/ue4-material-templates.png)

我們附帶了用於處理位移、折射及世界排列材質的模板，這些材質內建調整平鋪、貼圖大小、位移與發射參數的控制。 材質範本系統也允許你提供自訂範本。

![](../../../../../assets/ue4-material-instance-params.png)
