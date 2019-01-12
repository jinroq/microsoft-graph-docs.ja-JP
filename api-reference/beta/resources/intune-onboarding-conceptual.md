---
title: Intune における管理用にデバイスを登録する
description: " (BYOD) の登録では、個人の電話、タブレット、または Pc を登録することができます。 会社所有のデバイス (COD) の登録により、リモートワイプ、共有デバイス、デバイスのユーザー アフィニティなどの管理シナリオが可能になります。"
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 895977194822918fc2ac61ed13e0aae938a25166
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27923748"
---
# <a name="enroll-devices-for-management-in-intune"></a>Intune における管理用にデバイスを登録する

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing)を持っている必要があります。

デバイス (Windows PC を含む) を登録して、Microsoft Intune でモバイル デバイス管理 (MDM) を有効にすることができます。 このトピックでは、Intune 管理における、いくつかのモバイル デバイスの登録方法について説明します。 デバイスを登録する方法は、デバイスの種類、所有権、必要な管理のレベルによって異なります。 "Bring Your Own Device" (BYOD) の登録により、ユーザーは、個人の電話、タブレット、PC を登録することができます。 会社所有のデバイス (COD) の登録により、リモートワイプ、共有デバイス、デバイスのユーザー アフィニティなどの管理シナリオが可能になります。

次の Graph リソースを使用して、Intune での登録を管理できます。

- [証明書のコネクタの設定](intune-onboarding-certificateconnectorsetting.md)
- [デバイスとアプリケーションの管理データ](intune-onboarding-deviceandappmanagementdata.md)
- [デバイス登録の構成](intune-onboarding-deviceenrollmentconfiguration.md)
- [デバイス登録の制限の構成](intune-onboarding-deviceenrollmentlimitconfiguration.md)
- [デバイス登録プラットフォームの制限](intune-onboarding-deviceenrollmentplatformrestriction.md)
- [デバイス登録プラットフォームの制限の構成](intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)
- [デバイス登録 Windows Hello for Business の構成](intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md)
- [デバイス管理 exchange のアクセス レベル](intune-onboarding-devicemanagementexchangeaccesslevel.md)
- [デバイス管理 exchange のアクセス ルール](intune-onboarding-devicemanagementexchangeaccessrule.md)
- [デバイス管理 exchange アクセス規則の種類](intune-onboarding-devicemanagementexchangeaccessruletype.md)
- [デバイスの管理 Exchange コネクタ](intune-onboarding-devicemanagementexchangeconnector.md)
- [デバイス管理 exchange コネクタの状態](intune-onboarding-devicemanagementexchangeconnectorstatus.md)
- [デバイス管理 exchange コネクタの同期の種類](intune-onboarding-devicemanagementexchangeconnectorsynctype.md)
- [デバイス管理 exchange コネクタの種類](intune-onboarding-devicemanagementexchangeconnectortype.md)
- [デバイス管理 exchange デバイス クラス](intune-onboarding-devicemanagementexchangedeviceclass.md)
- [デバイス管理の交換設置のポリシー](intune-onboarding-devicemanagementexchangeonpremisespolicy.md)
- [デバイス管理パートナー](intune-onboarding-devicemanagementpartner.md)
- [デバイス管理のパートナー アプリケーションの種類](intune-onboarding-devicemanagementpartnerapptype.md)
- [デバイス管理のパートナーのテナントの状態](intune-onboarding-devicemanagementpartnertenantstate.md)
- [登録構成の割り当て](intune-onboarding-enrollmentconfigurationassignment.md)
- [Intune ブランド](intune-onboarding-intunebrand.md)
- [MDM 機関](intune-onboarding-mdmauthority.md)
- [ビジネス ポータルの選択オプションのマイクロソフト ストア](intune-onboarding-microsoftstoreforbusinessportalselectionoptions.md)
- [モバイルの脅威保護コネクタ](intune-onboarding-mobilethreatdefenseconnector.md)
- [モバイル脅威パートナー テナントの状態](intune-onboarding-mobilethreatpartnertenantstate.md)
- [オンプレミスの条件付きアクセス設定](intune-onboarding-onpremisesconditionalaccesssettings.md)
- [組織](intune-onboarding-organization.md)
- [側のロード キー](intune-onboarding-sideloadingkey.md)
- [VPP トークン](intune-onboarding-vpptoken.md)
- [VPP トークン処理結果](intune-onboarding-vpptokenactionresult.md)
- [VPP トークン ライセンスの概要](intune-onboarding-vpptokenlicensesummary.md)
- [VPP トークンの取り消しライセンスのアクションの結果](intune-onboarding-vpptokenrevokelicensesactionresult.md)
- [VPP トークンの状態](intune-onboarding-vpptokenstate.md)
- [VPP トークンの同期の状態](intune-onboarding-vpptokensyncstatus.md)
- [Windows 10 登録の完了] ページの構成](intune-onboarding-windows10enrollmentcompletionpageconfiguration.md)
- [Windows Hello ビジネス暗証番号 (pin) を使用するため](intune-onboarding-windowshelloforbusinesspinusage.md)
