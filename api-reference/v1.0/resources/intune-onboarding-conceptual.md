---
title: Intune における管理用にデバイスを登録する
description: " (byod) の登録では、ユーザーは自分の携帯電話、タブレット、または pc を登録できます。 会社所有のデバイス (COD) の登録により、リモートワイプ、共有デバイス、デバイスのユーザー アフィニティなどの管理シナリオが可能になります。"
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 2e7f6e85e32137804556c64a1995bd2e78b04068
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32564240"
---
# <a name="enroll-devices-for-management-in-intune"></a>Intune における管理用にデバイスを登録する

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing)を持っている必要があります。

デバイス (Windows PC を含む) を登録して、Microsoft Intune でモバイル デバイス管理 (MDM) を有効にすることができます。 このトピックでは、Intune 管理における、いくつかのモバイル デバイスの登録方法について説明します。 デバイスを登録する方法は、デバイスの種類、所有権、必要な管理のレベルによって異なります。 "Bring Your Own Device" (BYOD) の登録により、ユーザーは、個人の電話、タブレット、PC を登録することができます。 会社所有のデバイス (COD) の登録により、リモートワイプ、共有デバイス、デバイスのユーザー アフィニティなどの管理シナリオが可能になります。

次の Graph リソースを使用して、Intune での登録を管理できます。  

- [デバイス登録の構成](intune-onboarding-deviceenrollmentconfiguration.md)
- [デバイス登録の制限の構成](intune-onboarding-deviceenrollmentlimitconfiguration.md)
- [デバイス登録プラットフォームの制限](intune-onboarding-deviceenrollmentplatformrestriction.md)
- [デバイス登録プラットフォームの制限の構成](intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)
- [デバイス登録 Windows Hello for Business の構成](intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md)
- [デバイスの管理 Exchange コネクタ](intune-onboarding-devicemanagementexchangeconnector.md)
- [デバイスの管理 Exchange コネクタの状態](intune-onboarding-devicemanagementexchangeconnectorstatus.md)
- [デバイスの管理 Exchange コネクタの同期タイプ](intune-onboarding-devicemanagementexchangeconnectorsynctype.md)
- [デバイスの管理 Exchange コネクタのタイプ](intune-onboarding-devicemanagementexchangeconnectortype.md)
- [デバイス管理パートナー](intune-onboarding-devicemanagementpartner.md)
- [デバイス管理パートナー アプリの種類](intune-onboarding-devicemanagementpartnerapptype.md)
- [デバイス管理パートナー テナントの状態](intune-onboarding-devicemanagementpartnertenantstate.md)
- [有効化](intune-onboarding-enablement.md)
- [登録構成の割り当て](intune-onboarding-enrollmentconfigurationassignment.md)
- [Intune ブランド](intune-onboarding-intunebrand.md)
- [MDM 機関](intune-onboarding-mdmauthority.md)
- [モバイルの脅威保護コネクタ](intune-onboarding-mobilethreatdefenseconnector.md)
- [モバイル脅威パートナーのテナント状態](intune-onboarding-mobilethreatpartnertenantstate.md)
- [オンプレミスの条件付きアクセス設定](intune-onboarding-onpremisesconditionalaccesssettings.md)
- [組織](intune-onboarding-organization.md)
- [RGB カラー](intune-onboarding-rgbcolor.md)
- [VPP トークン](intune-onboarding-vpptoken.md)
- [VPP トークンの状態](intune-onboarding-vpptokenstate.md)
- [VPP トークンの同期状態](intune-onboarding-vpptokensyncstatus.md)
- [ビジネス向け Windows Hello 暗証番号 (PIN) の使用](intune-onboarding-windowshelloforbusinesspinusage.md)
