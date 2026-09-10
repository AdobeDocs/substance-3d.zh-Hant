---
helpx_url: "https://helpx.adobe.com/tw/substance-3d-integrations/3d-applications/blender/release-notes/add-on-0-9-3/add-on-2-0-0-plus.html"
breadcrumb-title: ''
description: 請參閱 Blender 附加元件 2.0.0 版及以上版本的發布說明，以了解新功能與改進。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > Blender > Release Notes > Add-on 2.0.0
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 附加元件 2.0.0
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '738'
ht-degree: 0%

---


# 附加元件 2.0.0+

## 附加元件 2.2

<b>補充：</b>

* 對 Octane 渲染器的支援
* 對 Redshift 的初步支援
* 對 Renderman 的初期支援

<b>更新：</b>

* 升級至最新版本的 Connector
* 新增使用 Connector 接收預設功能
* 強化匯入預設功能：現在所有包含該材質的 SBSAR 實例都會新增預設
* 標準化連接器功能

<b>修正：</b>

* 儲存混合檔案後輸入圖片無法運作的持久性錯誤
* 更新著色器預設時著色器網路無法運作的問題
* 下載外掛按鈕的網址錯誤
* Octane中的倒置鋪磚
* 使用第三方渲染器的輸入值失效
* 未建立浮點點輸入值參數的問題
* Renderman 色彩空間運作不正常
* 著色器預設沒有依可用渲染器過濾

## 附加元件 2.1.1

此更新包含對 Blender 4.0+ 的支援，以及附加元件偏好設定中的多項新功能。 我們也新增了 Substance Connector 支援，能無縫在 Substance 3D Sampler 與 Blender 之間傳輸資料（傳送到），並修正了一些錯誤。 請參閱下方詳細的發行說明。

<b>新增/更新：</b>

* 新增 Substance Connector 功能（支援 SBSAR 檔案與 USD 檔案）。
* 支援 Blender 4.0+。
* 支援 SRE 2.1.0 版本。
* 附加元件偏好設定：
  * 能夠選擇 Substance Integration Tools 的安裝路徑。
  * 按鈕將整合工具重置為預設路徑。
  * 按鈕開啟整合工具資料夾。
  * 新增 Apply 類型來指派材料（插入：設定為主要素材，Append：將它加入清單底部）。
  * 新增了選擇輸入群組預設行為的核取方塊（摺疊/展開）。
  * 新增了選擇「唯一更新材質」屬性預設行為的勾選框。
  * 開啟 Blender 時自動啟動 Substance Remote Engine（使用 Connector 時啟用很重要）。
* 附加內容：
  * 新增：僅更新貼圖（允許更改參數而無需重新製作節點圖）。
  * 新增了展開所有群組和摺疊所有群組按鈕。
  * 新增輸入影像群組，以便在 SBSAR 中需要時將所有輸入影像分組。
  * 參數輸入現在與 Designer 的順序相同。
  * 新增了每種Substance素材的縮圖預覽。

<b>修正：</b>

* 已修正空 General 輸入群組的錯誤。

<b>已知問題：</b>

* 目前選擇物件時自動選擇 SBSAR 的功能無法運作，因此已被停用。

## 附加元件 2.0.0

Substance 3D Addon 2.0 對 Blender 使用者來說是一項變革性的更新，採用完全重構的外掛架構。 這次重新設計著重於無縫整合、提升效能，以及為未來擴展提供靈活基礎。 這不僅是升級，更是對 Blender 中 Substance 材質處理方式的重新想像，以滿足 3D 專業人士不斷演變的需求。

<b>2.0 版本亮點：</b>

* 重構架構 — 改良插件結構以提升效能與整合度
* 未來擴充支援——這次更新為未來輕鬆新增功能奠定基礎
* 更廣泛的相容性 – 完全相容於 Blender 3.0 及以上版本，並支援 Mac 用戶

<b>新增/更新：</b>

* [SRE]物質引擎選擇支援（GPU 為預設）
* [SRE]新的影像格式以匯出材質
* [SRE]每種映射類型的位元深度選擇
* [BLD]價值輸出支援
* [BLD]字串輸入支援
* [SRE]新增選擇預設暫存資料夾的選項，作為影像匯出目的地

<b>修正：</b>

* [SRE]整體績效提升
* [BLD]修正了整合工具與 Blender 之間的通訊問題
* [BLD]整合工具無法安裝/啟動
* [無聲無聞]整合工具在關閉 Blender 時不會停止
* [BLD]更改地圖檔案類型時，材質未更新
* [SRE]所有材料的地圖都會一直被輸出
* [SRE]積分工具 匯出帶有階梯步進的法線貼圖
* [SRE]物質負荷永遠不會結束
* [SRE]實體尺寸單位不會根據現場調整
* [BLD]Blender 產生的預設無法與其他整合相容
* [BLD]素材在週期中不會更新
* [BLD]輸入的軟限制與硬限制被忽略
* [BLD]調整參數時色彩強度未正確更新
* [SRE]整合工具卸載失敗
* [SRE]我們已經修正了多次重複材料會出錯的問題。
* [SRE]影像節點的色彩空間現在能正確符合使用者偏好。

<b>已知問題：</b>

* 使用 Blender v4.0+ 時，啟用和停用多次後插槽順序不正確
* Cltr+Z 來還原變更可能會造成錯誤
* 載入空檔或資料夾而非 .sbsar 檔案可能會破壞外掛
* 支援 Blender 無頭模式
