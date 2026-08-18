---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/features/gpu-raytracing.html"
breadcrumb-title: ''
description: 啟用硬體加速的 GPU 光線追蹤，將烘焙計算加速 25 倍以上，以提升工作流程。
helpx_creative_field: ""
helpx_description: bakers > Features > GPU Raytracing
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: GPU 光線追蹤
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '326'
ht-degree: 1%

---


# GPU 光線追蹤

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

有些烘焙師支援 GPU 上的光線追蹤硬體加速，通常能將運算速度提升 25 倍以上。

## 硬體需求

若系統符合以下要求，光線追蹤將自動啟用：

* 已安裝相容的顯示卡/*（RTX 系列、Titan V 或 GeForce 10xx）
* GPU 驅動程式是最新的
* 已安裝 Windows 10「秋季創建者」/十月更新（版本 1809）或更高版本\*\*

</td>
<td style="border: 0;" valign="top">

![GPU 光線追蹤開關](../../assets/rtx-ao-demo.gif "比較 GPU 光線追蹤開關比較"){zoomable="yes"}

</td>
</tr>
</table>

\*：相容的 NVIDIA GPU 包含所有使用 Pascal 架構或較近期的 GPU。 例如，GTX 10 系列、Titan V 系列、RTX 20 系列，或是較新的型號。

\*\*：要查看你的 Windows 版本，請點選開始選單，輸入「winver」並按 Enter。\
你可以透過 [Microsoft 支援網站的專屬頁面](https://support.microsoft.com/en-us/help/4028685/windows-10-get-the-update) 獲得更新。

>[!TIP]
>
> 如果遇到問題，可以在應用程式偏好設定中關閉 GPU 光線追蹤。

## 支持烘焙師

以下表格列出了每位烘焙師依據 Substance 3D 烘焙版本對 GPU 光線追蹤的支援：

+++版本 3 及以上

| 貝克 | 支援 GPU 光線追蹤 |
| --- | --- |
| 環境遮蔽 | <div><img alt="（滴答聲）" data-preserve-html="true" src="../../assets/check.svg"/></div> |
| 彎曲正常 | <div><img alt="（滴答聲）" data-preserve-html="true" src="../../assets/check.svg"/></div> |
| 顏色 | <div><img alt="（滴答聲）" data-preserve-html="true" src="../../assets/check.svg"/></div> |
| 曲率 | <div><img alt="（滴答聲）" data-preserve-html="true" src="../../assets/check.svg"/></div> |
| 高度 | <div><img alt="（滴答聲）" data-preserve-html="true" src="../../assets/check.svg"/></div> |
| 正常 | <div><img alt="（滴答聲）" data-preserve-html="true" src="../../assets/check.svg"/></div> |
| 正常世界空間 | <div><img alt="（錯誤）" data-preserve-html="true" src="../../assets/error.svg"/></div> |



| 貝克 | 支援 GPU 光線追蹤 |
| --- | --- |
| 不透明度遮罩 | <div><img alt="（滴答聲）" data-preserve-html="true" src="../../assets/check.svg"/></div> |
| 位置 | <div><img alt="（滴答聲）" data-preserve-html="true" src="../../assets/check.svg"/></div> |
| 位置低 | <div><img alt="（錯誤）" data-preserve-html="true" src="../../assets/error.svg"/></div> |
| 厚度 | <div><img alt="（滴答聲）" data-preserve-html="true" src="../../assets/check.svg"/></div> |
| 轉印紋理 | <div><img alt="（滴答聲）" data-preserve-html="true" src="../../assets/check.svg"/></div> |
| 世界與切線 | <div><img alt="（錯誤）" data-preserve-html="true" src="../../assets/error.svg"/></div> |


+++

+++版本 2

| 貝克 | 支援 GPU 光線追蹤 |
| --- | --- |
| 環境遮蔽 | <div><img alt="（錯誤）" data-preserve-html="true" src="../../assets/error.svg"/></div> |
| 網格環境遮蔽 | <div><img alt="（滴答聲）" data-preserve-html="true" src="../../assets/check.svg"/></div> \* |
| 網格彎曲法線 | <div><img alt="（滴答聲）" data-preserve-html="true" src="../../assets/check.svg"/></div> \* |
| 網格色彩 | <div><img alt="（錯誤）" data-preserve-html="true" src="../../assets/error.svg"/></div> \* |
| 將 UV 轉換成 SVG | <div><img alt="（錯誤）" data-preserve-html="true" src="../../assets/error.svg"/></div> |
| 網格曲率 | <div><img alt="（滴答聲）" data-preserve-html="true" src="../../assets/check.svg"/></div> \* |
| 網格高度 | <div><img alt="（錯誤）" data-preserve-html="true" src="../../assets/error.svg"/></div> \* |
| 從網格中取法線 | <div><img alt="（錯誤）" data-preserve-html="true" src="../../assets/error.svg"/></div> \* |



| 貝克 | 支援 GPU 光線追蹤 |
| --- | --- |
| 網格的不透明度遮罩 | <div><img alt="（錯誤）" data-preserve-html="true" src="../../assets/error.svg"/></div> \* |
| 網格位置 | <div><img alt="（錯誤）" data-preserve-html="true" src="../../assets/error.svg"/></div> \* |
| 位置 | <div><img alt="（錯誤）" data-preserve-html="true" src="../../assets/error.svg"/></div> |
| 網格厚度 | <div><img alt="（滴答聲）" data-preserve-html="true" src="../../assets/check.svg"/></div> \* |
| 從網格轉移貼圖 | <div><img alt="（錯誤）" data-preserve-html="true" src="../../assets/error.svg"/></div> \* |
| 世界空間方向 | <div><img alt="（錯誤）" data-preserve-html="true" src="../../assets/error.svg"/></div> |
| 世界空間法線 | <div><img alt="（錯誤）" data-preserve-html="true" src="../../assets/error.svg"/></div> |


\*：支援 CPU 光線追蹤，速度明顯比 GPU 光線追蹤慢很多。

+++
