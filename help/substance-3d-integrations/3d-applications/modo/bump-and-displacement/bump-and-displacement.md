---
helpx_url: "https://helpx.adobe.com/tw/substance-3d-integrations/3d-applications/modo/bump-and-displacement.html"
breadcrumb-title: ''
description: 在 MODO 中使用 Substance 材質的凹凸與位移貼圖，為模型增添表面細節與深度。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > MODO > Bump and Displacement
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 凸起與排氣量
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '151'
ht-degree: 0%

---


# 凸起與排氣量

與凸起與排氣的合作

物質可以有可選的高度輸出。 你可以把它當作排氣或凸起。 當你啟用高度時，它會被設定成凸起貼圖效果。 Unity 的設定會設為 Unity Bump，Unreal 則是 Unreal Bump。 接著你可以選擇物質物品材質，並相應地設定凸起幅度。 如果你想用高度作為位移，可以將材質層效果改成 surface shading > Displacement。 接著在材質參考中設定適當的位移距離。

![](../../../assets/bump-1.png)

在這個例子中，我使用 Unreal 材質，但將 Unreal 的凹凸層效果改成了位移。 接著在物質物品材質上設定位移距離並相應地渲染細分層級。

![](../../../assets/dis.png)
