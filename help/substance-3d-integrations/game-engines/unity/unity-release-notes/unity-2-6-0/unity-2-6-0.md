---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unity/unity-release-notes/unity-2-6-0.html"
breadcrumb-title: ''
description: 請參閱 Unity 外掛 2.6.0 版本的發行說明，了解新功能、改進與錯誤修正。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Unity Release Notes > Unity 2.6.0
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Unity 2.6.0
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '191'
ht-degree: 0%

---


# Unity 2.6.0

2021年6月7日發行

更新/新增：

* 存取物質來源的新工作流程！ Substance Source 動作現在會進入 Substance Launcher 中的 Source 標籤，讓資產可以直接傳送到 Unity
* 插件版本資訊可以複製到剪貼簿
* 「載入時產生」已從目標設定中移除

修正方法：

* 在 HDRP 專案中，當材質設定有變更時，位移模式會回復到預設值（Tessallation）
* 解析度大小不會顯示在檢查器視窗中
* 無法安裝到 Unity 2020.2 及以上版本的外掛

已知問題：

* 存取被拒錯誤及/或當機發生在從 2.5.4 及以下版本更新外掛時
  * 解決方法：先前的 2.5.4 及以下插件版本，安裝 2.6.0 版本前，必須先從 Unity 專案 2020.2 及以上版本中卸載
* 安裝 Substance 外掛時，影像檔案的貼圖預覽不會在檢查器中顯示
  * 這個問題的根源存在於 Unity 內部，並計劃在 2021.2 版本（目前為測試階段）中修復
