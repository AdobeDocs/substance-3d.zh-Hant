---
helpx_url: "https://helpx.adobe.com/tw/substance-3d-integrations/renderers/color-management.html"
breadcrumb-title: ''
description: 在使用 Substance 材質搭配不同渲染器時，了解色彩管理與伽瑪校正。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Renderers > Color Management
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 色彩管理
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '683'
ht-degree: 0%

---


# 色彩管理

我們將採取簡化的方法，說明線性空間渲染能提供正確的光照計算數學。 它創造了一個環境，使光線互動能以可信的真實世界方式呈現。 關於線性空間渲染的討論，我們必須介紹伽瑪修正的概念。 在編碼影像以供顯示和儲存用途時，伽瑪校正是優化頻寬與位元分配的過程。 此過程利用人眼對亮度的感知，亮度大致遵循亮度的立方根。

>[!NOTE]
>
> 線性空間渲染是一個高度複雜的學科。 欲了解更多資訊，請參閱免費 [的PBR指南第一卷](https://academy.substance3d.com/courses/the-pbr-guide-part-1) ，內容關於 [Substance Academy](https://academy.substance3d.com/)。

## 色彩管理

本文件的目的是詳細說明如何處理從 **Substance Painter** 和 **Substance Designer** 匯出的材質，並以 3D 軟體[&#128279;](https://www.adobe.com/tw/products/substance3d/3d-augmented-reality.html)及渲染器進行處理。

正確解讀作為材質通道輸入的影像，取決於該影像在場景中的使用方式。 色彩空間、編碼，以及色彩值是否與&#x200B;**場景參考亮度**&#x200B;**或顯示**&#x200B;亮度成正比，也扮演重要角色。

* 用於表示 **非彩色資料** 的影像不應被轉換。 這些&#x200B;**&#x200B;**&#x200B;**通常是正常、粗糙度**、**金屬感**、**位移**&#x200B;和&#x200B;**環境**&#x200B;**遮蔽**&#x200B;等。
* 代表我們所見顏色的影像可以有多種情境。 例如，已經&#x200B;**是場景線性的**&#x200B;影像通常不需要轉換，例如&#x200B;**儲存在 OpenEXR** 和 **HDR** 等格式&#x200B;**的高動態範圍**&#x200B;影像。
* 為顯示而製作的影像（**顯示參考**）則需去除其伽瑪影像。 這些格式包括大多數格式，如 **PNG、**&#x200B;**JPEG** 和 **BMP**。這些影像分為&#x200B;**底**&#x200B;**色**、**漫反射**、**鏡面及**&#x200B;**發射。**

雖然這是過度簡化的說法，但將過程理解為以下會有幫助：

* 「場景指涉（例如） 線性化） ： 不要套用轉換
* 「顯示參考（例如） sRGB）」：應用反轉換以「線性化」影像以進行正確計算

>[!NOTE]
>
> sRGB 解碼函數（EOTF）將伽瑪空間轉換為線性空間，用於 Substance Painter 與 Substance Designer，並由 IEC 61966-2-1：1999 標準定義

Substance Designer 可設定為使用 [OpenColorIO](https://opencolorio.org/) 進行色彩管理。 這讓你能在多個應用程式中保持一致&#x200B;**&#x200B;的色彩轉換和影像顯示。在此模式下，Substance Designer 內部會處理 &#x200B;** 線性 RGB **&#x200B; 色彩。 由於 8 位元深度通常不足以表示線性顏色，因此建議圖形中的[&#128279;](https://docs.substance3d.com/display/SDDOC/Graph+View)色彩紋理至少使用&#x200B;**&#x200B;**16位元**&#x200B;深度。

![](https://helpx-prod.scene7.com/is/image/HelpxProd/sd-cm?$png$&jpegSize=200&wid=686)

當我們引入 [ACES](https://www.oscars.org/science-technology/sci-tech-projects/aces) 時，現在有兩種不同的色彩空間：線性 sRGB（無伽瑪版本的 sRGB）和 [ACEScg](https://acescolorspace.com/)，後者是一種寬色域（「場景參考」或線性）色彩空間，更適合 CG 渲染。

*色系圖示 -<https://acescolorspace.com/>*

Substance Designer 也支援 **Adobe Color Engine（ACE）。**&#x200B;使用 **ACE** 時，你可以選擇工作色彩空間，選擇 **sRGB**、 **線性 sRGB** 和 **ACEScg**。 使用 **sRGB** 時， **ACE** 基本上和舊模式一樣。 使用線性色彩空間時， **ACE** 大致上類似 [OpenColorIO](https://opencolorio.org/index.html)。

## Substance 插件

透過 Substance Integration 插件使用 Substance 材質時，輸出會透過整合系統和主機應用程式的色彩管理自動標記為線性/伽瑪。 不過，了解這個過程很重要：當 Substance 貼圖被用作匯出的點陣圖而非 Substance 材質時，你可能需要根據你使用的渲染器，手動標記這些貼圖為 **gamma 編碼** 或 **原始** 材質。 通常 8 或 16 位元 .png、.jpg、.tga 或 .tif 檔案是 gamma 編碼，而 **sRGB OETF** 和 .exr 檔案則是線性編碼。

## 3D 應用

### 處理貼圖

* [瑪雅中的物質材質](../../renderers/color-management/textures-in-maya/substance-textures-in-maya.md)
* [3ds Max 中的物質材質](../../renderers/color-management/textures-in-3ds-max/substance-textures-in-3ds-max.md)
