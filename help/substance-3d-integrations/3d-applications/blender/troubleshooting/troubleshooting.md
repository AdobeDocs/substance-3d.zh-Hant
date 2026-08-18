---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/blender/troubleshooting.html"
breadcrumb-title: ''
description: 透過系統控制台診斷並解決 Blender 中 Substance 3D 附加元件的常見問題。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > Blender > Troubleshooting
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 疑難排解
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '812'
ht-degree: 0%

---


# 疑難排解

系統主控台可用於診斷使用附加元件時遇到的錯誤。 Blender 的系統主控台視窗會根據你的作業系統不同而不同地開啟。 如需詳細說明，請依照 Blender 系統主控台 [文件頁面](https://docs.blender.org/manual/en/2.79/advanced/command_line/introduction.html#console-window-status-and-error-messages)的步驟操作。 控制台輸出在遇到意外問題時很有幫助，例如材質無法載入或材質卡在處理過程中。

若要回報錯誤，請加入Substance Discord伺服器的 [#substance-blender-beta頻道，或造訪[Adobe社群](https://community.adobe.com/t5/substance-3d-plugins/ct-p/ct-substance-3d-plugins?page=1&sort=latest_replies&lang=all&tabid=all&topics=label-blender)。](https://discord.com/invite/substance3d)主控台日誌中的相關資訊及任何重複步驟可納入報告中。

## 常見問題與解決方案

* *與 WMIC 相關的控制台錯誤。*
  * *有時候 Windows 安裝時不會包含 WMIC，這種情況下是必要的。 以下是你可以手動解決的方法：*
    * 前往設定 - 系統 - 可選功能
    * 選擇「檢視功能」，再選擇「新增選項功能」
    * 這會跳出一個新視窗，往下捲動找到 WMIC，勾選勾選方塊，然後按「下一」，在下一個視窗按「新增」。
    * 你現在應該會跳到一個新視窗，顯示 WMIC 安裝在最近操作下的進度。
    * *請注意，下載可能需要幾分鐘。 之後，重啟電腦並重新啟動 Blender 和外掛。 當你點擊 Substance 3D 面板的載入時，檔案瀏覽器視窗應該會顯示出來。*
  * 如果這還是沒解決，你可能還需要在 PATH 變數中定義 WMIC。 請參考您所使用版本 Windows 的文件。
* *更新附加元件並載入材質後，並非所有設定都會出現在 Substance 3D 面板中。*
  * 這種情況可能發生在移除舊版本外掛並安裝新版本時，因為舊檔案可能仍被快取在系統中。\
    重新啟動 Blender 應該會讓這些變更生效。
* *安裝附加元件時出現問題。/ 材料在兩次會話之間卡住處理。 / 材質不會在兩次工作間產生貼圖。 / 載入 .sbsar 檔案時出現錯誤。*
  * 這可能是整合工具安裝的問題，通常透過手動移除工具即可解決。 請造訪「 [卸載附加元件](../../../3d-applications/blender/uninstalling-the-add-on/uninstalling-the-add-on.md) 」頁面，了解手動移除的步驟。
* *材質不會在 Cycles 渲染檢視*&#x200B;中更新。
  * 預設情況下，該外掛不會在 Cycles 渲染視圖中更新材質。 不過，透過在附加偏好設定中啟用 <b>Cycles 自動更新材質</b>，可以強制更新材質。
* 在 Cycles 渲染檢視中儲存後，參數似乎會回復。
  * 這是 Blender 端已知的快取問題，僅以視覺形式呈現。 儲存時，不會傳送訊息給遠端引擎更新產生的材質檔案。 離開 Cycles 渲染視圖並切回該視圖後，貼圖會恢復正常。
* *材質在撤銷或更改參數後就不再更新了。*
  * 材料在還原動作後可能會無法更新。 雖然參數會回復到先前的狀態，但貼圖不會被恢復以匹配。 要再次更新貼圖，請使用刷新按鈕將參數回復預設並重新載入貼圖。
* *Substance Designer 設定的顏色在 Blender 的色彩選擇器中呈現略有不同，且色彩值也不相同。*
  * Blender 只對顏色的 Blender 色彩選擇器套用伽瑪校正。 雖然這會導致色彩選擇器出現差異，但貼圖中出現的顏色與 Substance 應用程式設定的數值相當準確。
* *在 Windows 載入材質時出現「wmic 未被識別」的主控台錯誤。*
  * 當 C：\Windows\System32\wbem\ 未包含在 PATH 系統變數中時，會發生此問題。 請參考您所使用版本 Windows 的文件。
* *Mac 上出現「CPU 類型錯誤但可執行」錯誤。*
  * 當 ROSETTA 未在 ARM Mac 機器上啟用時，會發生此問題。 更多資訊請參閱 [蘋果的 Rosetta 頁面](https://support.apple.com/en-us/102527) 。 此外，請參閱此 [安裝指南](https://medium.com/@jithmisha/fix-for-macbook-air-m1-m2-bad-cpu-type-in-executable-error-3719a0a1cb6) 以獲得更多指示。
* *使用刷新按鈕或更新參數時，對著色器圖的修改會被撤銷。*
  * 該附加元件會在變更或刷新後刷新圖表中的連線。 為了解決這個問題，可以複製從 .sbsar 產生的 blender 素材，並取一個你選擇的新名稱。 只把你的節點加到重複的節點。 紋理會在節點群組中更新，同時保留使用者新增的節點。 重新整理時，複製這些節點並貼回新的圖表。
