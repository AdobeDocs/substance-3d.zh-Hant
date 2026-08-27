---
helpx_url: "https://helpx.adobe.com/tw/substance-3d-integrations/game-engines/unity/unity-release-notes/unity-2-4-5.html"
breadcrumb-title: ''
description: 請參閱 Unity 外掛 2.4.5 版本的發行說明，了解新功能、改進與錯誤修正。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Unity Release Notes > Unity 2.4.5
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Unity 2.4.5
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '344'
ht-degree: 0%

---


# Unity 2.4.5

2020年4月6日發行

* 新增：使用 2019.3 API 進行 HDRP 資產檢查
* 新增：Substance Engine 7.2 更新 - 修正 Source 中部分 Substance 材料無法運作
* 新增：更新目標設定以匹配 CPU 解析度
* 新增：CPU 引擎最大解析度設定（4K 或 2K 設定）
* 新增：在 HDRP 專案中轉換非 HDRP 物質
* 已修正：大量進口物質時會當機
* 已修正：在更改Substance參數後，點擊遊戲模式重新匯入時出現異常
* 修正：驗證輸出（紋理）解析度（API限制CPU引擎至2K）使用者偏好設定預設為4K
* 修正：在播放模式下點擊物質圖上的「產生 Mip 映射」，然後更改參數會導致無限卡頓
* 修正：在使用 Substance 插件進行 HDRP 專案時，使用 Raw 壓縮會將灰階材質設定為 Alpha8
* 修正：遊戲物件在遊玩模式中取消選取
* 已修正：粗糙度貼圖不會隨著參數變更而更新
* 修正：某些 Substance 檔案在 HDRP 中，遮罩輸出未正確產生
* 已修正：在切換 packed alpha 地圖下拉選單時會當機
* 已修正：當點擊離開 Substance 材質時，GPU 實例化的勾選框會被回復。
* 修正：使用複製（）函數時，複製的物質圖沒有正確地將平滑度壓縮進金屬的 alpha 中。
* 修正：將建置目標切換到 Android 會導致材質格式錯誤，直到手動重新匯入為止。
* 已修正：在 Unity 中刪除 Substance 檔案會觸發 NullReferenceException。
* 已修正：停用先前版本的 Unity 2019.3 HDRP API

已知問題：

* 排放核取框預設未啟用，且 HDR 值在物質匯入時設為黑色。
* 標準物質包裝的材料特性不會帶入進口。
* 2017-2019/2020 年的更新在 HDRP 中無法運作
* 在設定選單中選擇 4096 時（未點選套用）時，點擊設定選單中的 2048 夾具選項（未點選套用），會在主控台日誌中出現錯誤
