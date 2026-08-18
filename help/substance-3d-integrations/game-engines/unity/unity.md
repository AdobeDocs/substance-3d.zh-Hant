---
helpx_url: "https://helpx.adobe.com/tw/substance-3d-integrations/game-engines/unity.html"
breadcrumb-title: ''
description: 在 Unity 遊戲引擎中匯入並使用 Substance 材質，並支援原生插件並控制執行時參數。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 統一
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '743'
ht-degree: 0%

---


# 統一

![](../../assets/unity.png)

>[!NOTE]
>
> **Unity 支援版本**
> 
> Adobe Substance 3D 外掛目前支援 Unity 2020.3.27x 及以上版本。 你可以從 [Unity 資產商店](https://assetstore.unity.com/packages/tools/utilities/substance-3d-for-unity-beta-213208)下載。

>[!WARNING]
>
> 在升級或使用外掛前，請先查看 [升級專案頁面](https://helpx.adobe.com/tw/substance-3d/unlisted/documentation/integrations/upgrading-projects-182256244.html)。

>[!WARNING]
>
> 在撰寫自訂物質材料前，務必先查看 [優化指南](../../game-engines/unity/optimization-guidelines/optimization-guidelines.md) 頁面。

## 目錄

* [Unity 發布說明](https://helpx.adobe.com/tw/substance-3d/unlisted/documentation/integrations/beta-release-information-170460277.html) — Substance in Unity 插件版本的新內容
* [在 Unity](../../game-engines/unity/downloading-plugin-unity/downloading-substance-3d-plugin-in-unity.md) 下載 Substance 3D 外掛 — Adobe Substance 3D for Unity 可在 Unity 資產商店 https://assetstore.unity.com/packages/tools/utilities/substance-in-unity-110555 取得。
* [Unity 外掛概述](../../game-engines/unity/unity-plugin-overview/unity-plugin-overview.md)
* [Unity 偏好設定](../../game-engines/unity/unity-preferences/unity-preferences.md) — Substance 偏好設定視窗允許你設定外掛的使用者自訂選項。
* [優化指南](../../game-engines/unity/optimization-guidelines/optimization-guidelines.md) — 在製作自訂物質材料時，務必查看以下優化指南。
* [升級專案/已知問題](https://helpx.adobe.com/tw/substance-3d/unlisted/documentation/integrations/upgrading-projects-182256244.html) — Substance in Unity 插件的已知問題
* [管理 Substance Graphs](https://helpx.adobe.com/tw/substance-3d/unlisted/documentation/integrations/managing-and-navigating-substance-graphs-170459636.html) — 您可以使用 Substance Graph Manager （SGM） 根據 Substance Material 建立新材料
* [參數變更](../../game-engines/unity/changing-parameters/changing-parameters.md) — 物質材料的參數可在物質圖物件（SGO）中存取。
* [生成材質（包裝）](../../game-engines/unity/generated-textures-pac/generated-textures-packing.md) — 生成材質顯示物質引擎計算出的材質輸出以產生材質
* [渲染色彩空間](../../game-engines/unity/rendering-color-space/rendering-color-space.md) — 為了獲得最佳效果，你應該在 Unity Player 設定中將色彩空間設為線性。
* [使用影像輸入](../../game-engines/unity/using-image-inputs/using-image-inputs.md)
* [行動](../../game-engines/unity/publishing-for-mobile/publishing-for-mobile.md) 平台出版指南 — 行動平台發佈指南
* [Substance 3D 用於 Unity 腳本](../../game-engines/unity/3d-for-unity-scripting/substance-3d-for-unity-scripting.md) — 利用 Substance API，你可以撰寫腳本在執行時更新和更改 Substance 參數。
* [Unity 中的腳本（已棄用）](https://helpx.adobe.com/tw/substance-3d/unlisted/documentation/integrations/scripting-in-unity-170459644.html) — 利用 Substance API，你可以撰寫腳本在執行時更新和更改 Substance 參數。
* [Substance 3D 資產庫的使用](https://helpx.adobe.com/tw/substance-3d/unlisted/documentation/integrations/substance-3d-assets-library-225970070.html)
* [移除 Substance 插件](../../game-engines/unity/removing-plugin/removing-substance-plugin.md)
* [Unity 中的 Substance 3D 教學](../../game-engines/unity/3d-in-unity-tutorials/substance-3d-in-unity-tutorials.md)
* [Unity 中的實體尺寸](../../game-engines/unity/physical-size-in-unity/physical-size-in-unity.md)
* [專案間共享 sbsar 檔案](https://helpx.adobe.com/sharing-sbsar-files-between-projects.html) [&#128279;](../../game-engines/unity/sharing-sbsar-files-bet/sharing-sbsar-files-between-projects.md)

**[已找到表格 - 需規則]**

>[!WARNING]
>
> 在升級或使用外掛前，請先查看 [升級專案頁面](https://helpx.adobe.com/tw/substance-3d/unlisted/documentation/integrations/upgrading-projects-182256244.html)。

>[!WARNING]
>
> 在撰寫自訂物質材料前，務必先查看 [優化指南](../../game-engines/unity/optimization-guidelines/optimization-guidelines.md) 頁面。

### 目錄

* [Unity 發布說明](https://helpx.adobe.com/tw/substance-3d/unlisted/documentation/integrations/beta-release-information-170460277.html) — Substance in Unity 插件版本的新內容
* [在 Unity](../../game-engines/unity/downloading-plugin-unity/downloading-substance-3d-plugin-in-unity.md) 下載 Substance 3D 外掛 — Adobe Substance 3D for Unity 可在 Unity 資產商店 https://assetstore.unity.com/packages/tools/utilities/substance-in-unity-110555 取得。
* [Unity 外掛概述](../../game-engines/unity/unity-plugin-overview/unity-plugin-overview.md)
* [Unity 偏好設定](../../game-engines/unity/unity-preferences/unity-preferences.md) — Substance 偏好設定視窗允許你設定外掛的使用者自訂選項。
* [優化指南](../../game-engines/unity/optimization-guidelines/optimization-guidelines.md) — 在製作自訂物質材料時，務必查看以下優化指南。
* [升級專案/已知問題](https://helpx.adobe.com/tw/substance-3d/unlisted/documentation/integrations/upgrading-projects-182256244.html) — Substance in Unity 插件的已知問題
* [管理 Substance Graphs](https://helpx.adobe.com/tw/substance-3d/unlisted/documentation/integrations/managing-and-navigating-substance-graphs-170459636.html) — 您可以使用 Substance Graph Manager （SGM） 根據 Substance Material 建立新材料
* [參數變更](../../game-engines/unity/changing-parameters/changing-parameters.md) — 物質材料的參數可在物質圖物件（SGO）中存取。
* [生成材質（包裝）](../../game-engines/unity/generated-textures-pac/generated-textures-packing.md) — 生成材質顯示物質引擎計算出的材質輸出以產生材質
* [渲染色彩空間](../../game-engines/unity/rendering-color-space/rendering-color-space.md) — 為了獲得最佳效果，你應該在 Unity Player 設定中將色彩空間設為線性。
* [使用影像輸入](../../game-engines/unity/using-image-inputs/using-image-inputs.md)
* [行動](../../game-engines/unity/publishing-for-mobile/publishing-for-mobile.md) 平台出版指南 — 行動平台發佈指南
* [Substance 3D 用於 Unity 腳本](../../game-engines/unity/3d-for-unity-scripting/substance-3d-for-unity-scripting.md) — 利用 Substance API，你可以撰寫腳本在執行時更新和更改 Substance 參數。
* [Unity 中的腳本（已棄用）](https://helpx.adobe.com/tw/substance-3d/unlisted/documentation/integrations/scripting-in-unity-170459644.html) — 利用 Substance API，你可以撰寫腳本在執行時更新和更改 Substance 參數。
* [Substance 3D 資產庫的使用](https://helpx.adobe.com/tw/substance-3d/unlisted/documentation/integrations/substance-3d-assets-library-225970070.html)
* [移除 Substance 插件](../../game-engines/unity/removing-plugin/removing-substance-plugin.md)
* [Unity 中的 Substance 3D 教學](../../game-engines/unity/3d-in-unity-tutorials/substance-3d-in-unity-tutorials.md)
* [Unity 中的實體尺寸](../../game-engines/unity/physical-size-in-unity/physical-size-in-unity.md)
