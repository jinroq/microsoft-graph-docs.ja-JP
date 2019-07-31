---
title: Intune を使用した管理対象デバイス-Microsoft Graph API
description: テナント組織用にデバイスをオンボード (構成および初期化) するために使用される Intune エンドポイント (REST) の Microsoft Graph API の一覧を示します。
localization_priority: Normal
author: rolyon
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: cc082578bea7e6b1d477547538e01dbaa1ef2bdb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35998234"
---
# <a name="enroll-devices-for-management-in-intune"></a>Intune における管理用にデバイスを登録する

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでは、これらの API の使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

デバイス (Windows PC を含む) を登録して、Microsoft Intune でモバイル デバイス管理 (MDM) を有効にすることができます。 このトピックでは、Intune 管理における、いくつかのモバイル デバイスの登録方法について説明します。 デバイスを登録する方法は、デバイスの種類、所有権、必要な管理のレベルによって異なります。 "Bring Your Own Device" (BYOD) の登録により、ユーザーは、個人の電話、タブレット、PC を登録することができます。 会社所有のデバイス (COD) の登録により、リモートワイプ、共有デバイス、デバイスのユーザー アフィニティなどの管理シナリオが可能になります。

次の Graph リソースを使用して、Intune での登録を管理できます。

- [証明書コネクタの設定](intune-onboarding-certificateconnectorsetting.md)
- [デバイスおよびアプリの管理データ](intune-onboarding-deviceandappmanagementdata.md)
- [デバイス登録の構成](intune-onboarding-deviceenrollmentconfiguration.md)
- [デバイス登録の制限の構成](intune-onboarding-deviceenrollmentlimitconfiguration.md)
- [デバイス登録プラットフォームの制限](intune-onboarding-deviceenrollmentplatformrestriction.md)
- [デバイス登録プラットフォームの制限の構成](intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)
- [デバイス登録 Windows Hello for Business の構成](intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md)
- [デバイスの管理 Exchange アクセス レベル](intune-onboarding-devicemanagementexchangeaccesslevel.md)
- [デバイスの管理 Exchange アクセス ルール](intune-onboarding-devicemanagementexchangeaccessrule.md)
- [デバイスの管理 Exchange アクセス ルールのタイプ](intune-onboarding-devicemanagementexchangeaccessruletype.md)
- [デバイスの管理 Exchange コネクタ](intune-onboarding-devicemanagementexchangeconnector.md)
- [デバイスの管理 Exchange コネクタの状態](intune-onboarding-devicemanagementexchangeconnectorstatus.md)
- [デバイスの管理 Exchange コネクタの同期タイプ](intune-onboarding-devicemanagementexchangeconnectorsynctype.md)
- [デバイスの管理 Exchange コネクタのタイプ](intune-onboarding-devicemanagementexchangeconnectortype.md)
- [デバイスの管理 Exchange デバイス クラス](intune-onboarding-devicemanagementexchangedeviceclass.md)
- [デバイスの管理 Exchange オンプレミスのポリシー](intune-onboarding-devicemanagementexchangeonpremisespolicy.md)
- [デバイス管理パートナー](intune-onboarding-devicemanagementpartner.md)
- [デバイス管理パートナー アプリの種類](intune-onboarding-devicemanagementpartnerapptype.md)
- [デバイス管理パートナー テナントの状態](intune-onboarding-devicemanagementpartnertenantstate.md)
- [登録構成の割り当て](intune-onboarding-enrollmentconfigurationassignment.md)
- [Intune ブランド](intune-onboarding-intunebrand.md)
- [MDM 機関](intune-onboarding-mdmauthority.md)
- [ビジネス向け Microsoft Store のポータル選択オプション](intune-onboarding-microsoftstoreforbusinessportalselectionoptions.md)
- [モバイルの脅威保護コネクタ](intune-onboarding-mobilethreatdefenseconnector.md)
- [モバイル脅威パートナーのテナント状態](intune-onboarding-mobilethreatpartnertenantstate.md)
- [オンプレミスの条件付きアクセス設定](intune-onboarding-onpremisesconditionalaccesssettings.md)
- [組織](intune-onboarding-organization.md)
- [サイドローディング キー](intune-onboarding-sideloadingkey.md)
- [VPP トークン](intune-onboarding-vpptoken.md)
- [VPP トークンのアクションの結果](intune-onboarding-vpptokenactionresult.md)
- [VPP トークンのライセンスの概要](intune-onboarding-vpptokenlicensesummary.md)
- [VPP トークンの失効ライセンスのアクションの結果](intune-onboarding-vpptokenrevokelicensesactionresult.md)
- [VPP トークンの状態](intune-onboarding-vpptokenstate.md)
- [VPP トークンの同期状態](intune-onboarding-vpptokensyncstatus.md)
- [Windows 10 登録完了ページの構成](intune-onboarding-windows10enrollmentcompletionpageconfiguration.md)
- [ビジネス向け Windows Hello 暗証番号 (PIN) の使用](intune-onboarding-windowshelloforbusinesspinusage.md)
