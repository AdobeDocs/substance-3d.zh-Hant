---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/modo/modo-plugin-release-notes/modo-v-2-7-0.html"
breadcrumb-title: ''
description: 請參閱 MODO 外掛 2.7.0 版本的發布說明，了解新功能、改進與錯誤修正。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > MODO > Modo Plugin Release Notes > Modo v. 2.7.0
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Modo 訴 2.7.0
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '203'
ht-degree: 0%

---


# Modo 訴 2.7.0

* 多次當機修復
* 32 位元浮點數支援
* CPU 引擎有 4K 材質，GPU 引擎有 8K 材質
* 插件版本的新 LPK 格式
* Substance 插件的新套件選單
* glTF / MODO 12.0 的原則著色器支援
* Substance 檔案新增相對路徑
* Linux 支援
* 新的預設值載入與儲存介面
* 嵌入式預設是從 Designer 載入的
* 移除了 GPU 記憶體警告框
* 編輯了預設的載入/儲存指令

  新增的指令包括：

  **substance.getsbsname** 將 substance 物件的識別碼轉換為其內部名稱

  這些都期望從 substance.getsbsname 獲得一個正式的內部名稱：

  **substance.setpreset** 將 Substance 目前預設設為索引 **substance.getpresetindex** 取得當前預設索引 **substance.getpresetat 在指定索引 substance.getpresetcount****回傳 Substance 在指定**&#x200B;索引處預設&#x200B;**的字串名稱 substance.savepresetfile** 將目前設定的預設儲存到指定檔案路徑 **substance.loadpresetfile** 將預設檔載入給定的 Substance

  UI 指令：

  **substance.loadpresetUI** 指令用來載入預設 **的 substance.savepresetUI** 指令 儲存預設 **的 Substance.selectpresetUI** UI 指令用來設定預設
