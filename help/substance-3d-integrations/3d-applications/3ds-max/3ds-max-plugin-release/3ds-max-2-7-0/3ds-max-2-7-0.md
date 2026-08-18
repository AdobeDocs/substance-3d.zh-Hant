---
helpx_url: "https://helpx.adobe.com/tw/substance-3d-integrations/3d-applications/3ds-max/3ds-max-plugin-release-notes/3ds-max-2-7-0.html"
breadcrumb-title: ''
description: 請參閱 3ds Max 外掛 2.7.0 版本的發行說明，了解新功能、改進與錯誤修正。
helpx_creative_field: ""
helpx_description: Substance 3D Integrations
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 3ds Max 2.7.0
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '302'
ht-degree: 0%

---


# 3ds Max 2.7.0

<b>新增/更新：</b>

* 將 Substance 引擎升級到 3ds Max 插件中的第 9 版，提升效能與相容性。

<b>修正：</b>

* 修正了 2019、2022、2023 和 2024 年版 3ds Max 的當機問題，當時拖曳 Substance 2 節點進入 Slate 材質編輯器會導致程式當機。 Substance 2 節點現在可以安全地拖放到 Slate 材質編輯器中。
* 解決了 3ds Max 的 Substance 插件中一個問題，選擇「Substance to Arnold」及其他工作流程時，無法在 Material Slate 編輯器中建立相關節點，反而錯誤地開啟了一個 Maxscript，並出現編譯錯誤。 像 Arnold 這類工作流程的節點現在會自動正確生成並連接。
* 解決了一個問題：從 Substance 3D Sampler 匯出起始資產/預設（.sbsar - Substance2 材質貼圖），再轉到 3ds Max 中的 Corona Renderer（版本 6 到 9hf1），結果材質損壞、渲染時底色變黑且凹凸法線壞掉。 此外，這次更新解決了材料中物質屬性標籤的無法存取問題，這個問題也影響了轉換成 Vray。
* 修正了 3ds Max 插件中一個問題，當從 Substance2 材質輸入插入或拔除 Corona Material 會導致當機
* 解決了 3ds Max 2024 中預設不允許嵌入或呼叫 Python 腳本的相容性問題
* 修正了 3Ds Max 插件中一個問題，匯入並執行 Substance to Corona 插件時，材質在著色器預覽和渲染中呈現黑色且閃亮。 此問題現已成功解決，確保 Corona 渲染器正確顯示與渲染 Substance 貼圖。

此版本於 2021、2022 及 2023 年推出 3ds Max 版本
