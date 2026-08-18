---
helpx_url: "https://helpx.adobe.com/tw/substance-3d-integrations/3d-applications/maya/maya-plugin-release-notes/maya-2-2-1.html"
breadcrumb-title: ''
description: 查看 Maya 外掛 2.2.1 版本的發布說明，了解新功能、改進與錯誤修正。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > Maya > Maya Plugin Release Notes > Maya 2.2.1
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Maya 2.2.1
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '226'
ht-degree: 0%

---


# Maya 2.2.1

Maya 2.2.1 版本：

* 更新 Substance Engine 至 8.3.0
* 新增原生支援 Arnold，移除對磁碟快取的需求
* 這可以在設定中啟用渲染擴充功能並重新啟動 Maya 後使用
* 支援的版本包括：
* Maya 2017 - MtoA 3.1.0/Arnold 5.2.0
* Maya 2018 - MtoA 4.0.0/Arnold 6.0.0，MtoA 4.2.0/Arnold 6.2.0
* Maya 2019 - MtoA 4.0.0/Arnold 6.0.0，MtoA 4.2.0/Arnold 6.2.0，MtoA 5.0.0/Arnold 7.0.0
* Maya 2020 - MtoA 4.0.0/Arnold 6.0.0，MtoA 4.2.0/Arnold 6.2.0，MtoA 5.0.0/Arnold 7.0.0
* Maya 2022 - MtoA 4.2.1/Arnold 6.2.0，MtoA 5.0.0/Arnold 7.0.0
* 更新了 Windows 和 MacOS 的安裝目錄
* MacOS/Windows 上的二進位檔現在是使用 Adobe 憑證簽署的
* 當 sbsar 的作者是 Allegorithmic 或 Adobe，而非僅 Allegorithmic 時，頻道切換功能會被隱藏
* 新增 Worfklow 介面，新增複製、覆寫、重命名及刪除工作流程的功能

新增以下腳本指令：

物質瑪雅

substanceGetEnableRenderingExtensions

substanceSetEnableRenderingExtensions

substanceworkflow.py

substanceWorkflowIsReadOnly

substanceWorkflowRenameWorkflow

substanceWorkflowDuplicateWorkflow

substanceWorkflowOverwriteWorkflow

substanceWorkflowRemoveWorkflow

錯誤修正：

* 開啟設定對話框時的修正錯誤
* 產生 pyc 時，工作流程函式不再失敗

此版本於 Maya 2017、2018、2019、2020 及 2022 年在 Linux、MacOS 與 Windows 平台發行，並於 Maya LT 2018、2019 及 2020 年在 MacOS 與 Windows 平台發行
