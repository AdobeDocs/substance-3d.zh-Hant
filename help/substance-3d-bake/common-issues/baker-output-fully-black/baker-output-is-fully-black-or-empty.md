---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/common-issues/baker-output-is-fully-black-or-empty.html"
breadcrumb-title: ''
description: 找出為什麼 baker 輸出完全黑或空，並學習如何修復網格和 UV 問題。
helpx_creative_field: ""
helpx_description: bakers > Common Issues > Baker output is fully black or empty
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Baker 輸出為全黑或為空
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 0%

---


# Baker 輸出為全黑或為空

>[!WARNING]
>
> **子嗣**
> 
> 烘焙的結果是黑色或空洞的紋理：
> 
> ![](../../assets/black.png)

>[!NOTE]
>
> **說明**
> 
> 黑色紋理表示烘焙師無法找到輸出結果所需的資訊。 例如烘焙過程找不到高多邊形網格和低多邊形的網格匹配，導致沒有任何可比較的模型。

>[!NOTE]
>
> **解法**
> 
> * 確認烘焙機所需的高多邊形網格是否正確載入（任何錯誤請參考日誌檔案/視窗）。
> * 確認低多邊形或高多邊形的網格不是太大（超過一公里）或太小（少於一公分）。
> * 確認烘焙師是否能讀取/處理網格（有錯誤請參考日誌檔/視窗）。
> * 確認「按名稱](../../features/matching-by-name/matching-by-name.md)匹配」功能是否[設定不當（有些物件可能彼此排除且永遠不會重疊）。
> * 確認低多邊形的紫外線是否在0-1範圍內。
