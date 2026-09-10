---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/3ds-max/3ds-max-plugin-release-notes/3ds-max-3-0-0-plus.html"
breadcrumb-title: ''
description: 請參閱 3ds Max 外掛 3.0.0 及以上版本的發行說明，了解新功能、改進與錯誤修正。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > 3ds Max > 3ds Max Plugin Release Notes > 3ds Max 3.0.0
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 3Ds Max 3.0.0
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 0%

---


# 3ds Max 3.0.0+

## 3ds Max 3.0.4

<b>新增/更新：</b>

* 更新了 Substance 插件圖示，並加入了最新的圖示。
* 新增了使用 Connector 在外掛中傳送與接收預設的支援。
* 整合選單管理器，從通知參數取代核心介面的使用。

<b>修正：</b>

* 已解決 Substance 2 材質在 Corona 的 IR/Production 中，當開啟 Slate 材質編輯器並選擇 Substance2 貼圖時，可能會無法渲染的問題。
* 解決了 Sampler Connector 更新時產生新 Substance2 節點，而非更新現有節點的問題。
* 解決了 3ds Max 插件新增 Substance2 節點時的當機問題，並確保使用 Batch Import 載入 .sbsar 檔案時不會再開啟腳本編輯器。
* 解決了 3DSMax 2025 外掛在使用 .msi 安裝程式時因不相容的 .dll 檔案而無法載入的問題。

## 3ds Max 3.0.2

<b>新增/更新：</b>

* Substance 外掛中標準化圖示管理，將所有現有圖示整合至 qrc 與 rcc 檔案，符合 Autodesk 偏好的方法，並確保 SBSAR 圖形面板載入一致。
* 強化了外掛中 Substance Settings 視窗的響應速度，確保調整視窗大小時輸入欄位及其描述能正確契合。
* Substance 外掛現已相容於 Corona 11。

<b>修正：</b>

* 解決了 V-Ray 材料中光澤顏色與光澤粗糙度無法自動連接的問題。 現在，兩個屬性在 V-Ray 和 Arnold 建立工作流程時都會自動連結。
* 修正了插件中的一個介面問題，調整 CPU 核心限制設定時，如果儲存的數值是個位數，會錯誤顯示兩位數值。
* 已修正 3ds Max 插件 v3.0.0 在主控台中與 Substance 相容性功能相關的渲染錯誤。 現在，使用 Substance Batch 匯入選單建立的 substance 節點會如預期般渲染。
