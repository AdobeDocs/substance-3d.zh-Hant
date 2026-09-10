---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/bakers-settings/curvature-from-mesh-deprecated.html"
breadcrumb-title: ''
description: 參考 Mesh baker 已棄用的 Curvature。 改用 Mesh baker 更新的 Curvature 版本。
helpx_creative_field: ""
helpx_description: bakers > Bakers Settings > Curvature from Mesh (deprecated)
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Mesh 曲率（已棄用）
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '144'
ht-degree: 0%

---


# Mesh 曲率（已棄用）

mesh baker 的曲率會從高多邊形網格產生曲率紋理。 它比基礎 [曲率](../../bakers-settings/curvature/curvature.md) 烘焙器慢，但產生更精確的結果。

**提供：**

* 物質設計師
* 物質自動化工具包

>[!NOTE]
>
> 自 Substance Designer 2019.3 起，這款烘焙器已被棄用，我們建議改用 [mesh](../../bakers-settings/curvature-from-mesh/curvature-from-mesh.md) baker 的新 Curvature。

## 參數

| *參數* | *描述* |
| --- | --- |
| **強度** | 曲率細節的強度。 若 **啟用軟飽和** ，該參數將被停用。 |
| **軟**  **飽和度** | 啟用後，曲率細節會被柔化。 |
| **最大化射程** | 啟用後，曲率細節會被納入貼圖範圍的容量內。 這表示非常強的數值會被定義為最大值，其他數值則會依此極端值進行調整。 |
