---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unity/unity-release-notes/unity-2-4-0.html"
breadcrumb-title: ''
description: 請參閱 Unity 外掛 2.4.0 版本的發布說明，了解新功能、改進與錯誤修正。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Unity Release Notes > Unity 2.4.0
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Unity 2.4.0
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 0%

---


# Unity 2.4.0

>[!WARNING]
>
> Unity 將預設建置架構改為 x86，而不是 x86\_64。\
> 如果腳本引用物質，就不會執行。 你需要改回 x86\_64，這樣建置就能正常運作。

## 新功能：

* 新增 HDRP 專案支援（預覽版）
* 在物質選單中新增偏好設定
* 新增設定預設 Substance 解析度匯入設定的功能
* 新增設定預設 Normal 壓縮的功能
* 新增能在 Substance 匯入時產生所有輸出的能力
* 支援自訂輸出 + 相同用途的輸出
* 新增平台解析度設定
* 新增 IL2CPP 支援 錯誤修正

### 錯誤修正：

* 修正了一個在 Mac OS 上開啟 Substance Source 會跳出 Linux 錯誤的錯誤
* 切換平台時所花的時間會縮短。 行動平台的貼圖轉換現在是在建置時完成，而非切換目標平台時。
* 匯入 SBSAR 時斷言失敗錯誤
* 使用 .NET 3.5 升級專案會導致 Substance 材料損壞
* Linux 對話框中不支援 Substance 來源，出現在 OS X 上
* 圖名變更會破壞 ForceText 序列化模式下的預製件與場景檔案
* Substance 材質如果有多個輸出，但用同一方式會壞掉插件在 SBSAR 裡不支援自訂輸出

### 已知問題：

* 當從 2017-2018/2019 升級專案時，使用者匯入 Substance 外掛後，必須重新啟動 Unity 才能更新專案。\
  變通方法：建立一個資產/專案的套件，然後用 2.4.0 外掛匯入新專案。 Substance 檔案應該正確轉換。
* Unity 已經把預設的建構架構改成 x86。 目前，Substance 外掛只支援 x86\_64。

**不再完全支援：**

* Substance Live Link 已從資產商店套件中移除。 （該套件仍可從 Substance Share 下載）
