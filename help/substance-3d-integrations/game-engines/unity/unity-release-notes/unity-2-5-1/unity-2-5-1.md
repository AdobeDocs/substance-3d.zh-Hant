---
helpx_url: "https://helpx.adobe.com/tw/substance-3d-integrations/game-engines/unity/unity-release-notes/unity-2-5-1.html"
breadcrumb-title: ''
description: 請查看 Unity 外掛 2.5.1 版本的發布說明，了解新功能、改進與錯誤修正。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Unity Release Notes > Unity 2.5.1
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Unity 2.5.1
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '246'
ht-degree: 0%

---


# Unity 2.5.1

2020年5月21日發行

新增內容

* 通用渲染管線支援：Substance 材質會自動使用 URP 著色器和材質

固定

* Substance CPU 引擎最大解析度設定：
  * 在 Substance 設定選單中將欄位名稱從「Texture Clamp \*\*」更新為「Substance CPU Engine Max Resolution」。
  * 當設定修改時，會顯示警告通知，表示所有物質材料將重新匯入
* 移除安裝時顯示的不必要除錯訊息（「TextureClamp = 4096 Unity.Engine.Debug:Log（Object）」）
* HDRP 專案：標準與 HDRP 材料中同時存在的材料特性，當包含 Substances 的包裝進口時，將持續使用
* 當從 Unity 版本中的 Substance 套件匯入 Substance 材質時，反射與 HDRP 遮罩會如預期般產生並運作
* 重複物質材質會是預期顏色，使用複製功能時不再是黃色
* Substance Source 在關閉並重新開啟 Unity 後會如預期載入
* 在將套件匯入 HDRP 專案時（間歇性地）當機
* 對於 Substance 材質，使用曝光參數且編輯器設定為 Color（灰階）時，滑桿功能正常
* 點擊「將預設預設」與沒有預設解析度的 Substance 圖表時會當機
* 當物質材料的輸出大小改變且輸出大小參數未被暴露時，當崩潰
* 為 iOS 建置不會失敗
* 使用 Substance 材質的腳本在為 Windows 獨立程式建置時會執行
