---
title: Microsoft Intune で会社のアプリ データを保護する方法
description: Microsoft Intune のアプリ保護ポリシーは、会社のデータを保護し、データの損失を防ぐのに役立ちます。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ca628b81015527cb5ab7e508bebbb2808cdcde7e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27925456"
---
# <a name="how-to-protect-your-company-app-data-with-microsoft-intune"></a>Microsoft Intune で会社のアプリ データを保護する方法

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing)を持っている必要があります。

Microsoft Intune のアプリ保護ポリシーは、会社のデータを保護し、データの損失を防ぐのに役立ちます。

Intune のアプリ保護ポリシーを使用して、会社のデータを保護することができます。 Intune アプリケーションの保護ポリシーを使用するすべてのモバイル デバイス管理 (MDM) ソリューションに依存しないために、デバイス管理ソリューションに登録するデバイスの有無にかかわらず、会社のデータを保護するために使用できます。 アプリレベルのポリシーを実装することで、会社のリソースへのアクセスを制限し、データを IT 部門の管理範囲内に維持できます。

次の Graph リソースを使用して、Intune でのアプリ保護ポリシーを管理できます。

- [Android 管理対象アプリの保護](intune-mam-androidmanagedappprotection.md)
- [Android 管理対象アプリの登録](intune-mam-androidmanagedappregistration.md)
- [Android モバイル アプリ ID](intune-mam-androidmobileappidentifier.md)
- [アプリケーション管理のレベル](intune-mam-appmanagementlevel.md)
- [アプリケーションの種類](intune-wip-applicationtype.md)
- [既定の管理対象アプリ保護](intune-mam-defaultmanagedappprotection.md)
- [Intune ブランドのプロファイル](intune-wip-intunebrandingprofile.md)
- [iOS 管理対象アプリ保護](intune-mam-iosmanagedappprotection.md)
- [iOS 管理対象アプリの登録](intune-mam-iosmanagedappregistration.md)
- [iOS モバイル アプリ ID](intune-mam-iosmobileappidentifier.md)
- [JSON](intune-mam-json.md)
- [アプリケーションのクリップボード共有機能レベルの管理](intune-mam-managedappclipboardsharinglevel.md)
- [管理対象アプリの構成](intune-mam-managedappconfiguration.md)
- [アプリケーション データの暗号化の種類を管理](intune-mam-managedappdataencryptiontype.md)
- [管理されているアプリケーション データの格納場所](intune-mam-managedappdatastoragelocation.md)
- [管理されているアプリケーション データの転送レベル](intune-mam-managedappdatatransferlevel.md)
- [管理対象アプリの診断状態](intune-mam-managedappdiagnosticstatus.md)
- [マネージ アプリケーションのフラグを設定した理由](intune-mam-managedappflaggedreason.md)
- [管理対象アプリの操作](intune-mam-managedappoperation.md)
- [暗証番号 (pin) のマネージ アプリケーションの文字セット](intune-mam-managedapppincharacterset.md)
- [管理対象アプリ ポリシー](intune-mam-managedapppolicy.md)
- [管理対象アプリ ポリシーの展開の概要](intune-mam-managedapppolicydeploymentsummary.md)
- [アプリごとの管理対象アプリ ポリシーの展開の概要](intune-mam-managedapppolicydeploymentsummaryperapp.md)
- [管理対象アプリ保護](intune-mam-managedappprotection.md)
- [管理対象アプリの登録](intune-mam-managedappregistration.md)
- [マネージ アプリケーションの修復操作](intune-mam-managedappremediationaction.md)
- [管理対象アプリの状態](intune-mam-managedappstatus.md)
- [管理対象アプリの Raw 状態](intune-mam-managedappstatusraw.md)
- [管理対象モバイル アプリ](intune-mam-managedmobileapp.md)
- [MDM Windows 情報保護ポリシー](intune-mam-mdmwindowsinformationprotectionpolicy.md)
- [モバイル アプリ ID](intune-mam-mobileappidentifier.md)
- [対象となる管理対象アプリの構成](intune-mam-targetedmanagedappconfiguration.md)
- [対象となる管理対象アプリ ポリシーの割り当て](intune-mam-targetedmanagedapppolicyassignment.md)
- [対象となる管理対象アプリの保護](intune-mam-targetedmanagedappprotection.md)
- [Windows 情報保護](intune-mam-windowsinformationprotection.md)
- [Windows 情報保護アプリ](intune-mam-windowsinformationprotectionapp.md)
- [Windows 情報保護アプリの学習概要](intune-wip-windowsinformationprotectionapplearningsummary.md)
- [Windows 情報保護アプリの Locker ファイル](intune-mam-windowsinformationprotectionapplockerfile.md)
- [Windows 情報保護のデータ回復証明書](intune-mam-windowsinformationprotectiondatarecoverycertificate.md)
- [Windows 情報保護のデスクトップ アプリ](intune-mam-windowsinformationprotectiondesktopapp.md)
- [Windows 情報保護の適用レベル](intune-mam-windowsinformationprotectionenforcementlevel.md)
- [Windows 情報保護の IP 範囲のコレクション](intune-mam-windowsinformationprotectioniprangecollection.md)
- [Windows 情報保護のネットワークの学習概要](intune-wip-windowsinformationprotectionnetworklearningsummary.md)
- [Windows 情報保護暗証番号 (pin) の文字の要件](intune-mam-windowsinformationprotectionpincharacterrequirements.md)
- [Windows 情報保護ポリシー](intune-mam-windowsinformationprotectionpolicy.md)
- [Windows 情報保護のプロキシ化されたドメイン コレクション](intune-mam-windowsinformationprotectionproxieddomaincollection.md)
- [Windows 情報保護のリソース コレクション](intune-mam-windowsinformationprotectionresourcecollection.md)
- [Windows 情報保護ストア アプリ](intune-mam-windowsinformationprotectionstoreapp.md)
