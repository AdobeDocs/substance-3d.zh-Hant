---
helpx_url: "https://helpx.adobe.com/tw/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-4/plugin-settings-ue4.html"
breadcrumb-title: ''
description: 透過 Unreal Engine 4 的專案設定來自訂插件行為。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 4 > Plugin Settings - UE4
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 插件設定 - UE4
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '567'
ht-degree: 0%

---


# 插件設定 - UE4

要進入設定，請前往編輯>專案設定，然後往下滑到插件類別，點選 Substance。

![](../../../../assets/settings-36.png){width="400px"}

## 硬體預算

記憶體預算是物質引擎可使用的最大記憶體量。 可增加以提升物質處理速度，但會消耗更多系統資源。 （在專案層級，這不一定是有幫助的提升。）

CPU 核心數是 Substance 引擎允許使用的核心數。 這包括實體核心和超執行緒。 （若分配的編號大於系統可用核心數，則預設使用所有可用核心。

## 烹飪

在烹調過程中移除的 Mip Level 數量會改變包裝材質的產生方式。 此設定能大幅提升載入時間並縮小套件大小，因為較大的貼圖 MIP 層級將不再需要載入。 較低解析度/較小的 LOD 會被載入，最高 LOD 會由 UE4 預設。 這些物質隨後會透過物質引擎處理，並在運行時更新高解析度的LOD。

Substance Engine 可以是 CPU 或 GPU。 GPU 引擎會讓你製作 4K 材質。 CPU 引擎的效能上限是 2K。

## 預設生成：

物質生成模式（SGM）控制材質的產生方式。 這是物質的全局設定。 SGM可在物質工廠依據物質進行變更。

**SGM Baked**：烘烤物質的紋理。 你在執行時失去了改變參數的能力。

**SGM 載入同步**：在物質載入時阻擋該應用。

**SGM 在載入同步與快取**&#x200B;時：將貼圖的中間結果快取到磁碟上。

**SGM 負載非同步**：非阻塞。 物質是在背景中產生的。

**SGM 在非同步載入與快取**&#x200B;時：將貼圖的中間結果快取到磁碟上。

***平台預設是非同步載入與快取***

## 物質工廠

要更改某個物質的 SGM，請右鍵點擊物質工廠>資產行動>透過屬性矩陣進行批量編輯。 你就可以更改 SGM。

![](../../../../assets/sgm.png){width="800px"}

## 優化：

這限制了每批可傳遞給物質引擎的異步物質數量。 數字越低，非同步任務完成和更新的速度越快，數字越高則會同時處理多個內容。 （數字越高，材質更新越卡，因為更新間隔時間越長。）

## 非同步渲染

同步渲染是一種區塊渲染呼叫。 此時會將一個實體圖實例傳給待重新計算的實體引擎，但執行會暫停，直到實體引擎完成該實體處理後，才會繼續執行任何程式碼。 結果也會在流程結束後立即更新於你的螢幕上。

非同步會將你的圖表加入佇列，並在插件更新中一次將多個圖表傳送到物質引擎（在物質設定中設定）。 與同步渲染不同的是，一旦發送，程式會像平常一樣繼續運行，而不是等物質引擎完成。 當物質引擎完成該批次時，會回傳結果，我們套用到輸出，然後啟動另一批。
