---
title: Intune を使用して会社所有のデバイスを登録する
description: " (BYOD) のシナリオです。"
ms.openlocfilehash: b6c498a1471b95f28c26fb035eec3349108e1ec3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072565"
---
# <a name="enroll-corporate-owned-devices-by-using-intune"></a>Intune を使用して会社所有のデバイスを登録する

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing)を持っている必要があります。

組織所有または会社所有のデバイスを登録して、デバイスの種類、デバイスの購入方法、組織のニーズに応じて、さまざまな方法で Intune で管理することができます。 また、ポータル サイト アプリをインストールして、会社所有のデバイスの登録と管理を、"Bring Your Own Device" (BYOD) のようなシナリオで行うこともできます。

次の Graph リソースを使用して、Intune での会社所有のデバイスを管理できます。

- [Active directory windows 自動操縦装置の配置のプロファイル](intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md)
- [Azure AD windows 自動操縦装置の配置のプロファイル](intune-enrollment-azureadwindowsautopilotdeploymentprofile.md)
- [DEP の登録の基本プロファイル](intune-enrollment-depenrollmentbaseprofile.md)
- [DEP 登録プロファイル](intune-enrollment-depenrollmentprofile.md)
- [DEP iOS 登録プロファイル](intune-enrollment-depiosenrollmentprofile.md)
- [DEP macOS 登録プロファイル](intune-enrollment-depmacosenrollmentprofile.md)
- [DEP の採用の設定](intune-enrollment-deponboardingsetting.md)
- [DEP のトークンの種類](intune-enrollment-deptokentype.md)
- [法的証拠開示要求](intune-enrollment-discoverysource.md)
- [登録プロファイル](intune-enrollment-enrollmentprofile.md)
- [登録状態](intune-enrollment-enrollmentstate.md)
- [インポートされた Apple のデバイス id](intune-enrollment-importedappledeviceidentity.md)
- [Apple デバイス識別情報の結果のインポート](intune-enrollment-importedappledeviceidentityresult.md)
- [インポートされたデバイスの識別情報](intune-enrollment-importeddeviceidentity.md)
- [デバイス識別情報の結果のインポート](intune-enrollment-importeddeviceidentityresult.md)
- [デバイス id の種類をインポート](intune-enrollment-importeddeviceidentitytype.md)
- [インポートされた windows の自動操縦装置のデバイス id](intune-enrollment-importedwindowsautopilotdeviceidentity.md)
- [インポートされた windows 自動操縦装置のデバイス id のインポート状態](intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)
- [インポートされた windows 自動操縦装置のアイデンティティの状態](intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)
- [インポートされた windows 自動操縦装置のデバイス識別情報のアップロード](intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)
- [インポートされた windows 自動操縦装置のデバイス id アップロード状態](intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)
- [iTunes ペアリング モード](intune-enrollment-itunespairingmode.md)
- [拇印を含む証明書を管理](intune-enrollment-managementcertificatewiththumbprint.md)
- [ボックス エクスペリエンスの設定](intune-enrollment-outofboxexperiencesettings.md)
- [プラットフォーム](intune-enrollment-platform.md)
- [Windows 自動操縦装置の配置のプロファイル](intune-enrollment-windowsautopilotdeploymentprofile.md)
- [Windows 自動操縦装置の配置のプロファイル割り当て](intune-enrollment-windowsautopilotdeploymentprofileassignment.md)
- [Windows 自動操縦装置のデバイス id](intune-enrollment-windowsautopilotdeviceidentity.md)
- [Windows 自動操縦装置のプロファイルの割り当てステータスの詳細](intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)
- [Windows 自動操縦装置のプロファイルの割り当ての状態](intune-enrollment-windowsautopilotprofileassignmentstatus.md)
- [Windows の自動操縦装置の設定](intune-enrollment-windowsautopilotsettings.md)
- [Windows 自動操縦装置の同期の状態](intune-enrollment-windowsautopilotsyncstatus.md)
- [Windows デバイスの使用法の種類](intune-enrollment-windowsdeviceusagetype.md)
- [Windows の登録ステータス画面の設定](intune-enrollment-windowsenrollmentstatusscreensettings.md)
- [Windows ユーザーの種類](intune-enrollment-windowsusertype.md)
