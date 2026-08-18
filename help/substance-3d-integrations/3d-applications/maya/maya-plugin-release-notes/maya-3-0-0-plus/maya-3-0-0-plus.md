---
helpx_url: "https://helpx.adobe.com/tw/substance-3d-integrations/3d-applications/maya/maya-plugin-release-notes/maya-3-0-0-plus.html"
breadcrumb-title: ''
description: 請參閱 Maya 外掛 3.0.0 及以上版本的發布說明，了解新功能、改進與錯誤修正。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > 3ds Max > 3ds Max Plugin Release Notes > Maya 3.0.0
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Maya 3.0.0
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '169'
ht-degree: 0%

---


# Maya 3.0.0+

## Maya 3.0.3

<b>新增/更新：</b>

* 強化了 Maya 外掛的快取系統，使其在初始網路建立時僅快取一次，並啟用手動重存。
* 提供了一個選項，可以更改 Maya 外掛中「substance」資料夾的位置。
* 更新了 Maya 外掛的工作流程匯入系統，以確保與 Autodesk 更新至 Python 3.12 的相容性。
* 更新了 Substance 插件圖示，並加入了最新的圖示。
* 新增了使用 Connector 在外掛中傳送與接收預設的支援。

<b>修正：</b>

* 已解決 Maya 的 Substance 插件載入/卸載時會出現錯誤畫面並當機的問題。
* 修正了快取問題，特別是確保 .exr 檔案正確引用，並減少大型場景中快取相關的凍結。
* 已解決範例視窗中材質預覽在 Maya 外掛載入 SBSAR 檔案時無法顯示的問題。
* 已解決 Connector 無法接收 SBSAR 檔案的問題，前提是至少有一個 SBSAR 已經存在於 Hypershade 中。
