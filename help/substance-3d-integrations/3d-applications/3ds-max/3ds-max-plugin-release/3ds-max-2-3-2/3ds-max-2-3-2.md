---
helpx_url: "https://helpx.adobe.com/tw/substance-3d-integrations/3d-applications/3ds-max/3ds-max-plugin-release-notes/3ds-max-2-3-2.html"
breadcrumb-title: ''
description: 請參閱 3ds Max 外掛 2.3.2 版本的發佈說明，了解新功能、改進與錯誤修正。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > 3ds Max > 3ds Max Plugin Release Notes > 3ds Max 2.3.2
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 3ds Max 2.3.2
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 0%

---


# 3ds Max 2.3.2

2020年4月8日發行

今天我們釋出了外掛的 2.3.2 版本，主要是在 2.3.1 基礎上的錯誤修正版本。

2.3.2 發行：

* Substance 引擎更新至 7.2.9
* 已修正 Redshift/VRay 在 2018、2019 及 2020 年 3ds Max 中渲染時當機的問題
* 除錯斷言錯誤將不再出現
* Substance2 節點現在正確地擁有 iMultipleOutputChannelsWithValues 的腳本介面
* 選單中的 Substance 來源條目現在會開啟 Substance 啟動器到來源標籤，如果已安裝的話
* 物質材質現在在使用 Corona 渲染器時應該會正確更新
* Substance 輸出在 VRay Next 使用時不再暫時被影像取代
* 自動套用的渲染相容性對話框已移除。 如果需要，設定對話框裡仍然可以找到
* 修正了在 3ds Max 2021 中套用物質材質時，匯出 FBX 可能出現的問題

已知問題：

* 在 3ds Max 2018 中，匯出帶有 Substance 材質的 fbx 會在 fbxmax.dlu 插件中當機。 我們目前正在與 Autodesk 洽談，看看我們這邊是否有可做的事，還是這是舊版 fbx 整合的限制。 之前的解決方法不可靠，後來被移除。 在 2019 年或更新版本的 3ds Max 中則沒有這種情況。

此版本於 2018、2019、2020 及 2021 年版 3ds Max 發行。
