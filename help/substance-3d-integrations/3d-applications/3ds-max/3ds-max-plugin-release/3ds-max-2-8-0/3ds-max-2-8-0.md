---
helpx_url: "https://helpx.adobe.com/tw/substance-3d-integrations/3d-applications/3ds-max/3ds-max-plugin-release-notes/3ds-max-2-8-0.html"
breadcrumb-title: ''
description: 查看 3ds Max 插件 2.8.0 版本的發布說明，了解新功能、改進與錯誤修正。
helpx_creative_field: ""
helpx_description: Substance 3D Integrations
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 3ds Max 2.8.0
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 0%

---


# 3ds Max 2.8.0

<b>新增/更新：
</b>

* 支援參數的條件可見性（「如果可見」）;當條件未達成時，參數將被隱藏，且其對應的群組仍可見。
* 將 Corona Renderer 升級到 3ds Max 插件中的 10 版，提升渲染能力
* 最新更新大幅提升了 3ds Max 2024 在使用 Substance 時的渲染速度與 CPU 利用率，使其效能更接近 3ds Max 2022 的效率。

<b>修正：</b>

* 強化 Substance 外掛，限制鍵盤輸入值在每個參數的實際範圍內，避免滑桿控制及手動數值調整的問題。
* 解決了一個問題：在 Slate 材質編輯器中複製 Substance2 材質轉換（.sbsar）時，導致複製節點意外實例化，可能導致與 d3d11.dll 相關的當機
* 在 3ds Max 中用 Corona Interactive 渲染自訂/編輯複製材質物質（.sbsar）時，解決了當機問題
* 已修正 3ds Max 的 Substance2 Node 中一個問題，整數 3 和 4 的滑桿無法反應，只有手動輸入數字能更新。 此外，這些數值在浮點數格式中也被錯誤顯示。 滑桿功能正常，能準確反映預期值類型。
* 解決了 3ds Max 2021 中 Corona Render 的問題，當時 Substance 材質在視窗中正確顯示，但當檔案傳輸到另一台電腦時卻呈現為灰色。 使用者不再需要從零開始設定材質或載入預設來正確渲染。
* 在嘗試在 Slate 材質編輯器中複製 Substance 節點時，解決了 3ds Max 插件當機的問題。
* 解決了 Substance 插件中 CPU 核心限制設定在重啟 3ds Max 後未被儲存的問題，導致使用者設定的數值在多個工作階段中持續存在。

此版本於 2021、2022 及 2023 年推出 3ds Max 版本
