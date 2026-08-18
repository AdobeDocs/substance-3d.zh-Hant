---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unity/changing-parameters.html"
breadcrumb-title: ''
description: 在 Unity 中修改 Substance 材質參數，以在執行時自訂材質外觀與屬性。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Changing parameters
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 參數變更
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '208'
ht-degree: 0%

---


# 參數變更

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

物質材質的參數可在物質圖物件（SGO）中存取。

1. 在專案視窗中，選擇你想自訂的圖表的 sbsar 檔案標誌。 SBSAR上有綠色的「SBSAR」標誌。

   ![](../../../assets/screen-shot-2022-03-29-at-2-27-56-pm.png)

## 程序性質

1. **產生所有輸出**：從 Substance sbsar 檔案產生所有輸出。 預設情況下，只會產生標準著色器使用的輸出。
1. **產生 Mipmaps**：會為每個 Substance 輸出產生 MIP 貼圖。
1. **隨機種子**：這個按鈕會改變物質圖用來生成材質的隨機種子。 更改此值會根據種子值產生新的紋理結果。
1. Substance 檔案中暴露的參數可在 Unity 中取得。 編輯器控制是根據為該物質所建立的參數類型而設。
1. **預設處理：** 你可以匯出或匯入 Substance 預設檔案（sbsar）。 匯出預設會根據 Substance 的參數設定建立一個預設檔案。 你可以從 Substance Designer 和 Substance Player 匯出預設檔案，然後用匯入預設按鈕匯入。 這有助於在應用程式和團隊間分享 Substance 預設。

</td>
<td style="border: 0;" valign="top">

![](../../../assets/changing-parameters.png)

</td>
</tr>
</table>
