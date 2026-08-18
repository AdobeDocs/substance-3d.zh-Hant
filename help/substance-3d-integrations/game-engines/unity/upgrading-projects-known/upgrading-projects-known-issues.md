---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unity/upgrading-projects-known-issues.html"
breadcrumb-title: ''
description: 了解如何用 Substance 材質升級 Unity 專案，以及遷移過程中已知要避免的問題。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Upgrading ProjectsKnown Issues
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 專案升級已知問題
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '161'
ht-degree: 1%

---


# 升級專案/已知問題

>[!WARNING]
>
> Unity 3.0.0 的 Substance 3D 外掛不支援向下相容。 所以，請務必使用 Unity 2020.3.27x 及以上版本。
> 
> Unity 將預設建置架構改為 x86，而不是 x86\_64。\
> 如果腳本引用物質，就不會執行。 你需要改回 x86\_64，這樣建置就能正常運作。

## 已知問題

* 在瀏覽面板資料夾時出現「*陳述失敗」錯誤。*
  * 這是 Unity 端發生的錯誤，當對使用者介面做變更時，通常是縮圖變更，應該是無害的訊息。
* *影像輸入似乎被鎖定在 8 位元。*
  * 這個問題在 3.8.0-3 版本中被修正。 正確的工作流程是讓使用者將 Unity 的材質預設格式改成 RGBA64。 外掛會負責正確地將這些資訊傳送給 Substance 引擎。
