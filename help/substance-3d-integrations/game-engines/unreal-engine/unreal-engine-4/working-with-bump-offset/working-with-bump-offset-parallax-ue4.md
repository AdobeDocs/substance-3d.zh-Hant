---
helpx_url: "https://helpx.adobe.com/tw/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-4/working-with-bump-offset-parallax-ue4.html"
breadcrumb-title: ''
description: 在 Unreal Engine 4 中使用 Substance 材質的凹凸偏移貼圖，來創造深度錯覺和表面細節。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 4 > Working with Bump Offset (Parallax) - UE4
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 使用 Bump Offset（視差）- UE4
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '198'
ht-degree: 0%

---


# 使用 Bump Offset（視差）- UE4

**凹凸偏移** 貼圖透過創意修改 UV 座標，讓表面產生深度錯覺，進一步將紋素與物件表面移開，讓表面看起來比實際細節更多。 在這個「如何做」範例中，我們不僅會說明如何找到 Bump Offset 材質表達式，也會說明如何在材質中利用 Bump Offset 節點。

<https://docs.unrealengine.com/latest/INT/Engine/Rendering/Materials/HowTo/BumpOffset/>

要使用高度輸出，你需要在物質工廠實例中雙擊輸出來建立高度。 高度預設是沒有啟用的。 接著你可以把這個高度輸出拖到你的材質裡。

![](../../../../assets/height-1.png){width="600px"}

建立一個凸起偏移節點，然後把該高度的紅色通道插入 Height。 接著你可以把 TexCoord 輸入到 bump offset 的座標輸入。 最後，凸起偏移的輸出會接到所有 Substance 材質的 UV 輸入端。

![](../../../../assets/bump.png){width="800px"}
