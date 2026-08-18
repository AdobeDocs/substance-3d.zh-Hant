---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unity/unity-release-notes/unity-2-3-2.html"
breadcrumb-title: ''
description: 請參閱 Unity 外掛 2.3.2 版本的發行說明，了解新功能、改進與錯誤修正。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Unity Release Notes > Unity 2.3.2
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Unity 2.3.2
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 0%

---


# Unity 2.3.2

## 新功能：

* 材料序列化
* 反思：外掛現在允許在套件中匯入舊的 Substance 檔案（匯入時自動更新為新的 Substance 資料）
* 材料性質會隨著包含物質資料的套件匯入而轉移
  * 注意：此規定僅適用於使用 2.3.0 更新或更新後建立的套件
* 在 Substance 圖表選單中新增了烘焙貼圖按鈕

### 錯誤修正：

* 修正了 Substance 材質平鋪在移除 Library 資料夾後會被重置的問題
* 從遊玩模式出來時速度提升
* 修正了在使用 Substance DLL 時更新插件時的當機問題
* Allegorithmic 資料夾現在無法在 Unity 中刪除。
  * 注意：Allegorithmic 資料夾的內容無法被修改。 在 Unity 內刪除它可能會引發多種問題，導致 Unity 關閉再重新開啟時，Allegorithmic 資料夾會神奇地重新出現。 現在有警告，提醒使用者必須手動從專案的 Assets 資料夾關閉 Unity 刪除
* 從遊玩模式出來時速度提升
* 修正了一個在移除 Library 資料夾時重置物質材質屬性的錯誤

## 已知問題：

**核心物質外掛**

* 使用者必須在 Xcode 的建置設定選單中停用「啟用 Bitcode」才能為 iOS 建置
* Material 不適用於 Asset Bundles
* 資產瀏覽器中的 Substance 預覽圖示在重新匯入後都會全部改成 Substance S 圖示

**腳本編寫**

* 如果專案在建置設定中設定為 x86，腳本在執行時就無法運作
* 在某些建置平台上使用 il2cpp 腳本後端的問題

**Substance Painter 即時連結**

* 在用 Substance Live Link 繪製後建構專案時，已繪製的網格會回到預設材質
* AO 頻道未透過 Painter 即時連結傳送
* 多材質的網格在 Unity Live Link 中無法運作
* Unity LiveLink 使用 SimpleJson 的方式會與專案中其他 SimpleJson 實例衝突
