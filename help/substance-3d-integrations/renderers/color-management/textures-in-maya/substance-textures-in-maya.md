---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/renderers/color-management/substance-textures-in-maya.html"
breadcrumb-title: ''
description: 在 Maya 中為 Substance 材質設定色彩空間，以確保色彩管理與渲染的準確度。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Renderers > Color Management > Substance textures in Maya
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 瑪雅中的物質材質
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '134'
ht-degree: 0%

---


# 瑪雅中的物質材質

你為地圖設定的色彩空間取決於 Maya 色彩管理設定[&#128279;](https://help.autodesk.com/view/MAYAUL/2020/ENU/?guid=GUID-B260195C-A0FE-4F51-9EA2-099B61B7725A)中所設定的規則。

Substance in Maya 外掛在檔案節點上設定為「忽略色彩空間檔案規則」。 該外掛會根據以下方式處理色彩空間設定，無論有沒有色彩管理：

基色、漫射、發射、鏡面 = sRGB\
法線、高度、位移、粗糙度、金屬質感 = RAW

通常，對於代表非顏色資料的影像，你需要將色彩空間設為 RAW。 不過，這個設定可能會受到你在色彩管理中設定的規則影響。

![](../../../assets/raw.png)
