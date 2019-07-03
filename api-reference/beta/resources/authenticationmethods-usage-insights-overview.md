---
title: 認証方法の利用状況レポート API を使用する
description: '[認証方法] 利用状況レポートを使用すると、セルフサービスのパスワードのリセットや多要素認証 (MFA) など、エンドユーザーが Azure Active Directory の機能をどのように使用しているかを把握することができます。'
author: davidmu1
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 19f99b0909a762201ea91399125bba841d705338
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35504181"
---
# <a name="working-with-the-authentication-methods-usage-report-api"></a>認証方法の利用状況レポート API を使用する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

認証方法の利用状況レポートは、組織内のユーザーが Azure Active Directory (Azure AD) 機能を使用する方法を理解するのに役立ちます。これには、セルフサービスのパスワードの rest や多要素認証 (MFA) などがあります。

これらのレポートは、次のような情報を提供します。

- 組織にとって、どの認証方法が成功するか。 
- エンドユーザーが実行しているエラーの種類。
- エンドユーザーがセルフサービスのパスワード rest と MFA の使用を採用できるようにするために実行する必要のあるキャンペーン。

## <a name="common-requests"></a>一般的な要求

次の表に、この API で使用できる一般的な要求の一覧を示します。

| Operation | Graph エクスプローラーで試します | 説明 |
| --------- | --- | ----------- |
| [getCredentialUserRegistrationcount](/graph/api/resources/credentialUserRegistrationCount?view=graph-rest-beta) | [/Credentialuserregistrationcount の取得](https://developer.microsoft.com/graph/graph-explorer?request=reports/getCredentialUserRegistrationcount()&version=beta) | セルフサービスのパスワードのリセットと MFA に登録されているユーザーの数を取得します。 |
| [getCredentialUsageSummary](/graph/api/resources/credentialUsagesSummary?view=graph-rest-beta) | [/Credentialusagesummary を取得する](https://developer.microsoft.com/graph/graph-explorer?request=reports/getCredentialUsageSummary&version=beta) | セルフサービスのパスワードのリセットを使用してユーザーの数を取得します。 |
| [credentialUserRegistrationDetails](/graph/api/resources/credentialUserRegistrationDetails?view=graph-rest-beta) | [/Credentialuserregistrationdetails の取得](https://developer.microsoft.com/graph/graph-explorer?request=reports/credentialUserRegistrationDetails&version=beta) | セルフサービスのパスワードのリセットと MFA の登録アクティビティに関するユーザーの詳細を取得します。 |
| [Usercredentialの詳細](/graph/api/resources/userCredentialUsageDetails?view=graph-rest-beta) | [/Usercredentialusagedetails を取得する](https://developer.microsoft.com/graph/graph-explorer?request=reports/userCredentialUsageDetails&version=beta) | すべてのセルフサービスのパスワードリセットアクティビティのユーザー詳細を取得します。 |

## <a name="licenses"></a>ライセンス

利用状況レポートは、セルフサービスのパスワードのリセットとテナントでの MFA を利用するライセンス機能で利用できます。

## <a name="next-steps"></a>次のステップ

- [Azure Active Directory のセルフサービスのパスワードのリセットを展開](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-deployment)する方法について説明します。
- [Azure Active DIRECTORY MFA](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-getstarted)を展開する方法について説明します。
- 統合された[セキュリティ情報登録](https://docs.microsoft.com/azure/active-directory/authentication/howto-registration-mfa-sspr-combined)を有効にする方法について説明します。



