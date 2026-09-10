---
helpx_url: "https://helpx.adobe.com/tw/substance-3d-bake/getting-started/software-interface/substance-3d-designer.html"
breadcrumb-title: ''
description: 學習如何存取並使用Substance 3D Designer中的烘焙視窗，將模型資訊烘焙到貼圖中。
helpx_creative_field: ""
helpx_description: bakers > Getting Started > Software Interface > Substance 3D Designer
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Substance 3D Designer
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '496'
ht-degree: 1%

---


# Substance 3D Designer

![](../../../assets/sd-mesh-right-click.png)

烘焙視窗可以透過檔案總管[&#128279;](https://helpx.adobe.com/tw/substance-3d/unlisted/documentation/sddoc/the-explorer-129368147.html)視窗中的網格檔案進入。右鍵點擊網格名稱，選擇「**烘焙模型資訊**」以開啟烘焙視窗。

## 概觀

![](../../../assets/sd-window-overview.png){width="500px"}

烘焙窗口分為數個面板，以下將說明。

### 元素烘焙

![](../../../assets/sd-mesh-selection.png)

這個面板控制低多邊形網格的哪一部分將用於烘焙。

這個面板會列出低多邊形網格檔案內的幾何體。 預設情況下，列表是根據檔案中發現的個別材質，但當需要時，也可以切換到子網格。 你可以取消勾選烘焙過程中應該忽略的元素。

### 輸出

![](../../../assets/sd-output.png)

這個面板控制烘焙貼圖的位置。

| *參數* | *描述* |
| --- | --- |
| **方法** | 控制烘焙後的貼圖如何與 Substance 套件一起儲存。可能的數值：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Embedded</strong> ：烘焙的貼圖會儲存在 Substance 套件旁邊的子資料夾中，並有特定命名。</li><li data-preserve-html="true"><strong>連結</strong> （預設）：烘焙的貼圖會儲存在定義的資料夾中，然後再被引用到打包的 Substance 中。</li></ul> |
| **資料夾** | 儲存後烘焙材質的位置。 點擊三點按鈕開啟檔案對話框並選擇匯出資料夾。右側會有一個勾選標記，用來表示該資料夾是否真實存在。 |
| **名稱** | 烘焙材質的命名慣例。 點擊三點按鈕打開下拉選單，並插入其他佔位符（烘焙名稱、自訂、材質、網格）。 |
| **範例** | 模擬一個檔名來測試命名慣例。 |
| **將資源放入特定網格的資料夾** | 啟用後，烘焙的材質會儲存在一個名為網格檔案的資料夾中。 |

### 高解析度網格

![](../../../assets/sd-high.png)

這個面板控制高多邊形網格列表及相關設定。 更多資訊請參閱 [常見參數](../../../bakers-settings/common-parameters/common-parameters.md) 。

### 預設值

![](../../../assets/sd-default-values.png)

更多資訊請參閱 [常見參數](../../../bakers-settings/common-parameters/common-parameters.md) 。

### 烘焙清單與設定

![](../../../assets/sd-baker-list.png)

烘焙師是你可以選擇想要產生哪種烘焙紋理的地方。 預設情況下，清單是空的。

* **新增烘焙師：** 點擊「新增烘焙師」按鈕。
* **移除烘焙師：** 在列表中選擇烘焙師，然後點擊「刪除烘焙師」按鈕。
* **將烘焙師移到頂部：** 在列表中選擇烘焙師，然後點擊「拉到頂部」按鈕。
* **向下移動烘焙師：**&#x200B;在列表中選擇烘焙師，然後點擊「向下推」按鈕。

每個烘焙師預設繼承預設值（見上文）。 例如，點擊烘焙師行中的儲存格即可覆蓋大小（解析度）。 這點對線上其他設定也適用。

點擊清單中的烘焙器時，烘焙者參數檢視會更新其特定參數。

欲了解更多具體參數，請參閱： [Bakers 設定](../../../bakers-settings/bakers-settings.md)。
