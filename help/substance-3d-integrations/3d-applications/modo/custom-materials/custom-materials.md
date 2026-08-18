---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/modo/custom-materials.html"
breadcrumb-title: ''
description: 在 MODO 中使用 Unreal、Unity 和 glTF 自訂材質，搭配 Substance 插件來進行專門的工作流程。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > MODO > Custom Materials
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 客製化材料
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '380'
ht-degree: 10%

---


# 客製化材料

Substance 外掛支援 Unreal、Unity 和 glTF 自訂材質。 在載入 SBSAR 檔案之前，你可以選擇想使用的著色模式。

## 目錄

## Unity 資料

使用 Unity 材質時，材質圖層效果會自動設定。 Substance 插件會將 Unity 材質直接放在 Substance Item 材質上方。

| 物質輸出 | 色彩空間 | 材料層效應 |
| --- | --- | --- |
| 基本顏色 | sRGB | 聯合阿爾貝多 |
| 光澤度 | 線性 | Unity 平滑性 |
| 金屬 | 線性 | Unity 金屬 |
| 正常 | 線性 | Unity Normal |
| 發射體 | sRGB | Unity Emission **\*在圖片靜態中設定為 sRGB** |
| 高度 | 線性 | 團結碰撞 |
| 環境遮擋 | 線性 | Unity 環境遮蔽 |

![](../../../assets/unity-1.png){width="600px"}

## 虛幻素材

使用 Unreal Material 時，材質層效果會自動設定。 Substance 插件會把 Unreal Material 直接放在 Substance Item Material 上方。

| 物質輸出 | 色彩空間 | 材料層效應 |
| --- | --- | --- |
| 基本顏色 | sRGB | 虛幻底色 |
| 粗糙度 | 線性 | Unreal Roughness |
| 金屬 | 線性 | 虛幻金屬 |
| 正常 | 線性 | 不真實的正常 |
| 高度 | 線性 | Unreal Bump |
| 發射體 | sRGB | Unreal Emissive **\*在圖片靜態中設定為 sRGB** |
| 環境遮擋 | 線性 | Unreal 環境遮蔽 |
| 不透明度 | 線性 | Unreal Opacity **\*需要取消勾選在材質圖層的反轉** |

![](https://helpx-prod.scene7.com/is/image/HelpxProd/unreal?$png$&jpegSize=200&wid=1343){width="600px"}

你可能需要反轉法線。 如果物質有正常方向的控制，你可以從調整選單中操作。 如果沒有，也可以直接在貼圖上做。 欲了解更多資訊，請參閱「**[法線](../../../3d-applications/modo/working-with-normals/working-with-normals.md)**&#x200B;操作」頁面。

## glTF 材料

使用 glTF 材質時，材質層效果會自動設定。 Substance Plugin 會把 glTF Material 直接放在 Substance Item Material 上方。

| 物質輸出 | 色彩空間 | 材料層效應 |
| --- | --- | --- |
| 基本顏色 | sRGB | glTF 底色 |
| 粗糙度 | 線性 | glTF 粗糙度 |
| 金屬 | 線性 | glTF 金屬 |
| 正常 | 線性 | glTF 普通 |
| 發射體 | sRGB | glTF 發射 **\*在影像靜態中設定為 sRGB** |
| 環境遮擋 | 線性 | glTF 環境遮蔽 |

![](../../../assets/gltf.png){width="600px"}

你可能需要反轉法線。 如果物質有正常方向的控制，你可以從調整選單中操作。 如果沒有，也可以直接在貼圖上做。 欲了解更多資訊，請參閱「**[法線](../../../3d-applications/modo/working-with-normals/working-with-normals.md)**&#x200B;操作」頁面。
