---
title: Intune を使用して会社のデバイスを登録する-Microsoft Graph API
description: テナント組織のデバイスを登録する Intune エンドポイント (REST) の Microsoft graph API の一覧を示します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4b4100265797fd3cefc60e0288961b74839199c2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32573922"
---
# <a name="enroll-corporate-owned-devices-by-using-intune"></a>Intune を使用して会社所有のデバイスを登録する

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing)を持っている必要があります。

組織所有または会社所有のデバイスを登録して、デバイスの種類、デバイスの購入方法、組織のニーズに応じて、さまざまな方法で Intune で管理することができます。 また、ポータル サイト アプリをインストールして、会社所有のデバイスの登録と管理を、"Bring Your Own Device" (BYOD) のようなシナリオで行うこともできます。

次の Graph リソースを使用して、Intune での会社所有のデバイスを管理できます。

- [Active Directory Windows Autopilot 展開プロファイル](intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md)
- [Azure AD Windows Autopilot 展開プロファイル](intune-enrollment-azureadwindowsautopilotdeploymentprofile.md)
- [DEP 登録ベース プロファイル](intune-enrollment-depenrollmentbaseprofile.md)
- [DEP 登録プロファイル](intune-enrollment-depenrollmentprofile.md)
- [DEP iOS 登録プロファイル](intune-enrollment-depiosenrollmentprofile.md)
- [DEP macOS 登録プロファイル](intune-enrollment-depmacosenrollmentprofile.md)
- [DEP オンボード設定](intune-enrollment-deponboardingsetting.md)
- [DEP トークンの種類](intune-enrollment-deptokentype.md)
- [探索ソース](intune-enrollment-discoverysource.md)
- [登録プロファイル](intune-enrollment-enrollmentprofile.md)
- [登録状態](intune-enrollment-enrollmentstate.md)
- [インポートしたアップル デバイス ID](intune-enrollment-importedappledeviceidentity.md)
- [インポートしたアップル デバイス ID の結果](intune-enrollment-importedappledeviceidentityresult.md)
- [インポートしたデバイス ID ](intune-enrollment-importeddeviceidentity.md)
- [インポートしたデバイス ID の結果](intune-enrollment-importeddeviceidentityresult.md)
- [インポートしたデバイス ID のタイプ](intune-enrollment-importeddeviceidentitytype.md)
- [インポートした Windows AutoPilot デバイス ID](intune-enrollment-importedwindowsautopilotdeviceidentity.md)
- [インポートした Windows AutoPilot デバイス ID のインポート状態](intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)
- [インポートした Windows AutoPilot デバイス ID の状態](intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)
- [インポートした Windows AutoPilot デバイス ID のアップロード](intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)
- [インポートした Windows AutoPilot デバイス ID のアップロードの状態](intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)
- [iTunes ペアリング モード](intune-enrollment-itunespairingmode.md)
- [拇印を含む証明書の管理](intune-enrollment-managementcertificatewiththumbprint.md)
- [Out Of Box Experience の設定](intune-enrollment-outofboxexperiencesettings.md)
- [プラットフォーム](intune-enrollment-platform.md)
- [Windows Autopilot 展開プロファイル](intune-enrollment-windowsautopilotdeploymentprofile.md)
- [Windows AutoPilot Deployment プロファイルの割り当て](intune-enrollment-windowsautopilotdeploymentprofileassignment.md)
- [Windows AutoPilot デバイス ID](intune-enrollment-windowsautopilotdeviceidentity.md)
- [Windows AutoPilot デバイスの種類](intune-enrollment-windowsautopilotdevicetype.md)
- [Windows Autopilot プロファイルの割り当ての状態の詳細](intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)
- [Windows Autopilot プロファイルの割り当ての状態](intune-enrollment-windowsautopilotprofileassignmentstatus.md)
- [Windows Autopilot の設定](intune-enrollment-windowsautopilotsettings.md)
- [Windows AutoPilot の同期状態](intune-enrollment-windowsautopilotsyncstatus.md)
- [Windows デバイスの使用法の種類](intune-enrollment-windowsdeviceusagetype.md)
- [Windows 登録ステータス画面の設定](intune-enrollment-windowsenrollmentstatusscreensettings.md)
- [Windows ユーザーの種類](intune-enrollment-windowsusertype.md)
