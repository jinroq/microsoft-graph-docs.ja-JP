---
title: Intune における管理用にデバイスを登録する
description: " (BYOD) の登録では、個人の電話、タブレット、または Pc を登録することができます。 会社所有のデバイス (COD) の登録により、リモートワイプ、共有デバイス、デバイスのユーザー アフィニティなどの管理シナリオが可能になります。"
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 2e7f6e85e32137804556c64a1995bd2e78b04068
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917441"
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
- [デバイス管理 exchange コネクタの状態](intune-onboarding-devicemanagementexchangeconnectorstatus.md)
- [デバイス管理 exchange コネクタの同期の種類](intune-onboarding-devicemanagementexchangeconnectorsynctype.md)
- [デバイス管理 exchange コネクタの種類](intune-onboarding-devicemanagementexchangeconnectortype.md)
- [デバイス管理パートナー](intune-onboarding-devicemanagementpartner.md)
- [デバイス管理のパートナー アプリケーションの種類](intune-onboarding-devicemanagementpartnerapptype.md)
- [デバイス管理のパートナーのテナントの状態](intune-onboarding-devicemanagementpartnertenantstate.md)
- [有効化](intune-onboarding-enablement.md)
- [登録構成の割り当て](intune-onboarding-enrollmentconfigurationassignment.md)
- [Intune ブランド](intune-onboarding-intunebrand.md)
- [MDM 機関](intune-onboarding-mdmauthority.md)
- [モバイルの脅威保護コネクタ](intune-onboarding-mobilethreatdefenseconnector.md)
- [モバイル脅威パートナー テナントの状態](intune-onboarding-mobilethreatpartnertenantstate.md)
- [オンプレミスの条件付きアクセス設定](intune-onboarding-onpremisesconditionalaccesssettings.md)
- [組織](intune-onboarding-organization.md)
- [RGB カラー](intune-onboarding-rgbcolor.md)
- [VPP トークン](intune-onboarding-vpptoken.md)
- [VPP トークンの状態](intune-onboarding-vpptokenstate.md)
- [VPP トークンの同期の状態](intune-onboarding-vpptokensyncstatus.md)
- [Windows Hello ビジネス暗証番号 (pin) を使用するため](intune-onboarding-windowshelloforbusinesspinusage.md)
