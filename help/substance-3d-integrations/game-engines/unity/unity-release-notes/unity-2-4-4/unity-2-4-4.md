---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unity/unity-release-notes/unity-2-4-4.html"
breadcrumb-title: ''
description: 請參閱 Unity 外掛 2.4.4 版本的發佈說明，了解新功能、改進與錯誤修正。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Unity Release Notes > Unity 2.4.4
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Unity 2.4.4
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '186'
ht-degree: 0%

---


# Unity 2.4.4

2020年2月發行

* 新增：2019.3 版的正確支援：修正了導致 Substance 外掛腳本物件受損的 Unity API 變更。 重新設計物件以支援 2019.3 API 更新。 修正 - 使用自訂材質會導致離開遊戲時材質變黑
* 已修正 - 在腳本中使用 Duplicate（） 函式後，進入和退出播放時會當機。
* 已修正 - 材質平鋪、設定與著色器重置於 2019.3 版本
* 已修正 - HDRP 材質著色器不會刷新參數變更
* 已修正 - HDRP 遮罩貼圖未更新
* 固定 - 新增字串參數以重複函式
* 已修正 - 修正最新 Unity Stable 中的 Linux 支援
* 已修正 - 解決 iOS 上必須停用位元碼的問題

已知問題：

* 重新命名 HDRP 資產會導致插件無法產生遮罩貼圖。
* 在使用 Substance 插件進行 HDRP 專案時，使用 Raw 壓縮會將灰階貼圖設定為 Alpha8。
* 遊戲物件會在遊玩模式中取消選取
* 在播放模式下點擊物質圖上的「產生 Mip Maps」，然後更改參數，會導致無限延遲。
