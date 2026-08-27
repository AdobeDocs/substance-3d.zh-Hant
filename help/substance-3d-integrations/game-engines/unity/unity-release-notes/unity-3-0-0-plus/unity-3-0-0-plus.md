---
helpx_url: "https://helpx.adobe.com/tw/substance-3d-integrations/game-engines/unity/unity-release-notes/unity-3-0-0-plus.html"
breadcrumb-title: ''
description: 請參閱 Unity 外掛 3.0.0 及以上版本的發佈說明，了解新功能與改進。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Unity Release Notes > Unity 3.0.0
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Unity 3.0.0
user-guide-description: ''
user-guide-title: ''
source-git-commit: 4a060ee1aaa1731c04e70d5512e3271cd63d0381
workflow-type: tm+mt
source-wordcount: '1384'
ht-degree: 0%

---


# Unity 3.0.0+

## Unity 3.12.0

<b>新增/更新：</b>

* Unity 支援 Substance 3D 連接器，使 SendTo 功能能在 Substance 3D 取樣器與 Unity 之間傳送資產。
* 支援將 .sbsar 圖形從 Designer 重新命名並重新發布到 Unity 中，確保在更新的圖形重新匯入 Unity 外掛時，Designer 中的變更依然存在。
* Unity 專案間分享 .sbsar 檔案的文件。
* Unity 外掛文件的社群貢獻頁面：https://helpx.adobe.com/substance-3d-integrations/game-engines/unity/community-contributions.html。

<b>修正：</b>

* Unity 專案資產資料夾中的材質迷你模型在重新發布 .sbsar 檔案後不會更新，顯示的是之前的材質而非目前的資料。

## Unity 3.11.0

<b>新增/更新：</b>

* 提升了擁有 1000+ Substance 圖表的專案效能，顯著縮短了 UI 在 Assets 資料夾中檢查 sbsar 檔案時的回應時間。
* 新增了重置按鈕，可將 sbsar 檔案還原至原始狀態，提升工作流程效率。
* 更新的文件中包含解決「影像輸入鎖定於 8 位元」問題的解決方法，可於以下網站取得： [Substance 3D 整合於 Unity - 升級專案與已知問題](../../../../game-engines/unity/upgrading-projects-known/upgrading-projects-known-issues.md)。
* 更新文件以解決在 Unity 面板資料夾中瀏覽時遇到的「陳述失敗」錯誤： [Unity 中的 Substance 3D 整合 - 升級專案與已知問題](../../../../game-engines/unity/upgrading-projects-known/upgrading-projects-known-issues.md)。

<b>修正：</b>

* 修正了導致外掛在 Linux 平台上故障的問題。
* 已修正 2023 版本 Unity 外掛的相容性問題。

## Unity 3.10.1

<b>修正：</b>

* 修正了 Substance Engine 因 Substance 3D for Unity 插件的 sbsario.dll 問題而無法載入的問題。

## Unity 3.10.0

<b>新增/更新：</b>

* 更新了外掛中 RenderInstanceAsync API 的註解區

<b>修正：</b>

* 解決了外掛 C++ 程式碼中的記憶體洩漏問題，確保物件丟棄後能完全恢復記憶體。
* 已修正 Linux 上匯入 Unity 外掛套件時出現「SubstanceException： A invalid argument to the API」錯誤，現在允許成功匯入 SBSAR 檔案。
* 解決了 SubstanceGraphSO.CurrentStatePreset 在 Unity 中用自訂編輯器視窗腳本載入預設時無法正常運作的問題;現在我們的 Substance 文件（HelpX）頁面有修正腳本：https://experienceleague.adobe.com/zh-hant/docs/substance-3d/ecosystem/game-engines/unity/substance-3d-for-unity-scripting/substance-3d-for-unity-scripting
* 修正了一個在 Unity 編輯器重新選取圖屬性時會消失的錯誤。
* 解決了 Unity 外掛中 SubstanceGraphSO 相關的「未知受管理型別參考」問題，提升了 Android 平台的相容性與功能性，特別是針對 Unity 2022.1，並有可能適用於所有 Unity 版本。
* 修正了技術參數區塊中「NORMAL FORMAT」選項錯誤顯示為數字輸入欄位的問題，而非預期的下拉選單，並包含 DirectX 和 OpenGL 選項。

## Unity 3.9.0

<b>新增/更新：</b>

* SBSAR 檔案現在可以拖放到專案中。 .sbsar 物件可以在 Unity 2022.3 中如預期套用到網格上。
* 插件的強化說明文件。

<b>修正：</b>

* 修正了 Unity 插件在 Android 上無法使用的問題。
* 解決了 Unity 外掛的命名限制。 當檔名包含「.」時，外掛無法正確載入該檔案。
* 修正了一個問題，就是取消勾選「產生所有輸出」並不會自動刪除多餘的貼圖。
* 已修正 Unity 2021.3 標準專案中 SBSAR 材質的錯誤匯入問題。 現在，在標準模板專案中，SBSAR 材質可以匯入 assets 資料夾並套用到 3D 網格上，且不會出錯。
* 已修正 Unity 2021/2022 HDRP 專案中錯誤匯入 SBSAR 材質的問題。 現在，在 HDRP 模板專案中，SBSAR 材質可以匯入 assets 資料夾，並套用到 3D 網格上，且不會出錯。
* 修正了產生 Android 版本以產生 APK 時的編譯錯誤：「編譯失敗;詳情請參閱編譯器錯誤輸出。」
* 修正了導致 Windows 建置專案流程錯誤失敗的問題。
* 已修正 Android 上導致建置專案失敗且錯誤的問題：UnityEditor.BuildPlayerWindow+BuildMethodException。
* 解決了執行時變更 SubstanceGraph 輸入時遇到的 UnityException 問題。 過去，呼叫 SubstanceRuntimeGraph.SetTexturesResolution 與 SubstanceRuntimeGraph.Render（） 會導致 SubstanceGraph 產生錯誤結果。
* SubstanceEditorTools.cs 修正了印刷錯誤。

## Unity 3.8.0

<b>新增/更新：</b>

* 新增了具備條件可見性的參數支援（Visible If 功能）。
* 將Substance引擎升級到第9版。
* 更新文件以解決 NativeGraph.InRenderWork 在自訂編輯器視窗腳本中無法運作的問題。 更多細節可在此處查閱： [Substance 3D for Unity Scripting - 類別文件](../../../../game-engines/unity/3d-for-unity-scripting/class-documentation/substanceruntime-class/substanceruntime-class.md)

<b>修正：</b>

* 解決了 Android 專案中影響法線貼圖的問題。
* 已修正一個錯誤，當將 SBSAR 物件拖入場景視圖時，所有滑鼠懸停物件的材質都被 SBSAR 物件材質覆蓋。
* 修正了一個錯誤，該錯誤在檢查標記為僅執行時的材質，並開啟輸出貼圖映射時會出錯。

## Unity 3.7.0

<b>新增/更新：</b>

* 支援嵌入式及外部預設
* 與 Unity 2022.2 的相容性

<b>修正：</b>

* 使用 copy graph 按鈕為 sbsar 檔案建立新圖時出現錯誤：「腳本類別的意外遞迴傳輸」
* 在 Mac 上重新開啟專案後建立額外的材料資料夾
* SubstanceFileSO 陣列在建立/刪除圖實例時無法更新
* 複製物質時會顯示錯誤輸入選項
* .sbsprs 檔案匯出中的空標籤欄位
* 在編輯器 EndLayoutGroup： BeginLayoutGroup 預設匯出/匯入時，必須先呼叫錯誤。

<b>已移除：</b>

* 由於用戶價值不足，來自 Unity 外掛的頻道區塊

## Unity 3.6.0

<b>新增/更新：</b>

* 能夠讓個別 Int 4 值獨立編輯。

<b>修正：</b>

* 一個問題，當重新開啟專案時，材料會回復到先前的狀態
* 嘗試修改材料圖時會顯示「找不到任何圖表」的錯誤訊息
* 一個問題是 Physical Size 功能中旋轉偏移參數的輸入值沒有改變
* 重複的圖形實例輸入值錯誤的問題
* 一個問題是 Substance 產生器在編輯器中使用編輯器腳本（自訂編輯器視窗）更改圖表時，初始化時無法正確初始化
* 一個問題：從自訂編輯器視窗腳本匯出 SubstanceGraphSO.CurrentStatePreset 時，匯出了快取版本的圖表
* 一個參數變更在檢查器視窗鎖定時無法儲存的問題
* 一個問題是，在實體尺寸選項的「位置偏移」區段手動鍵盤輸入，對編輯器模式下的材質沒有任何影響
* 在手動輸入 SBSAR 物件參數值時發生的錯誤

## Unity 3.5.0

<b>新增/更新：</b>

* 支援使用者更改輸出材質對 Unity 材質的指派方式
* 與最新 Unity 2022.2 版本的外掛相容性

<b>修正：</b>

* 當材料有 Int4 輸入時，空參考誤差
* 錯誤：Int4 輸入時，W 值會被分配給 Data2，而非 Data3
* 函式名稱「\_OcclusionStrength」 中的打字錯誤

## Unity 3.4.0

<b>新增/更新：</b>

* 位置偏移控制，用來在物理尺寸面板中將貼圖移到表面
* 在專案設定中下載 Adobe Substance 3D 資產與 Substance Community 資產的連結

## Unity 3.3.0

<b>新增/更新：</b>

* HDRP 的實體尺寸特性，允許根據材料的實際尺寸進行貼布與縮放
* 專案設定中的 GPU 啟用介面

<b>已移除：</b>

* 大多數 API 呼叫的 graphID

## Unity 3.2.1

<b>修正：</b>

* 將外掛從 3.0.0 和 3.1.0 升級到最新版本的問題。

## Unity 3.2.0

<b>新增/更新：</b>

* 腳本重新編譯的效能提升

<b>修正：</b>

* 在 Unity 插件匯入自訂 Sbsar 材質時，資產匯入失敗
* 「ArgumentException： Value 不在預期範圍內」錯誤
* 「ArgumentOutOfRangeException： Index was out of range」錯誤

## Unity 3.1.0

<b>新增/更新：</b>

* Mac 效能提升 1.38 倍
* Mac 的 GPU 引擎使用 Metal 而非 OpenGL

<b>修正：</b>

* Mac 的問題是輸出材質的 R 聲道和 B 聲道會被翻轉

## Unity 3.0.0

<b>新增/更新：</b>

* Apple Silicon 支援
* 新的 YouTube 教學，教你如何使用這個插件
* 新的腳本文件

<b>修正：</b>

* 反覆按隨機按鈕時，檢查器顯示會出現錯誤
* Null 材質輸入破壞 Substance 更新
* 「產生所有輸出」、「產生 MIP 映射」和「僅執行時」切換功能無法運作
* 命名空間的問題
* 進入遊玩模式並選取圖形資產時，會出現空參考錯誤
* 使用僅執行時材質時，最新 2021.3 LTS 版本 Unity 的 HDRP 與 URP 問題
