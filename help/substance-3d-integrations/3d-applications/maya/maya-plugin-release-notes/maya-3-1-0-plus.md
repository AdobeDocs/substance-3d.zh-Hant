---
description: 檢視 Maya 外掛 3.0.0 及以後版本的發行說明，了解新功能、改進與錯誤修正。
title: Maya 3.0.0
source-git-commit: 28a9d8cf7a4eed4163f99e8158c9cb8f9da88302
workflow-type: tm+mt
source-wordcount: '223'
ht-degree: 0%
---

# Maya 3.1.0+

## Maya 3.1.1

**發行日期：** 2026 年 11 月 18 日

**相容於：** Maya 2025 及更新版本

### 新增/更新

* Substance Engine 更新（9.6.1.） 包含安全修補
* Maya 2025、2026 與 2027（Arnold 與 V-Ray）的 OpenPBR 支援

### 已知限制

* 排放權重：emission_weight 參數不屬於 OpenPBR 1.1 規範，且不會自動連接。 套用工作流程後，若材料使用排放，請手動在 OpenPBR 節點設定排放重量值。
* OpenPBR - V-Ray — 次表面半徑縮放：使用 OpenPBR - V-Ray 工作流程時，subsurface_radius_scale 可能會回傳 0 值。 若發生此情況，請移除連線並在 V-Ray 節點中手動設定該值。
* 渲染器間的視覺差異：Substance 3D Designer 中材質預覽與 Arnold 或 V-Ray 渲染結果的部分差異，是由於各渲染器對 OpenPBR 規範的實作不同，隨著實作趨同，情況會有所改善。
* 從 Substance 3D Painter 12.2.0 匯出的 SBSAR 檔案。 或更早版本在使用 OpenPBR 工作流程時可能無法正確連線。新增/更新：Substance Engine 更新（9.6.1.） 包括安全修正。

## Maya 3.1.0

**發行日期：** 2026 年 11 月 18 日

**相容於：** Maya 2024

### 新增/更新

* Substance Engine 更新（9.6.1.） 包含安全修補
