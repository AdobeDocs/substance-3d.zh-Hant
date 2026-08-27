---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/guides/performances-and-optimizations.html"
breadcrumb-title: ''
description: 學習如何優化硬體配置和網格準備，以提升烘焙速度。
helpx_creative_field: ""
helpx_description: bakers > Guides > Performances and optimizations
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 效能與優化
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '612'
ht-degree: 0%

---


# 效能與優化

## 最低硬體需求

使用 Substance Bakers 沒有最低要求，但需注意以下幾點：

* 好的 CPU 能減少計算時間（多核心會加快使用 raytrac 的網狀&#x200B;**烘焙器計算**&#x200B;速度）。
* 有足夠的記憶體（RAM）可以載入包含大量細節（多邊形）的網格。
* 一塊好的 GPU 可以產生高解析度（像是 8K）的材質。

## 三角測量

烘焙師內部使用三角網格;若三維模型（低多邊形與高多邊形）未三角化，烘焙師會自行三角化網格。 此過程可能耗時較長，且會隨著模型中多邊形數量的增加而線性增加。 一般建議將網格（尤其是高多邊形網格）三角定位，以避免烘烤過程中發生此過程。

如果你的工作流程是基於 FBX，你可以在匯出時用 DCC 應用程式中的選項三角定位網格。

## 幾何快取

更多資訊請見以下頁面： [幾何快取](../../features/geometry-cache/geometry-cache.md)

## 抗鋸齒

烘焙師可以使用超取樣來執行抗鋸齒。 超取樣意味著烘焙者會在每個像素投射更多光線以使結果平滑。 此設定會大幅影響烘烤時間;這對於需要大量光線的烘焙機尤其如此，例如網狀烘焙機的環境遮蔽。

舉個例子：

* AA設定為2x2意味著烘焙師會投射出初始射線量的4倍。 對於 2048\*2048 像素的材質，計算結果相當於烘焙一個 4096\*4096px 材質，計算時間約是 4 倍。
* AA 設定為 8x8 意味著烘焙師會投射出初始射線量的 64 倍。 對於 2048\*2048 px 的紋理，計算時間相當於烘焙一個 16384\*16384px 紋理，計算時間約為 64 倍。

**考慮到這些數字，8x8 的設定應該謹慎**&#x200B;使用。

為了減少雜訊存在，通常建議增加次級光線數量（以適應環境遮蔽、厚度及彎曲法線烘焙），並維持2x2或4x4的抗鋸齒設定，而非使用少量次級光線和高抗鋸齒設定。

>[!NOTE]
>
> 一個好的效能/品質設定是用 AA 2x2 和至少 128 條次級光線。

## 檔案格式

匯出磁碟檔案會根據檔案格式、解析度、位元深度和壓縮設定，可能需要相當長的時間。 壓縮設定可在偏好設定 / 專案 / 一般 / 檔案格式選項中修改。 關閉壓縮可以縮短較大檔案的匯出時間。

## 墜機與TDR

當機可能由多種因素引起，其中之一是 TDR（逾時偵測恢復）。 TDR 是 Windows 的機制，設計用來偵測並恢復 GPU 似乎無法回應的情況。 由於 TDR 延遲偵測的預設值較低，在某些情況下使用特定烘焙器時可能會發生崩潰：

* 當用環境遮蔽烘焙器烘烤密集網格時
* 當使用 DXR 加速烘焙器，搭配非常密集的高多邊形網格（超過 6,000 萬個三角形）時，

你可以在這裡找到更多關於 TDR 的資訊和如何修改其相關設定的步驟指南： [GPU 驅動程式在長時間計算時當機（TDR 當機）](https://helpx.adobe.com/substance-3d/unlisted/documentation/spdoc/gpu-drivers-crash-with-long-computations-128745489.html)
