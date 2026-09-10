---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/blender/preferences.html"
breadcrumb-title: ''
description: 在 Blender 中設定 Substance 3D 附加偏好設定，以自訂外掛行為與設定。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > Blender > Preferences
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 偏好設定
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '845'
ht-degree: 0%

---


# 偏好設定

附加偏好設定可以在 Blender 的偏好設定視窗中找到。 請前往編輯>偏好設定>外掛，搜尋 Node： Adobe Substance 3D 外掛（用於 Blender）。

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

![附加偏好設定選單的前半段。](../../../assets/blender-prefs-1.png)

</td>
<td style="border: 0;" valign="top">

![附加偏好選單的後半段。](../../../assets/blender-prefs-2-b.png)

</td>
</tr>
</table>

<b>卸載</b> - 從系統刪除該附加元件，並從 Blender 的附加元件清單中移除。

<b>回報錯誤</b> - 開啟 Substance 3D 的 Blender Discord。

<b>接受工具資料夾</b> - 開啟 Blender 檔案瀏覽器，選擇 Substance Integration Tools 的安裝路徑。

<b>開啟工具 </b>- 在整合工具資料夾位置開啟系統檔案瀏覽器。

<b>重置路徑</b> - 將整合工具資料夾路徑重設為預設位置。

<b>卸載工具</b> - 移除已安裝版本的 Substance 3D 整合工具。

<b>更新工具</b> - 開啟檔案瀏覽器以選取工具的壓縮檔並更新工具。

<b>文件</b> - 在瀏覽器中開啟生態系統與插件文件頁面。

<b>論壇</b> - 在瀏覽器中開啟 Adobe 社群論壇。

<b>Discord 伺服器</b> - 在瀏覽器中開啟生態系統並外掛 Discord 伺服器。

<b>鋪</b> 磚——調整材料的X、Y、Z鋪磚。 鎖可以用來解除連結並分別調整這些數值。

<b>解析度</b> ——生成材質的預設解析度。 鎖可用來解除連結，分別設定它們的解析度。

<b>套用類型 </b>- 設定套用按鈕的行為： <b>插入 </b>會用選取的物質材質覆蓋目前材質， <b>而附加</b>則會將材質加入物件的新材質槽。

<b>匯出影像格式</b> - 當 Blender 產生的影像作為 Substance 材質的影像輸入時，此格式會用來將該影像儲存到時間資料夾中。

<b>輸入群組預設</b>會收合——切換 Substance 材質的輸入群組是否展開或收合。

<b>預設</b>只更新材質——切換天氣更新 Substance 參數只影響 Blender Shading 網路中的輸出材質。 關閉此功能後，調整參數後會重置節點連線。 建議在新增材質節點時啟用，否則調整參數後這些節點會被斷開。

<b>物質遠端引擎 </b>- 設定物質遠端引擎所使用的硬體。

<b>自動套用材質</b> - 當物質材質建立時，自動將材質附加到選取的物件上，並設置新的材質槽。

<b>自動高亮選取物件的</b>材質 - 若選取含有該材質的物件，請在 Substance 3D 面板中更改該高亮材質。

<b>Cycles 自動更新材質</b> - 在使用 Cycles 渲染視圖時，強制在 3D 視口中更新材質。

<b>移除預設刪除確認</b> - 移除刪除材質預設時出現的確認視窗。

<b>建立啟用假使用者</b>的資料 - 設定素材是啟用或停用「假使用者」的。 標記為假使用者的 Blender 資料即使未被使用，關閉後也不會被清除。

<b>自動啟動 Substance Remote Engine </b>- 如果 Substance Remote Engine 在 Blender 啟動時已被初始化，則會切換。 若停用，遠端引擎僅在使用者讀取按鈕或使用載入捷徑時啟動。

>[!NOTE]
>
> 注意：若使用 Substance Connector，必須啟用 SRE 才能讓發送應用程式偵測 Blender 作為端點。

<b>SBSAR 函式庫路徑</b> - 當讀取按鈕搜尋物質檔案時，預設會開啟的資料夾。

<b>暫存資料夾 </b>- 這個資料夾會是檔案第一次儲存前，貼圖會先儲存的預設位置。

<b>儲存時</b>複製 .sbsar 檔案 - 啟用時，.sbsar 檔案會被複製到指定的相對路徑。 這有助於裝置間的專案共享。

<b>儲存時，將貼圖複製到</b>——當檔案第一次被儲存時，暫存資料夾中的貼圖會被複製到這個位置。 $matname 變數用於為每種材料建立子資料夾。

<b>著色器預設</b> - 設定從 Materials 檔案建立 Blender 材質時使用的預設著色器預設。 可設定為基於 UV 的映射標準，或為基於箱體、球體與圓柱投影的投影。

<b>中階</b>位移 - 預設值是位移節點中位移的基礎值。 高於預設值會將表面向外推，低於預設值則會將表面往內拉。

<b>位移刻度</b>-位移節點的預設刻度值。

<b>發射強度</b>-原理BSDF節點中發射強度的預設值。

<b>投影混合</b> - 設定投影方法著色器角度間的混合量。

<b>AO Mix</b> - 當輸出啟用環境遮蔽時，這個值決定了 MixRGB 節點的預設因子值，該節點用於結合基色與環境遮蔽紋理。

<b>輸出</b> - 材料的個別輸出可以啟用或停用。 預設的色彩空間、檔案格式及個別輸出的色深也可以調整。

<b>捷徑 </b>- 自訂用來開啟浮動選單、載入物質材質及套用當前材質的快捷鍵。 捷徑更新需要重新啟動才能生效。
