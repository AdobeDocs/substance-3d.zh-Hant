---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/maya/substance-in-maya-overview.html"
breadcrumb-title: ""
description: 了解 Maya 的 Substance 外掛，以及如何匯入和在工作流程中使用 Substance 材質。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > Maya > Substance in Maya Overview
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Maya 中的實質概覽
user-guide-description: ""
user-guide-title: ""
source-git-commit: 28a9d8cf7a4eed4163f99e8158c9cb8f9da88302
workflow-type: tm+mt
source-wordcount: '433'
ht-degree: 0%
---

# Maya 中的實質概覽

## 外掛程式概覽

Substance for Maya 外掛程式允許您直接載入任何現有的 Substance 3D 材質（。SBSAR 檔案）在 Maya 中。 Substance 3D 材質可從 Substance 3D Designer 或 Substance 3D Sampler 撰寫並匯出為 SBSAR 檔案，亦可從現有函式庫（如 Substance 3D 資產庫）下載。 Substance for Maya 外掛程式會建立 Maya 材質，並將輸出材質輸入到正確的材質通道輸入

>[!NOTE]
>
> 請確認您在設定/偏好設定中已載入該外掛 ->Maya 外掛管理員

## 在 Hypershade 節點編輯器中開啟 SBSAR 檔案

1. 開啟 **Hypershade**，在節點編輯器&#x200B;**中**，在標記選單中右鍵點擊並向上滑動，選擇&#x200B;**建立節點**。在建立 **節點視窗**&#x200B;中，搜尋並選取「 **Substance」節點**。

   ![](../../../assets/createnode.png)

   在 Hypershade 中點擊 **Substance 節點** 以選取它。 這會開啟 **材質編輯器**，您可以點擊資料夾圖示載入您的 Substance 3D 材質（SBSAR 檔案）。

1. 或者，您也可以將 SBSAR 檔案拖放到 Maya **的 Hypershade 編輯器**&#x200B;中，然後點擊自動建立的 Substance 節點，直接檢視並編輯材質編輯器&#x200B;**中的**&#x200B;選項。

### 在屬性編輯器中調整 SBSAR 參數

![](../../../assets/1.png)

1. **若 Substance 包含多個圖表，則會顯示「已選取圖表」下拉選單**。選擇要使用哪張圖表來建立材質。

1. **「圖譜資訊」按鈕**&#x200B;會顯示在 Substance Designer 中設定的圖屬性。

1. 透過設定 **寬度** 與 **高度** 來設定解析度。 停用 **鎖定比率** 以選擇非方形比例。

1. 啟用 **快取輸出到磁碟** ，將 Substance 輸出烘焙到磁碟，以便搭配像 Arnold 這樣的渲染器使用。 快取的檔案會由外掛透過 Maya 檔案節點重新讀取。

   ![](../../../assets/outputsettings.png)

1. 選擇您所使用的渲染器工作流程，然後點擊「 **建立著色器網路」按鈕**。 為渲染器工作流程建立一個著色器網路。 在 3.1.1. 版本中，工作流程清單也提供建立 OpenPBR 著色器網路的選項。 一旦著色器網路建立好，你就可以在場景中套用材質。

   ![](../../../assets/createnetwork.gif){width="1000px"}

## 疑難排解

若要回報錯誤，請加入 Substance Discord 伺服器的 [&#128279;](https://discord.com/invite/substance3d)#maya-plugin 頻道，或造訪 [Adobe 社群](https://community.adobe.com/t5/substance-3d-plugins/ct-p/ct-substance-3d-plugins?page=1&sort=latest_replies&lang=all&tabid=all&topics=label-autodesk3dsmax)。將主控台日誌中的相關資訊及任何重現步驟納入，將有助於我們更有效率地診斷問題。