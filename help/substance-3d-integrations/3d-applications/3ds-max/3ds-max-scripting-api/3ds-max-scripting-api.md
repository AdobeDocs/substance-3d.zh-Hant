---
helpx_url: "https://helpx.adobe.com/tw/substance-3d-integrations/3d-applications/3ds-max/3ds-max-scripting-api.html"
breadcrumb-title: ''
description: Substance 3ds Max 腳本 API 的參考文件，用於自動化物料作業。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > 3ds Max > 3ds MAX Scripting API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 3ds MAX 腳本 API
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '895'
ht-degree: 0%

---


# 3ds MAX 腳本 API

以下是 Substance 2 節點的指令與屬性列表。

## 屬性：

| 財產 | 說明 | 類型 |
| --- | --- | --- |
| 名稱 | Substance2 節點的名稱。 預設是「Substance2」。 | 弦 |

## 指令：

| 指揮 | 說明 | 返回 | 退貨類型： | 參數 |
| --- | --- | --- | --- | --- |
| getCurrentPackageName | 取得載入套件的基礎檔名（sbsar file 載入於圖節點） | 載入套件（sbsar 檔案）的檔名（不含前綴目錄） | 弦 |  |
| getCurrentGraphName | 取得目前圖表的名稱 | 目前圖實例的識別碼 | 弦 |  |
| getOutputsNamesFromCurrentGraph | 取得啟用輸出的輸出使用名稱清單 | 包含啟用輸出通道名稱列表的表格 | 列表 |  |
| getPresetIdentifiers | 從 Substance 圖表取得預設列表 | 包含所有預設的字串識別碼清單的表格 | 列表 |  |
| setPackageAndGraphNames | 從磁碟載入 sbsar 檔案到圖形節點 | 成功時為真，失敗時為假 | 布林值 | ***String parameter：**&#x200B;***substancePackageFilePath** 指向磁碟上 sbsar 檔案的路徑&#x200B;***String parameter***： **graphInstanceNameToSelect** 圖的字串識別碼 |
| setInputInt | 設定一個整數輸入並設定一個新的值 |  |  | ***整數參數***： **value** 整數值用以設定輸入為&#x200B;***字串參數***： **inputIdentifier** 輸入的唯一字串識別碼 |
| setInputFloat | 設定一個浮點點數輸入並設定一個新值 |  |  | ***浮點參數***： **value** 浮點點數值用來設定輸入為&#x200B;***字串參數***： **inputIdentifier** 輸入的唯一字串識別碼 |
| setInputString | 設定一個新值的字串輸入 |  |  | ***字串參數***： **value** 字串值用來設定輸入為&#x200B;***字串參數***： **inputIdentifier** 輸入的唯一字串識別碼 |
| setInputBool | 設定一個布林輸入並設定新值 |  |  | ***布林參數：* 值&#x200B;**&#x200B;布林值以設定輸入為&#x200B;***字串參數&#x200B;***： **inputIdentifier** 輸入的唯一字串識別碼 |
| setInputVec2 | 設定一個包含兩個元素的向量輸入 |  |  | Point2 參數：**&#x200B;*** value **最大 point2 值用以設定輸入為&#x200B;***String參數&#x200B;***：**&#x200B;inputIdentifier** 輸入的唯一字串識別碼 |
| setInputVec3 | 設定一個包含三個元素的向量輸入 |  |  | ***Point3 參數：* 值&#x200B;**&#x200B;最大點3值以設定輸入為&#x200B;***字串參數&#x200B;***： **inputIdentifier** 輸入的唯一字串識別碼 |
| setInputVec4 | 設定一個包含四個元素的向量輸入 |  |  | ***Point4 參數***： **值** 最大 point4 值以設定輸入為&#x200B;***字串參數：* inputIdentifier &#x200B;** 輸入的唯一字串識別碼 |
| setInputColor | 設定一個顏色輸入，並設定一個新的值 |  |  | ***顏色參數***： **值** 最大顏色值以設定輸入為&#x200B;***字串參數：* inputIdentifier &#x200B;** 輸入的唯一字串識別碼 |
| setInputComboSelection | 在組合輸入中設定目前選取的值 |  |  | ***整數參數***： **value** 組合盒小工具的索引&#x200B;***字串參數***： **inputIdentifier** 輸入的唯一字串識別碼 |
| getInputInt | 取得整數輸入型態的輸入值 | 輸入的當前整數值 | 整數 | ***字串參數：* inputIdentifier &#x200B;** 輸入的唯一字串識別碼 |
| getInputFloat | 取得浮點數輸入類型的輸入值 | 輸入的當前浮點數值 | 浮標 | ***字串參數：* inputIdentifier &#x200B;** 輸入的唯一字串識別碼 |
| getInputString | 取得字串輸入類型的輸入值 | 輸入的當前字串值 | 弦 | ***字串參數：* inputIdentifier &#x200B;** 輸入的唯一字串識別碼 |
| getInputBool | 取得布林輸入型態的輸入值 | 輸入的當前布林值 | 布林值 | ***字串參數：* inputIdentifier &#x200B;** 輸入的唯一字串識別碼 |
| getInputVec2 | 取得 point2 輸入類型的輸入值 | 輸入的當前最大 point² 值 | 第二點 | ***字串參數：* inputIdentifier &#x200B;** 輸入的唯一字串識別碼 |
| getInputVec3 | 取得 point3 輸入類型的輸入值 | 輸入的當前最大點三方值 | 第3點 | ***字串參數：* inputIdentifier &#x200B;** 輸入的唯一字串識別碼 |
| getInputVec4 | 取得 point4 輸入類型的輸入值 | 輸入的當前最大 Point4 值 | 第四點 | ***字串參數：* inputIdentifier &#x200B;** 輸入的唯一字串識別碼 |
| getInputColor | 取得顏色輸入類型的輸入值 | 輸入的當前值作為顏色 | 顏色 | ***字串參數：* inputIdentifier &#x200B;** 輸入的唯一字串識別碼 |
| getInputComboSelection | 根據識別碼取得組合盒選擇的索引 | 所選組合盒項目的索引 | 整數 | ***字串參數：* inputIdentifier &#x200B;** 輸入的唯一字串識別碼 |
| getMaterialDependentCount | 取得材料依賴的數量 | 具有材料類型的依賴參考數量 | 整數 |  |
| ApplyValuesToSelectedPreset | 將目前選擇的預設值覆蓋為當前輸入值 |  |  |  |
| 移除所有預設 | 移除目前圖節點中的所有預設 |  |  |  |
| CreatePreset | 從目前的輸入建立一個新的預設 |  |  | ***字串參數：* newPresetName &#x200B;** 新預設的顯示名稱 |
| RemoveOnePreset | 移除帶有名字的預設 |  |  | ***String 參數：* selectPresetName &#x200B;** 要移除的預設名稱 |
| ImportPreset | 將 sbsprs 檔案匯入目前的預設 |  |  | String 參數：**&#x200B;***filePath** 包含匯入預設的檔案路徑的字串 |
| ExportPreset&#x200B;**\*deprecated** 在 2.5.0\* 中移除 | 將目前選擇的預設匯出成 sbsprs 檔案 |  |  | ***字串參數***： **filePath** 包含檔案路徑的字串，用來匯出預設為 |
| exportPresetList | 將給定的預設匯出成單一預設檔 |  |  | ***String 參數***：filePath **包含匯出預設值的檔案路徑的字串***List 參數&#x200B;***：**&#x200B;預設 **&#x200B; 包含要匯出的**&#x200B;預設名稱的清單 |
| BakeOutputsOfSelectedGraph | 將所選圖形實例的位圖烘焙到磁碟 |  |  | ***String 參數：* filePath &#x200B;** 用來寫入圖片的根路徑目錄&#x200B;***String參數&#x200B;***： **imageFormatExtension** 將影像寫入為 |
