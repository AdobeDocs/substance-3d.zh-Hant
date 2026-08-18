---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unity/unity-release-notes/unity-2-5-2.html"
breadcrumb-title: ''
description: 請參閱 Unity 外掛 2.5.2 版本的發行說明，了解新功能、改進與錯誤修正。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Unity Release Notes > Unity 2.5.2
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Unity 2.5.2
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '147'
ht-degree: 0%

---


# Unity 2.5.2

2020年7月23日發行

補充：

* 「IsProcessing（）」函式，該函式會顯示渲染器是否處於忙碌狀態，或是閒置（非繁忙狀態）

修正：

* 設定 2048 夾具和 4096 目標設定時不再顯示錯誤
* 材料特性在升級為 HDRP 和/或 URP 從標準升級時會繼承
* 修改Substance素材的腳本在部署到行動裝置時會如預期運作
* 紅通道不再複製到 Alpha，預設 Alpha 轉為白色
* Mac 上改變目標設定的當機
* 已移除建立 Unity 材質時的 NullReferenceException 錯誤
* 刪除了編輯平鋪屬性後退出播放模式時的錯誤
* 啟用 GPU 實例化
* 使用透明的材質在現有的遊玩模式中不會消失或錯誤變黑
* 在 HDRP 專案中升級外掛時，物質材質不會被銷毀
