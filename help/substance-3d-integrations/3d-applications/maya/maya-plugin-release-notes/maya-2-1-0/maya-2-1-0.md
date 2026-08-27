---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/maya/maya-plugin-release-notes/maya-2-1-0.html"
breadcrumb-title: ''
description: 請參閱 Maya 外掛 2.1.0 版本的發行說明，了解新功能、改進與錯誤修正。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > Maya > Maya Plugin Release Notes > Maya 2.1.0
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Maya 2.1.0
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '357'
ht-degree: 0%

---


# Maya 2.1.0

Maya 2.1.0 變更日誌中的 Substance

* 確保與 Python 3 的相容性
* Substance Engines 更新至 7.2.9 版本
* 在套用工作流程時，解決了全域 mel 變數名稱衝突的錯誤
* Redshift 工作流程現在將 Frennel 設為金屬性
* 新增外掛檔 substancelink，處理與其他 Substance 程式及 Substance 啟動器的互通性
* 現在打開 Substance Source，如果已經載入 Substancelink 外掛，就會開啟 Substance Launcher 到「Source」分頁
* Substancelink 外掛允許啟動器在新增 UI 時，將 Substance Source 材質傳送到 Maya 整合
* 新增腳本指令以取得內部函式庫版本，以及開啟物質啟動器至原始碼頁面
* 網站連結現在已開放至 [substance3d.com](http://substance3d.com) 而非 [allegorithmic.com](http://allegorithmic.com)
* 文件與原始碼連結在開啟網頁時，現在會開啟使用者設定的預設瀏覽器
* 在 Windows 上，Internet Explorer 已不再開啟
* 在書架和選單中新增了 Substance 分享的連結
* 新增了查詢 Substance Linker 版本和雜湊值的新指令
* 在 Maya LT 中，該版本已從設定選單中移除
* 關於選單不再用 PySide2 和 Python 撰寫，而是用原生程式碼使用 Qt 撰寫。 現在它已經在 Maya LT 版本中提供，之前沒有。
* 關於選單有不同的診斷資訊;現在會顯示 git 雜湊值，以匹配來源控制的變更
* 關於選單複製到剪貼簿的版本現在也會有這個 git 雜湊值，以及該外掛所支援的 Maya 版本。
* 關於視窗中的授權現在以文字檔開啟
* 新增對 Maya 2017 的支援
* 工作流程腳本產生器不再輸出「排序」成員的字串。 現有的工作流程都會被妥善處理

新增的腳本指令：\
物質瑪雅：\
\* substanceUtilityGetLinkerVersion\
\* substanceUtilityGetLinkerHash\
\* 物質UiOpenAboutWindow（關於窗戶）\
\* substanceUiOpenSource網站\
\* substanceUiOpenDocumentation\
\* 內容UiOpenShareWebsite

Substancelink：\
\* 內容連結GetLinkVersion。\
\* substanceLinkGetPortalCliVersion\
\* 內容連結OpenLauncher

此版本於 Windows 平台的 Maya 2017、2018、2019 及 2020 年版本發行，\
Linux 和 Macos。 它也在 Maya LT 2018、2019 和 2020 年版上發行\
Windows 和 MacOS。
