---
title: サインイン リソースの種類
doc_type: resourcePageType
description: ユーザーとアプリケーションのサインイン アクティビティを監査するのに役立つ Microsoft Graph API (REST) のサインイン リソースについて説明します (ベータ版)。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6197600854833f7887556c35a511fad61b4539d5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965062"
---
# <a name="signin-resource-type"></a>サインイン リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

ディレクトリでのユーザーやアプリケーションのサインイン アクティビティについて詳しく説明します。 

## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[サインインを一覧表示する](../api/signin-list.md) | [サインイン](signin.md) |サインイン オブジェクトのプロパティとリレーションシップを読み取ります。|
|[サインインを取得する](../api/signin-get.md) | [サインイン](signin.md) |サインイン オブジェクトのプロパティとリレーションシップを読み取ります。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|appDisplayName|String|Azure ポータルで表示されるアプリケーション名を参照します。|
|appId|String|Azure Active Directory でのアプリケーション ID を表す一意の GUID を参照します。|
|clientAppUsed|String|サインインに使用するレガシ クライアントを示します。例: ブラウザー、Exchange Active Sync、先進認証クライアント、IMAP、MAPI、SMTP、POP が含まれます。|
|appliedConditionalAccessPolicy|[conditionalAccessPolicy](conditionalaccesspolicy.md) コレクション|対応するサインイン アクティビティでトリガーされる条件付きアクセス ポリシーの一覧を示します。|
|conditionalAccessStatus|string| トリガーされる条件付きアクセス ポリシーの状態を示します。 使用可能な値は、`success`、`failure`、`notApplied`、`unknownFutureValue` です。|
|originalRequestId|String|認証シーケンスで最初の要求の要求 ID です。|
|isInteractive|Boolean|サインインが対話型かどうかを示します。|
|tokenIssuerName|String|ID プロバイダーの名前 (例: sts.microsoft.com) |
|tokenIssuerType|String|identityProvider の種類を示します。 使用可能な値は、`AzureAD`、`ADFederationServices`、`UnknownFutureValue` です。|
|correlationId|String|サインインが開始されるときに、クライアントから送信される ID を参照します。 これは、ヘルプデスクまたはサポートに問い合わせをするときに、対応するサインイン アクティビティのトラブルシューティングに使用されます。|
|createdDateTime|DateTimeOffset|サインインが開始された日付を示します。 Timestamp 型は、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|deviceDetail|[deviceDetail](devicedetail.md)|サインインが発生した場所からデバイスの情報を提供します。 これは、deviceId、OS、ブラウザーなどの情報が含まれます。 |
|id|String|サインイン アクティビティを表す一意の ID を示します。|
|ipAddress|String|サインインが発生した場所から、クライアントの IP アドレスを提供します。|
|location|[signInLocation](signinlocation.md)|サインインが発生した場所から市区町村、都道府県、2 文字の国コードを示します。|
|processingTimeInMilliseconds|Int|要求処理時間を AD STS のミリ秒単位で示します。|
|riskDetail|`riskDetail`|リスクの高いユーザー、サインイン、リスク イベントのいずれかの特定の状態の背後にある「理由」について示します。 使用可能な値: `none`、`adminGeneratedTemporaryPassword`、`userPerformedSecuredPasswordChange`、`userPerformedSecuredPasswordReset`、`adminConfirmedSigninSafe`、`aiConfirmedSigninSafe`、`userPassedMFADrivenByRiskBasedPolicy`、`adminDismissedAllRiskForUser`、`adminConfirmedSigninCompromised`、`unknownFutureValue`。 値 `none` は、ユーザーについて実行されたアクションまたはサインインが今のところないことを意味しています。 **注:** このプロパティの詳細は、Azure AD Premium P2 のお客様のみ利用可能です。 その他のお客様には `hidden` が返されます。|
|riskLevelAggregated|`riskLevel`|集計されたリスク レベルを示します。 使用可能な値: `none`、`low`、`medium`、`high`、`hidden`、`unknownFutureValue`。 値 `hidden` は、ユーザーまたはサインインが Azure AD Identity Protection で有効になっていないことを意味します。 **注:** このプロパティの詳細は、Azure AD Premium P2 のお客様のみ利用可能です。 その他のお客様には `hidden` が返されます。|
|riskLevelDuringSignIn|`riskLevel`|サインイン時のリスク レベルを示します。 使用可能な値: `none`、`low`、`medium`、`high`、`hidden`、`unknownFutureValue`。 値 `hidden` は、ユーザーまたはサインインが Azure AD Identity Protection で有効になっていないことを意味します。 **注:** このプロパティの詳細は、Azure AD Premium P2 のお客様のみ利用可能です。 その他のお客様には `hidden` が返されます。|
|riskEventTypes|`riskEventType` コレクション|サインインに関連付けられているリスク イベントの種類の一覧を示します。 使用可能な値: `unlikelyTravel`、`anonymizedIPAddress`、`maliciousIPAddress`、`unfamiliarFeatures`、`malwareInfectedIPAddress`、`suspiciousIPAddress`、`leakedCredentials`、`investigationsThreatIntelligence`、`generic`、`unknownFutureValue`。|
|riskState|`riskState`|リスクの高いユーザー、サインイン、リスク イベントの「リスクの状態」について示します。 使用可能な値: `none`、`confirmedSafe`、`remediated`、`dismissed`、`atRisk`、`confirmedCompromised`、`unknownFutureValue`。|
|mfaDetail|[mfaDetail](mfadetail.md)|MFA が必要か、対応するサインインの MFA の状態など MFA 関連の情報を提供します。|
|networkLocationDetails|[networkLocationDetail](networklocationdetail.md) コレクション|ネットワーク上の場所について詳細を示します。|
|status|[signInStatus](signinstatus.md)|サインイン状態について示します。 使用可能な値は、`Success`、`Failure` です。|
|userDisplayName|String|ユーザーの表示名を示します。|
|userId|String|ユーザーのユーザー ID を示します。|
|userPrincipalName|String|ユーザーの UPN を示します。|
|resourceDisplayName|String|ユーザーがサインインしているリソースの名前を示します。|
|resourceId|String|ユーザーがサインインしているリソースの ID を示します。|
|authenticationMethodsUsed|String|使用される認証方法の一覧を示します|

## <a name="relationships"></a>関係
なし


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.signIn"
}-->

```json
{
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "userDisplayName": "String",
  "userPrincipalName": "String",
  "userId": "String",
  "appDisplayName": "String",
  "appId": "String",
  "ipAddress": "String",
  "clientAppUsed": "String",
  "mfaDetail": {"@odata.type": "microsoft.graph.mfaDetail"},
  "correlationId": "String",
  "conditionalAccessStatus": "string",
  "appliedConditionalAccessPolicy": [{"@odata.type": "microsoft.graph.appliedConditionalAccessPolicy"}],
  "originalRequestId": "String",
  "isInteractive": "String",
  "tokenIssuerName": "String",
  "tokenIssuerType": "String",
  "deviceDetail": {"@odata.type": "microsoft.graph.deviceDetail"},
  "location": {"@odata.type": "microsoft.graph.signInLocation"},
  "riskDetail": "string",
  "riskLevelAggregated": "string",
  "riskLevelDuringSignIn": "string",
  "riskState": "string",
  "riskEventTypes": ["String"],
  "resourceDisplayName": "string",
  "resourceId": "string",
  "authenticationMethodsUsed": "string",
  "status": {"@odata.type": "microsoft.graph.signInStatus"},
  "processingTimeInMilliseconds": 12356,
  "networkLocationDetails": [{"@odata.type": "microsoft.graph.networkLocationDetail"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "signIn resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
