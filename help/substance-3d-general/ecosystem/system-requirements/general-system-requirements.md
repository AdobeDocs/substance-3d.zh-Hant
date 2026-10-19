---
helpx_url: 'https://helpx.adobe.com/tw/substance-3d-general/ecosystem/general-system-requirements.html'
breadcrumb-title: ''
description: 請檢查 Substance 3D 應用的系統需求，確保您的硬體符合最低、建議或最佳規格。
helpx_creative_field: ''
helpx_description: General Knowledge > Ecosystem > General system requirements
helpx_experience_level: ''
helpx_learn_topic: ''
helpx_tags: ''
title: 一般系統需求
user-guide-description: ''
user-guide-title: ''
source-git-commit: eef3d78f33034f2c24f4c4471d9ccac805184525
workflow-type: tm+mt
source-wordcount: '625'
ht-degree: 1%
---

# 一般系統需求

## 硬體需求

+++窗戶

|  | 最低限度 | 推薦 | 最佳 |
| --- | --- | --- | --- |
| **作業系統** | Windows 11 64 位元版本 23H2 | Windows 11 64 位元版本 24H1 | Windows 11 64 位元版本 24H2 |
| **中央處理器** | Intel Core i5 AMD Ryzen 5 | Intel Core i7 AMD Ryzen 7 | Intel Core i9 AMD Ryzen 9 |
| **GPU** | NVIDIA GeForce RTX 2060 超級 NVIDIA Quadro RTX 4000 AMD Radeon RX 5700 XT AMD Radeon Pro W5700 | NVIDIA GeForce RTX 3080、NVIDIA Quadro RTX A4000、AMD Radeon RX 6800 XT、AMD Radeon Pro W7700 | NVIDIA GeForce RTX 4090、NVIDIA Quadro RTX 5000、Ada 世代 AMD Radeon RX 7900、XTX AMD Radeon Pro W7800 |
| **VRAM** | 8 GB | 16 GB | 24 GB |
| **記憶體** | 16 GB | 32 GB | 64 GB |
| **儲存** | SSD 有 30 GB 可用空間 | SSD 有 50 GB 可用空間 | SSD 有 70 GB 可用空間 |

+++

+++macOS

|  | 最低限度 | 推薦 | 最佳 |
| --- | --- | --- | --- |
| **作業系統** | macOS 15 Sequoia | macOS 27 金門 | macOS 27 金門 |
| **中央處理器** | 蘋果 M1 | 蘋果 M2 Pro | Apple M4 Pro |
| **GPU** | 蘋果 M1 | 蘋果 M2 Pro | Apple M4 Pro |
| **記憶體** | 16 GB | 32 GB | 64 GB |
| **儲存** | SSD 有 30 GB 可用空間 | SSD 有 50 GB 可用空間 | SSD 有 70 GB 可用空間 |

>[!WARNING]
>
> 針對以 [VFX 參考平台](https://vfxplatform.com/) 為目標的管線，Substance 3D 應用程式仍可在 macOS 14 Sonoma 上安裝。 然而，Substance 應用程式不再在低於最低系統需求的作業系統版本上進行測試，因此穩定性並不保證。 建議更新到較新的作業系統版本。

+++

+++Linux

|  | 最低限度 | 推薦 | 最佳 |
| --- | --- | --- | --- |
| **作業系統** | **Enterprise ETLA** RHEL 8.6 或更新版本，或 RHEL 9.2 或更新 **版本，Steam** Ubuntu 22.04.1 LTS | **Enterprise ETLA** RHEL 8.6 或更新版本，或 RHEL 9.4 或更新 **版本，Steam** Ubuntu 22.04.1 LTS 或更新版本 | **Enterprise ETLA** RHEL 8.6 或更新版本，或 RHEL 9.4 或更新 **版本，Steam** Ubuntu 22.04.1 LTS 或更新版本 |

**Red Hat Enterprise Linux （RHEL） 9.x**：我們應用程式所需的 xcb-util-cursor 套件於 2024 年 5 月 10 日從 EPEL 9 倉庫中移除。 從此日起，該套件由預設的 RHEL 9 儲存庫支援，與 RHEL 9.4 版本同步。 使用 9.4 版本 RHEL 的客戶，將無法自 2024 年 5 月 10 日起從 EPEL 9 倉庫取得 xcb-util-cursor 套件。

如需了解此套件在預設 RHEL 9 儲存庫中的可用性，請參閱：[Red Hat Enterprise Linux 9 - 套件清單 - AppStream 儲存庫](https://access.redhat.com/documentation/en-us/red_hat_enterprise_linux/9/html-single/package_manifest/index#AppStream-repository)

關於此變更的更多資訊，請參閱： [Red Hat Bugzilla – Bug 2238273，Red](https://bugzilla.redhat.com/show_bug.cgi?id=2238273) [Hat Bugzilla – Bug 2212302](https://bugzilla.redhat.com/show_bug.cgi?id=2212302)

+++

+++VR

| 品牌 | 模型 |
| --- | --- |
| 中繼 | Rift、Rift S、Quest、Quest 2（搭配 Link）、Quest Pro |

+++

欲了解更多細節，請參閱每個申請項的要求：

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../assets/sa-appicon-noshadow-256.png" alt="Substance 3D 取樣圖示" width="64px"/><br><a href="https://experienceleague.adobe.com/zh-hant/docs/substance-3d-sampler/using/getting-started/system-requirements">Substance 3D Sampler</a></td>
    <td style="border: 0;" valign="top"><img src="../../assets/ds-appicon-noshadow-256.png" alt="Substance 3D Designer 圖示" width="64px"/><br><a href="https://experienceleague.adobe.com/zh-hant/docs/substance-3d-designer/using/getting-started/system-requirements">Substance 3D</a> <a href="https://experienceleague.adobe.com/zh-hant/docs/substance-3d-designer/using/getting-started/system-requirements">設計師</a></td>
    <td style="border: 0;" valign="top"><img src="../../assets/pt-appicon-noshadow-256.png" alt="Substance 3D Painter 圖示" width="64px"/><br><a href="https://experienceleague.adobe.com/zh-hant/docs/substance-3d-painter/using/getting-started/system-requirements">Substance 3D Painter</a></td>
  </tr>
</table>

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../assets/md-appicon-noshadow-256.png" alt="Substance 3D 建模器圖示" width="64px"/><br><a href="https://helpx.adobe.com/substance-3d-modeler/getting-started/system-requirements.html">Substance 3D 建模器</a></td>
    <td style="border: 0;" valign="top"><img src="../../assets/sg-appicon-noshadow-256.png" alt="Substance 3D Stager 圖示" width="64px"/><br><a href="https://helpx.adobe.com/substance-3d-stager/getting-started/system-requirements.html">Substance 3D Stager</a></td>
    <td style="border: 0;" valign="top"></td>
  </tr>
</table>

## 附加說明

### 不支援配置

* 蘋果電腦配置不支援搭載 eGPU 及使用者安裝的 GPU。
* 不支援 Windows 虛擬機。
* 不支援 Windows 伺服器作業系統。
