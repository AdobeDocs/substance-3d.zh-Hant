---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/renderers/keyshot.html"
breadcrumb-title: ''
description: 在 Keyshot 渲染器中使用 Substance 材質來進行產品視覺化，並匯出材質貼圖。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Renderers > Keyshot
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 關鍵射擊
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '196'
ht-degree: 7%

---


# 關鍵射擊

*Keyshot 6.1.72*[&#x200B;下載範例場景](https://www.dropbox.com/s/rvjsbbcx7c74aah/keyshot.zip?dl=0)

## 物質畫家出口

1. Keyshot 需要設定匯出預設，使用擴散、反射、金屬、粗糙度和法線（直接 X 鍵）。

   ![](https://helpx-prod.scene7.com/is/image/HelpxProd/key-01?$png$&jpegSize=300&wid=1794)

## 進階材質設定

你會用到兩種進階材料。 一個是金屬，另一個是介電質。

1. 把教材設為進階，然後把教材畫成圖表。

   **金屬色：**\
   a. 把折射率設為10\
   b. 請依照下表所示設置地圖

   | Substance Painter 材質 | 先進素材頻道 |
   | --- | --- |
   | 擴散 | 擴散 |
   | 金屬 | 不透明度 |
   | 正常 | Bump \*正常啟用 |
   | 粗糙度 | 粗糙度 |
   | 反思 | 反射 |

1. 創建新的進階教材

   **介電：**\
   a. 將折射率設為1.5\
   b. 請依照下表所示設置地圖

   | Substance Painter 材質 | 先進素材頻道 |
   | --- | --- |
   | 擴散 | 擴散 |
   | 正常 | Bump \*正常啟用 |
   | 粗糙度 | 粗糙度 |
   | 反思 | 反射 |

1. 取金屬先進材料的輸出，加到介電質先進材料的+中。 這會在素材上建立一個標籤欄位。

   ![](../../assets/key-02.png)
