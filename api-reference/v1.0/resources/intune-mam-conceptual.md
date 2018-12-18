---
title: Microsoft Intune で会社のアプリ データを保護する方法
description: Microsoft Intune のアプリ保護ポリシーは、会社のデータを保護し、データの損失を防ぐのに役立ちます。
author: tfitzmac
ms.openlocfilehash: d50b86b8ef1afe1cc6ddec125b3679c605979c88
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27340321"
---
# <a name="how-to-protect-your-company-app-data-with-microsoft-intune"></a>Microsoft Intune で会社のアプリ データを保護する方法

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing)を持っている必要があります。

Microsoft Intune のアプリ保護ポリシーは、会社のデータを保護し、データの損失を防ぐのに役立ちます。

Intune のアプリ保護ポリシーを使用して、会社のデータを保護することができます。 Intune のアプリ保護ポリシーは、モバイル デバイス管理 (MDM) ソリューションとは独立して使用できるため、デバイス管理ソリューションでのデバイス登録の有無に関係なく、会社のデータを保護することができます。 アプリレベルのポリシーを実装することで、会社のリソースへのアクセスを制限し、データを IT 部門の管理範囲内に維持できます。

次の Graph リソースを使用して、Intune でのアプリ保護ポリシーを管理できます。  

- [Android 管理対象アプリの保護](intune-mam-androidmanagedappprotection.md)
- [Android 管理対象アプリの登録](intune-mam-androidmanagedappregistration.md)
- [Android モバイル アプリ ID](intune-mam-androidmobileappidentifier.md)
- [アプリケーションの種類](intune-wip-applicationtype.md)
- [既定の管理対象アプリ保護](intune-mam-defaultmanagedappprotection.md)
- [iOS 管理対象アプリ保護](intune-mam-iosmanagedappprotection.md)
- [iOS 管理対象アプリの登録](intune-mam-iosmanagedappregistration.md)
- [iOS モバイル アプリ ID](intune-mam-iosmobileappidentifier.md)
- [IP 範囲](intune-mam-iprange.md)
- [IPv4 の範囲](intune-mam-ipv4range.md)
- [IPv6 の範囲](intune-mam-ipv6range.md)
- [JSON](intune-mam-json.md)
- [キー/値のペア](intune-mam-keyvaluepair.md)
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
- [管理対象アプリの状態](intune-mam-managedappstatus.md)
- [管理対象アプリの Raw 状態](intune-mam-managedappstatusraw.md)
- [管理対象モバイル アプリ](intune-mam-managedmobileapp.md)
- [MDM Windows 情報保護ポリシー](intune-mam-mdmwindowsinformationprotectionpolicy.md)
- [モバイル アプリ ID](intune-mam-mobileappidentifier.md)
- [プロキシ化されたドメイン](intune-mam-proxieddomain.md)
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
