---
helpx_url: "https://helpx.adobe.com/tw/substance-3d-integrations/3d-applications/3ds-max/3ds-max-plugin-release-notes/3ds-max-2-3-1.html"
breadcrumb-title: ''
description: 請參閱 3ds Max 插件 2.3.1 版本的發行說明，了解新功能、改進與錯誤修正。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > 3ds Max > 3ds Max Plugin Release Notes > 3ds Max 2.3.1
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 3ds Max 2.3.1
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 0%

---


# 3ds Max 2.3.1

2020年2月13日發行

這個插件現在會安裝在 3ds Max 目錄外的 C：\ProgramData\Autodesk\ApplicationPlugins\SubstanceIn3dsMax 裡。 現在只要 3ds Max 被指示要找插件，它應該都能正常運作，所以安裝在網路硬碟上等地方應該都能正常使用。\
請注意，切換到 Application Plugin 以及安裝目錄的變更，導致從 2.1.1 版本及之前版本升級時無法正常運作。 這些功能應該在 2018 和 2019 年的 3ds Max 中手動移除。 2.2.0 版本應該會正確升級。\
對於本版本未解決的一些問題，近期將推出另一版以修正這些及其他可能出現的問題。

此版本目前於 2018、2019、2020 及 2021 年版 3ds Max 發行。

* Load sbsar 現在會先在專案圖片資料夾裡查看
* 現在僅在 VRay RT 和 VUE 檔案渲染器中出現 Renderer 相容性對話框
* 關閉 Slate 材質編輯器的拖放功能，以消除 Max 批次的問題
* 渲染對話框不再在 3ds Max 靜音模式下顯示
* 較小的 Python 腳本現已相容於 Python 3
* 新增了對 Substance Launcher 的支援，可以將 Substance Source 資產傳送到 3ds Max。 這需要在啟動器中做調整，但隨著功能加入，外掛上的支援也會持續。
* Redshift 渲染器腳本現在使用 Redshift 2.6.24 中設定的新節點名稱
* 當 Substance2 SubstanceFilePath 被指派空路徑時，Max 不再當機
* 移除 SubstanceOutput 類型與舊插件的名稱碰撞
* 將 SubstanceOutput 類別重新命名為 Substance2Output
* 將 Substance Menu Manager 類別重新命名為 Substance2MenuManager
* 現在，當場景開啟時，參數區塊 ID 會被強制清除，從而消除場景檔案間的碰撞。 這應該能解決在場景間交替時載入時參數區塊無效的問題。 匯入可能仍有問題，因為那需要更複雜的變更
* 這個插件現在安裝在 3ds Max 之外。 所有路徑都已改為相對於負載位置。
* 該外掛現在使用 Autodesk 應用程式外掛系統。
