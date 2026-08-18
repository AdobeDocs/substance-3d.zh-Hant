---
helpx_url: "https://helpx.adobe.com/tw/substance-3d-integrations/game-engines/unity/unity-release-notes/unity-2-2-0.html"
breadcrumb-title: ''
description: 請參閱 Unity 外掛 2.2.0 版本的發布說明，了解新功能、改進與錯誤修正。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Unity Release Notes > Unity 2.2.0
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Unity 2.2.0
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '674'
ht-degree: 0%

---


# Unity 2.2.0

## 2.2.0 發行說明

**發行日期：2019/10**

### 核心外掛：

* 更新版物質引擎
* 提升程式碼穩定性
* **Unity 2018.3 支援**
* **.NET 4.x 支援**
* 2018.3 年的 Substance Source 支援
* Substance Source 的著色問題已修正
* 該圖及對應的材質現在擁有相同的物件名稱
* 新增 Unity Pro 皮膚圖形介面可讀性提升
* 新增對素材輸出指派的支援
* 修正了 sRGB 處理的一個錯誤
* 修正了一個使用者可以刪除所有圖實例的錯誤
* 修正了一個錯誤，就是在執行時嘗試渲染 Substument 並改變參數時，一次只能渲染兩個
* 當匯入包含舊 Substance 檔案的套件時，外掛會告知使用者該套件包含舊 Substance 資料，並在 Unity 嘗試匯入時刪除套件檔案（這樣使用者就不必手動刪除所有檔案，若檔案本身壞掉了）
* 在 Substance 選單中新增了一個「關於」按鈕，用來顯示與 Substance 插件相關的建置資訊
* 在 Substance GUI 中新增滑鼠懸停工具提示，以顯示暴露的 Substance 參數名稱
* 在 Substance 圖形介面中新增了導覽按鈕，可連結到 Substance 圖表和材質
* 在內容瀏覽器中新增了 Substance 圖表/材質/材質的圖示
* 在內容瀏覽器更新了Substance的縮圖
* 移除了 Substance 材料名稱前方的 .mat 標籤
* 新增了重新命名Substance圖表和材質的功能
* 當更改 Substance 圖解析度時，套用/還原的彈窗將不再出現，強制使用者當下提交變更
* 修正了一個 Bug，反射過程只使用預設的 Substance 解析度，而非使用者自行定義的解析度
* 在 Substance 介面中新增滑鼠懸停警告，提醒使用者色彩空間是否設定為 Gamma
* Substance 圖實例功能變更：使用者現在可以在 Substance 中建立圖實例，無需在 Substance 圖圖形介面中提示每個實例

### 腳本：

* 我們隱藏了一些不適合腳本支援的功能
* 新增了透過腳本複製 Substance 圖實例的功能：Duplicate（）
* 新增了透過 C# 查詢程序輸入資訊的函式，回傳一個包含 &#39;InputProperties&#39; 元素的陣列：GetInputProperties（）
* 新增一個用來檢查圖形中是否存在輸入的函式，回傳真/假：HasInput（字串 inputName）
* 新增了檢查 visibleif 輸入是否可見的函式，回傳 true/false：IsInputVisible（字串 inputName）
* 渲染方案已重新設計。 因此，RenderSubstancesAsync（） 已被棄用，並改為 graphName.RenderAsync（）

## 已知問題：

**核心物質外掛**

* 使用者必須在 Xcode 的建置設定選單中停用「啟用 Bitcode」才能為 iOS 建置
* 當建置目標設為 Android/iOS 時，內容瀏覽器中的 Substance 物件預覽會顯示為黑色
* 匯入 Substance 外掛後，非 Substance 材質介面中缺少 Alpha 按鈕和 Mip Map 預覽滑桿
* 使用者必須使用二的冪次方來透過腳本定義 Substance 圖的解析
* 物質材質在使用 Unity 套件匯出或匯入時不會持續存在
* Material 不適用於 Asset Bundles
* 資產瀏覽器中的 Substance 預覽圖示在重新匯入後都會全部改成 Substance S 圖示
* 重新命名場景中有材質的 Substance 圖，會將該材質從放置物件中移除
* （僅限 Mac）在 Mac 上更新外掛會移除場景中預製件中的 Substance 材質|

**腳本編寫**

* 如果專案在建置設定中設定為 x86，腳本在執行時就無法運作
* 在某些建置平台上使用 il2cpp 腳本後端的問題

**Substance Painter 即時連結**

* 在用 Substance Live Link 繪製後建構專案時，已繪製的網格會回到預設材質
* AO 頻道未透過 Painter 即時連結傳送
* 多材質的網格在 Unity Live Link 中無法運作
* Unity LiveLink 使用 SimpleJson 的方式會與專案中其他 SimpleJson 實例衝突
