---
helpx_url: "https://helpx.adobe.com/tw/substance-3d-bake/home.html"
breadcrumb-title: ''
description: 學習如何使用 Substance Bakers 將基於網格的資訊計算成貼圖檔案，並提升你的貼圖工作流程。
helpx_creative_field: ""
helpx_description: bakers > Home
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 物質烘焙師
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '363'
ht-degree: 2%

---


# 物質烘焙師

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

<b>Substance Bakers</b> 是一套先進演算法工具組，用來計算基於網格的資訊到貼圖檔案中。任何擁有 3D 網格的藝術家都能使用它們來利用進階貼圖方法。 烘焙是 Substance 軟體工作流程的核心流程，旨在提供<b> 強大的工具</b> 與 <b>自動化貼圖</b>。

本文件涵蓋 <b>烘焙</b> 的基本原理，以及 <b>處理此過程時常見的問題</b> 與錯誤。

</td>
<td width="58.30%" style="border: 0;" valign="top">

![](../assets/optim-baker-home.png){width="400px"}

</td>
</tr>
</table>

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

## 入門

* [什麼是烘焙？](../getting-started/what-is-baking/what-is-baking.md)
* 烘焙方法：
  * [Substance 3D Painter](../getting-started/software-interface/3d-painter/substance-3d-painter.md)
  * [Substance 3D Designer](../getting-started/software-interface/3d-designer/substance-3d-designer.md)
  * [Substance 3D 自動化工具包](../getting-started/software-interface/3d-automation-toolkit/substance-3d-automation-toolkit.md)
* [各軟體的可用性](../getting-started/availability-per-software/availability-per-software.md)
* [相容的 3D 軟體](../getting-started/compatible-3d-software/compatible-3d-software.md)
* [教學課程](../getting-started/tutorials/tutorials.md)

</td>
<td style="border: 0;" valign="top">

### 貝克設定

* [常見參數](../bakers-settings/common-parameters/common-parameters.md)
* [環境遮擋](../bakers-settings/ambient-occlusion/ambient-occlusion.md)
* [來自 Mesh 的環境遮蔽](../bakers-settings/ambient-occlusion-from/ambient-occlusion-from-mesh.md)
* [Mesh 的彎曲法線](../bakers-settings/bent-normals-from-mesh/bent-normals-from-mesh.md)
* [從網格取得色彩映射](../bakers-settings/color-map-from-mesh/color-map-from-mesh.md)
* [將 UV 轉換成 SVG](../bakers-settings/convert-uv-to-svg/convert-uv-to-svg.md)
* [曲率](../bakers-settings/curvature/curvature.md)
* [網格曲率](../bakers-settings/curvature-from-mesh/curvature-from-mesh.md)
* [Mesh 曲率（已棄用）](../bakers-settings/curvature-from-mesh-dep/curvature-from-mesh-deprecated.md)
* [網格高度圖](../bakers-settings/height-map-from-mesh/height-map-from-mesh.md)
* [從網格取得的法線貼圖](../bakers-settings/normal-map-from-mesh/normal-map-from-mesh.md)
* [來自網格的不透明度遮罩](../bakers-settings/opacity-mask-from-mesh/opacity-mask-from-mesh.md)
* [位置](../bakers-settings/position/position.md)
* [來自網格的位置圖](../bakers-settings/position-map-from-mesh/position-map-from-mesh.md)
* [從網格取得厚度貼圖](../bakers-settings/thickness-map-from-mesh/thickness-map-from-mesh.md)
* [從網格轉移貼圖](../bakers-settings/transferred-texture-from/transferred-texture-from-mesh.md)
* [世界太空方向](../bakers-settings/world-space-direction/world-space-direction.md)
* [世界空間法線](../bakers-settings/world-space-normals/world-space-normals.md)

</td>
<td style="border: 0;" valign="top">

### 導遊

* [錯誤與警告訊息](../guides/error-and-warning-mes/error-and-warning-messages.md)
* [效能與優化](../guides/performances-and-opt/performances-and-optimizations.md)
* [烘焙前的三角定位](../guides/triangulating-before-bak/triangulating-before-baking.md)

</td>
</tr>
</table>

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

### 特色

* [幾何快取](../features/geometry-cache/geometry-cache.md)
* [GPU 光線追蹤](../features/gpu-raytracing/gpu-raytracing.md)
* [姓名配對](../features/matching-by-name/matching-by-name.md)
* [切空間](../features/tangent-space/tangent-space.md)

</td>
<td style="border: 0;" valign="top">

### 常見問題

* [如何匯出烘焙好的地圖？](../common-questions/how-export-the-baked-maps/how-to-export-the-baked-maps.md)
* [抖動會應用在烘焙的貼圖上嗎？](../common-questions/dithering-applied-baked/is-dithering-applied-to-baked-textures.md)
* [我應該啟用「計算每個片段的切線空間」嗎？](../common-questions/should-enable-compute-tan/should-i-enable-compute-tangent-space-per-fragment.md)
* [Substance 軟體外烘焙的貼圖看起來不對](../common-questions/texture-baked-outside-sof/texture-baked-outside-of-substance-software-looks-incorrect.md)
* [什麼是 Assbin 檔案？](../common-questions/what-are-assbin-files/what-are-assbin-files.md)
* [烘焙材質的位元深度是多少？](../common-questions/what-the-bit-depth-baked/what-is-the-bit-depth-of-baked-textures.md)
* [OpenGL 和 DirectX 一般格式有什麼差別？](../common-questions/what-the-difference-bet/what-is-the-difference-between-the-opengl-and-directx-normal-format.md)
* [為什麼烘焙或匯出後，我的貼圖會有奇怪的拉伸感？](../common-questions/why-are-there-strange-str/why-are-there-strange-stretches-in-my-textures-after-baking-or-exporting.md)
* [為什麼「依名稱匹配」無法在環境遮蔽/厚度設定中運作？](../common-questions/why-matching-name-not-wor/why-is-matching-by-name-not-working-with-ambient-occlusion-thickness.md)
* [為什麼我的網狀物烘烤後會完全變黑？](../common-questions/why-mesh-fully-black-aft/why-is-my-mesh-fully-black-after-baking.md)

</td>
<td style="border: 0;" valign="top">

### 常見問題

* [UV 接縫上的鋸齒現象](../common-issues/aliasing-on-uv-seams/aliasing-on-uv-seams.md)
* [Baker 輸出為全黑或為空](https://helpx.adobe.com/tw/substance-3d/unlisted/documentation/bake/baker-output-is-fully-black-159451835.html)
* [用 Mesh 的 Color Map 烘焙失敗](../common-issues/baking-failed-with-color/baking-failed-with-color-map-from-mesh.md)
* [黑色陰影十字架可見於網格表面](../common-issues/black-shading-cross-are/black-shading-cross-are-visible-on-the-mesh-surface.md)
* [網狀零件會彼此滲出](../common-issues/mesh-parts-bleed-between/mesh-parts-bleed-between-each-other.md)
* [法線貼圖有奇怪的彩色漸層](../common-issues/normal-map-has-strange/normal-map-has-strange-colorful-gradients.md)
* [一般材質看起來像多面體](../common-issues/normal-texture-looks-fac/normal-texture-looks-faceted.md)
* [烘烤正常紋理後，接縫線可見](../common-issues/seams-are-visible-after/seams-are-visible-after-baking-a-normal-texture.md)
* [每面都能看到接縫](../common-issues/seam-visible-every-face/seam-visible-on-every-face.md)

</td>
</tr>
</table>
