---
helpx_url: "https://helpx.adobe.com/tw/substance-3d-integrations/3d-applications/cinema-4d/visual-feedback-of-animated-substances.html"
breadcrumb-title: ''
description: 在 Cinema 4D 中啟用動畫預覽，以在視窗中看到動畫材質的視覺回饋。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > Cinema 4D > Visual Feedback of Animated Substances
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 動畫物質的視覺回饋
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '520'
ht-degree: 2%

---


# 動畫物質的視覺回饋

為了在 Cinema 4D 的視窗中獲得動畫物質的視覺回饋，應啟用這些素材的動畫預覽選項。

此選項可在素材編輯器的編輯器（見下文）中找到。 如果材質是用「建立材質」指令建立的，這個選項預設會啟用。

![](../../../assets/cinema-4d-13.png){width="500px"}


## 創作素材

利用 Substance 資產管理器中的 Create Material（建立材質）指令，你可以輕鬆快速地用 Substance 製作 Cinema 4D 材質。

因此，將使用以下通道映射：

|  |  |
| --- | --- |
| **物質輸出通道** | **Cinema 4D 素材頻道** |
| 擴散 | 顏色 |
| 發射體 | 亮度 |
| 反思 | 反射率 |
| 環境 | 環境 |
| 撞擊 | 撞擊 |
| 不透明度 | Alpha |
| 反射 | 反射率 / 預設鏡面 |
| 高度 | 置換 |
| 正常 | 正常 |

此關聯僅用於「建立材料」指令，且所建立的材料可隨後被修改。 你可能想用這個指令快速建立基底材質，然後只需微調幾個通道即可微調。

在 Substance 著色器中，你不只限於上述幾個輸出通道，事實上你可以使用任何 Substance 可能提供的輸出通道。

## 手動製作物質材料

你也可以不用 Create Material（s） 指令，也可以用 Substance shader 手動建立材質。

只要在材質通道中選擇 Substance 著色器，然後拖入你想使用的 Substance。 下一步是選擇 Substance 的輸出通道，讓它用於這個著色器，這樣就完成了。

像這樣：

![](../../../assets/cinema-4d-15.png){width="800px"}

這種方法提供了極大的創意自由，讓你能做到以下幾點：

* 將Substance的輸出通道指派到任意的Cinema 4D素材通道。 沒必要只在指定頻道使用它們。
* 將單一 Substance 輸出通道分配給多個 Cinema 4D 素材通道。
* 將多個物質的輸出通道指派到單一 Cinema 4D 材質上。

## 限制

* Substance 輸入參數的關鍵影格會在時間軸中顯示，但不會顯示在 Cinema 4D 的 Powerslider（視窗下方的時間軸滑桿）。
* 由於限制，Substance 輸出通道不得使用自訂色彩設定檔。
* 在某些情況下，Substances的影像輸入會斷開\
  Cinema 4D 的 Merge...指令，將兩個場景合併成一個。 如果要合併的場景在專案目錄中有 Substances，且圖片輸入指向專案目錄中的影像，就會發生這種情況。 在這種情況下，影像輸入必須事後手動重新連結。
* 如果物質位於專案資料夾（或全域搜尋路徑的其他地方），它們在 Cineware 中無法使用。 此時他們會被渲染成紅色，彷彿物質缺失。 為了解決這個問題，Substance 檔案需要存放在專案目錄之外，因此它們會被絕對路徑引用。 你可以用 Filename 參數來更改檔案位置，前提是檔案移出專案路徑。
