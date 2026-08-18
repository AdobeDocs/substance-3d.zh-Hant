---
helpx_url: "https://helpx.adobe.com/tw/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-5/plugin-settings-ue5.html"
breadcrumb-title: ''
description: 透過 Unreal Engine 5 的專案設定設定 Substance 插件設定，以自訂插件行為。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 5 > Plugin Settings - UE5
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 插件設定 - UE5
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 0%

---


# 插件設定 - UE5

要進入設定，請前往編輯>專案設定，然後往下滑到插件類別，點選 Substance。

![](../../../../assets/screen-shot-2022-03-31-at-5-50-29-pm.png)

## 硬體預算

記憶體預算是 Substance 引擎可使用的最大記憶體量。 可以增加以提升物質處理速度，但會消耗更多系統資源。 （在專案層級，這不一定是有幫助的提升。）

CPU 核心決定了 Substance 引擎允許使用多少核心。 這包括實體核心和超執行緒。 （若分配的編號大於系統可用核心數，則預設使用所有可用核心。

## 烹飪

在烹調過程中移除的 Mip Level 數量會改變包裝材質的產生方式。 此設定能大幅提升載入時間並縮小套件大小，因為較大的貼圖 MIP 層級將不再需要載入。 較低解析度/較小的 LOD 會被載入，最高則由 UE5 預設。 物質接著會透過物質引擎處理，並在運行時更新高解析度的LOD。

Substance Engine 可以是 CPU 或 GPU。 GPU 引擎會讓你製作 4K 材質。 CPU 引擎的效能上限是 2K。

## 優化：

這限制了每批可傳遞給物質引擎的異步物質數量。 數字越低，非同步任務完成和更新的速度越快;數字越大，則會同時處理多個物質。 （數字越高，材質更新越卡，因為更新間隔時間越長。）

## 非同步渲染

同步渲染是一種區塊渲染呼叫。 此時會將 Substance 圖實例傳給 Substance 引擎進行重新計算，但執行會暫停，直到 Substance 引擎完成 Substance 處理後，才會繼續執行後續程式碼。 結果也會在流程結束後立即更新於你的螢幕上。

非同步會將你的圖表加入隊列，並在插件更新中一次將多個圖表傳送到 Substance 引擎（在 Substance 設定中設定）。 與同步渲染不同的是，一旦發送，程式會像平常一樣繼續運行，而不是等 Substance 引擎完成。 當 Substance 引擎完成該批次時，會回傳結果，我們套用到輸出，然後啟動另一批。
