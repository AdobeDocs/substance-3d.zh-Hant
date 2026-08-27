---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/3ds-max/troubleshooting.html"
breadcrumb-title: ''
description: 使用 Script Listener 在 3ds Max 中診斷並解決 Substance 插件的錯誤訊息問題。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > 3ds Max > Troubleshooting
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 疑難排解
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '209'
ht-degree: 1%

---


# 疑難排解

腳本監聽器可用來診斷使用外掛時遇到的錯誤。 要開啟腳本監聽器，請進入腳本選單>腳本聽取器。 當外掛使用過程中發生錯誤時，對應的錯誤訊息會印到這個腳本監聽器視窗。 欲知更多資訊，請造訪 [官方劇本編輯文件](https://help.autodesk.com/view/3DSMAX/2023/ENU/?guid=GUID-C8019A8A-207F-48A0-985E-18D47FAD8F36) 。

若要回報錯誤，請加入 Substance Discord 伺服器的 [&#128279;](https://discord.com/invite/substance3d)#3dsmax-plugin 頻道，或造訪 [Adobe 社群](https://community.adobe.com/t5/substance-3d-plugins/ct-p/ct-substance-3d-plugins?page=1&sort=latest_replies&lang=all&tabid=all&topics=label-autodesk3dsmax)。主控台日誌中的相關資訊及任何重複步驟可納入報告中。

## 已知問題

* *將使用漫射輸出的 .sbsar 替換成不使用漫射輸出的 .sbsar，會導致因缺少的漫射斷線而呈現黑色渲染。*
  * 這是多輸出節點的預期行為。 建議不要用同一個節點載入這些 .sbsar，而是分別使用不同的 Substance 節點。
