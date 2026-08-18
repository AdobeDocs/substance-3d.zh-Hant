---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/guides/error-and-warning-messages.html"
breadcrumb-title: ''
description: 使用 Substance 軟體烘焙時可能出現的所有錯誤與警告訊息參考指南。
helpx_creative_field: ""
helpx_description: bakers > Guides > Error and Warning Messages
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 錯誤與警告訊息
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '502'
ht-degree: 0%

---


# 錯誤與警告訊息

以下是使用 Substance 軟體烘焙時可能出現的所有錯誤訊息清單。

## 任何烘焙師

| *訊息* | *描述* |
| --- | --- |
| Baker 無法接聽。 | 此錯誤訊息通常會接著額外的錯誤訊息，通常與 GPU 問題相關。 如果 GPU 太老且不符合 [軟體的技術要求](https://www.allegorithmic.com/products/tech-specs) ，可能會發生這種情況。 |
| UV 集合 [X] 不存在。 | Baker 嘗試使用低多邊形網格中不存在的 UV 集合。 |
| 無法從 URL 載入場景。 | 這個訊息表示烘焙者無法載入網格檔案，通常是高多邊形網格。 這則訊息的來源可能有幾個：<ul data-preserve-html="true"><li data-preserve-html="true">提到的網格檔案已經不存在了。</li><li data-preserve-html="true">網狀檔案損壞或損壞，無法讀取。</li><li data-preserve-html="true">網格目前正在被另一個應用程式編輯，無法讀取。</li></ul> |

## UV 轉 SVG Baker

| *訊息* | *描述* |
| --- | --- |
| 找不到 mesh [mesh name] 的 UV。 | 沒有發現針對特定網格的紫外線。 如果匯入多個網格，但只有少數有 UV，可能會發生這種情況。 |
| 這個場景沒有 UV。 取消烘焙。 | 如果場景中沒有任何網格有 UV，烘焙過程就會被取消。 |

## 職位 Baker

| *訊息* | *描述* |
| --- | --- |
| 網格[網格名稱]沒有位置。 | 低多邊形網格沒有頂點位置。 |
| 網格 [網格名稱] 沒有 UV 設定 [X] 的 UV。 | Baker 嘗試使用低多邊形網格中不存在的 UV 集合。 |

## 任何「來自網格」的貝克

| *訊息* | *描述* |
| --- | --- |
| 在網格 [mesh name] 中找不到頂點法線。 | 在給定網格中未發現頂點法線。 通常不會發生，因為如果網格沒有頂點法線，頂點法線會被重新計算。 這可能是因為自訂切線空間插件有問題。 |
| 在網格 [網格名稱] 中找不到頂點切線。 | 同上一樣。 |
| 在網格 [網格名稱] 中找不到頂點雙法定。 | 同上一樣。 |
| 在網格 [mesh name] 中找不到頂點顏色。 | 在給定的網格中未發現頂點顏色。 如果高多邊形網格中至少有一個子網格沒有定義任何頂點顏色，這種情況就可能發生。 |
| 高多邊形的資料不足以使用選定的烘焙軟體。 中止烘焙。 | 至少在上述其中一則訊息之前。 通常，如果場景中只有一點資料缺失（例如：高多邊形場景中只有一個網格沒有頂點顏色），烘焙過程會用零填補缺失的資料，並持續烘焙。 若資料遺失過多，則輸出此訊息並停止烘焙過程。 |

## 從網格轉移貼圖

| *訊息* | *描述* |
| --- | --- |
| 細節貼圖載入失敗。 | 烘焙設定中定義的貼圖無法載入。 可能是因為檔案在磁碟上真的遺失，或是檔案損壞無法讀取。 |
