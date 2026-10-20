---
description: 從官方網站或 Blender 的附加元件管理器下載並安裝 Substance 3D Blender 外掛。
title: 下載與安裝外掛
user-guide-description: ""
user-guide-title: ""
source-git-commit: aa5acd016cd1a55ab230d36352c4d3aa5514012a
workflow-type: tm+mt
source-wordcount: '634'
ht-degree: 0%
---

# 下載與安裝外掛

## 下載

要下載外掛，請造訪 [Blender](https://substance3d.adobe.com/plugins/substance-in-blender/) 中的 Substance 3D。 點擊 **下載外掛** 開始下載。

你也可以直接從下方連結取得最新版本。

有兩個獨立的.zip檔案可供下載和安裝：

* Substance 3D Blender 外掛（[所有平台](https://www.adobe.com/go/substance3d-blender-multi-latest)單次下載）
* Substance 3D 整合工具（下載 [Windows](https://www.adobe.com/go/substance3d-integrationtools-win-latest)、 [Mac](https://www.adobe.com/go/substance3d-integrationtools-mac-latest)或 [Linux](https://www.adobe.com/go/substance3d-integrationtools-lin-latest) 版本）

>[!WARNING]
>
> **對於 Mac 使用者：***如果使用 Safari 下載外掛，應關閉「下載後開啟安全檔案」。*
>
> Safari 網頁瀏覽器預設會解壓下載的 .zip 檔案，安裝時必須保持壓縮狀態。 為了防止檔案解壓縮，請更新 Safari 偏好設定，讓下載後不要打開「安全」檔案。
>
> 1. 開放式狩獵
> 1. 點擊 **偏好設定**
> 1. 在「一般」標籤下，取消勾選「下載後開啟「安全」檔案的選項 **。**

## 安裝步驟

### 首次安裝

1. 從 Adobe 預發布頁面下載 Plugin .zip 檔案。
1. Open Blender（與 3.0 或更高）。
1. 從頂端導覽欄，選擇編輯，然後選擇偏好設定。 然後選擇「附加元件」標籤。
1. 點擊 **安裝** 按鈕。
1. 在檔案總管裡，找到.zip檔案下載的資料夾
1. 選擇Substance3DInBlender.zip檔案，點選 **安裝附加** 元件按鈕。
1. 在附加元件區塊中，點選啟用附加元件的勾選框，然後點擊下拉箭頭展開該區塊。
1. 系統會提示您安裝整合工具。 點選 **從磁碟** 安裝，選擇 **Substance3DIntegrationTools.zip** ，然後點選 **安裝工具** 按鈕。\
   如果之前沒有下載過，請點擊 **下載** ，在瀏覽器中開啟 Adobe 預發布頁面並下載工具，然後使用 **「從磁碟** 安裝」來安裝。
1. 這個附加元件現在已經準備好可以使用了！

![](../../../assets/blender-install.gif)

### 更新外掛與工具

1. 從上方連結下載最新發行版本。
1. 使用 **卸載工具** 按鈕移除 Substance 3D 整合工具。
1. 使用 **「移除** 」按鈕來卸載該附加元件
1. 關閉並重新啟動 Blender
1. 從頂端導覽欄，選擇編輯，然後選擇偏好設定。 然後選擇「附加元件」標籤。
1. 點擊 **安裝** 按鈕。
1. 在檔案總管中，找到新下載的 ZIP 檔案。
1. 選擇Substance3DInBlender.zip檔案，然後點擊 **安裝** 附加元件按鈕。
1. 在附加元件區塊中，點選啟用附加元件的勾選框，然後點擊下拉箭頭展開該區塊。
1. 系統會提示您安裝整合工具。 點選 **從磁碟** 安裝選擇Substance3DIntegrationTools.zip，然後點選 **安裝工具** 按鈕。\
   如果之前沒有下載過，請點擊 **下載** ，在瀏覽器中開啟 Adobe 預發布頁面並下載工具，然後使用 **「從磁碟** 安裝」來安裝。
1. 這個附加元件現在已經準備好可以使用了！

### 更新各個組件

僅更新附加元件時：

1. 在附加元件偏好設定中，使用 **「移除** 」按鈕來卸載該附加元件。
1. 重新啟動攪拌機
1. 再次進入附加元件偏好設定，使用 **安裝** 按鈕載入新版本的外掛。 先前載入的整合工具將保留。

僅更新整合工具時：

1. 在附加設定中，使用 **更新工具** 按鈕載入較新的整合工具版本。 先前使用的附加元件將保留。
1. 重新啟動 Blender 以取得變更效果。

或

1. 在附加元件偏好設定中，使用 **卸載工具** 按鈕移除整合工具。
1. 重新啟動攪拌機
1. 使用 **「從磁碟** 安裝」按鈕來尋找並載入新版本的整合工具。 先前使用的附加元件將保留。