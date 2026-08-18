---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unity/unity-release-notes/unity-2-3-4.html"
breadcrumb-title: ''
description: 請參閱 Unity 外掛 2.3.4 版本的發行說明，了解新功能、改進與錯誤修正。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Unity Release Notes > Unity 2.3.4
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Unity 2.3.4
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '409'
ht-degree: 0%

---


# Unity 2.3.4

>[!WARNING]
>
> **使用 Unity 2019.2 的外掛會產生以下錯誤：**
> 
> InspectorSubstanceImporter.OnInspectorGUI 必須呼叫 ApplyRevertGUI，以避免意外行為。\
> UnityEditor.Experimental.AssetImporters.AssetImporterEditor:OnDisable（）\
> Substance.Editor.InspectorSubstanceImporter:OnDisable（）
> 
> 此錯誤可清除，不會影響外掛功能

>[!WARNING]
>
> **請閱讀：物質材料破裂：**\
> 包含自訂輸出且使用空白的物質材料，匯入時會壞掉。 此外，含有重複使用內容的物質材料也會損壞。\
> GameTextures.com 的舊 sbsar 檔案目前不相容 Substance in Unity 外掛。 這些包含不支援使用輸出的教材正在失效。 使用插件前，務必備份專案。

## 新功能：

* 新增對 Substance Engine v7 的支援
* 新增 Linux 支援

### 錯誤修正：

* 修正了在沒有材質貼圖的情況下匯入 Substance 相關的問題
* 已修正 Unity 2019.x 中反射過程無法正常運作的問題
* 修正了進口含有 Substance 材料預製件的包裹時的預製件處理問題
* 固定材質/貼圖指派在反射過程後未被帶入
* 修正了更換著色器導致材質損壞的問題
* 修正了粗糙度無法被壓縮到金屬 alpha 通道的問題
* 修正了安裝 Substance 外掛時，更改非 Substance 材質的匯入設定會讓某些選項被回退的問題。
* 已修正 Substance Source 在 Mac 上無法開啟的問題

## 已知問題：

**核心物質外掛**

* 使用者必須在 Xcode 的建置設定選單中停用「啟用 Bitcode」才能為 iOS 建置
* Material 不適用於 Asset Bundles
* 資產瀏覽器中的 Substance 預覽圖示在重新匯入後都會全部改成 Substance S 圖示
* 自訂物質材料如果輸出設定使用量為空白，會破壞材料
* 自訂物質材料如果有重複用途會破壞材料
* 在 Linux 匯入外掛後，編輯器必須重新啟動

**腳本編寫**

* 如果專案在建置設定中設定為 x86，腳本在執行時就無法運作
* 在某些建置平台上使用 il2cpp 腳本後端的問題

**Substance Painter 即時連結**

* 在用 Substance Live Link 繪製後建構專案時，已繪製的網格會回到預設材質
* AO 頻道未透過 Painter 即時連結傳送
* 多材質的網格在 Unity Live Link 中無法運作
* Unity LiveLink 使用 SimpleJson 的方式會與專案中其他 SimpleJson 實例衝突
