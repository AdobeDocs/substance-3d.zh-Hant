---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/blender/release-notes/blender-add-on-2-0-0.html"
breadcrumb-title: ''
description: 查看 Blender 附加元件 2.0.0 版本的發布說明，了解新功能、改進與錯誤修正。
helpx_creative_field: ""
helpx_description: Substance 3D Integrations
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 附加元件 2.0.0
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 0%

---


# 附加元件 2.0.0

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
