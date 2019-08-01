---
title: サインイン リソースの種類
description: テナント (ディレクトリ) のユーザーおよびアプリケーションのサインインアクティビティについて説明します。
author: dhanyahk
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 735f7cc453a15ebf36aabc0e4d6a7a845a6c416c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034231"
---
# <a name="signin-resource-type"></a>サインイン リソースの種類

テナント (ディレクトリ) のユーザーおよびアプリケーションのサインインアクティビティについて説明します。

## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[サインインを一覧表示する](../api/signin-list.md) | [サインイン](signin.md) |サインイン オブジェクトのプロパティとリレーションシップを読み取ります。|
|[サインインを取得する](../api/signin-get.md) | [サインイン](signin.md) |サインイン オブジェクトのプロパティとリレーションシップを読み取ります。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|appDisplayName|String|Azure Portal に表示されるアプリ名。|
|appId|String|Azure Active Directory のアプリ ID を表す一意の GUID。|
|appliedConditionalAccessPolicy|[appliedConditionalAccessPolicy](appliedconditionalaccesspolicy.md)コレクション|対応するサインイン アクティビティでトリガーされる条件付きアクセス ポリシーの一覧を示します。|
|clientAppUsed|String|サインインアクティビティに使用されるレガシクライアントを識別します。  ブラウザー、Exchange アクティブ同期、モダンクライアント、IMAP、MAPI、SMTP、POP が含まれています。|
|conditionalAccessStatus|string| アクティブ化された条件付きアクセスポリシーの状態を報告します。 可能な値は`success`、 `failure`、 `notApplied`、、 `unknownFutureValue`です。|
|correlationId|String|サインインが開始されたときにクライアントから送信される要求 ID。サインインアクティビティのトラブルシューティングに使用されます。|
|createdDateTime|DateTimeOffset|日付と時刻 (UTC) サインインが開始されました。 例: 2014 年1月1日午前0時`'2014-01-01T00:00:00Z'`にはと報告されます。|
|deviceDetail|[deviceDetail](devicedetail.md)|サインインが発生した場所からのデバイス情報。デバイス ID、オペレーティングシステム、およびブラウザーが含まれます。 |
|id|文字列|サインインアクティビティを表す一意の ID。|
|ipAddress|String|サインインに使用されたクライアントの IP アドレス。|
|isInteractive|Boolean|サインインが対話型であるかどうかを示します。|
|location|[signInLocation](signinlocation.md)|サインインした場所の市区町村、都道府県、および国コードを提供します。|
|resourceDisplayName|String|ユーザーがサインインしたリソースの名前。|
|resourceId|String|ユーザーがサインインしたリソースの ID。|
|riskDetail|riskDetail|リスクの高いユーザー、サインイン、リスク イベントのいずれかの特定の状態の背後にある「理由」について示します。 使用可能な値: `none`、`adminGeneratedTemporaryPassword`、`userPerformedSecuredPasswordChange`、`userPerformedSecuredPasswordReset`、`adminConfirmedSigninSafe`、`aiConfirmedSigninSafe`、`userPassedMFADrivenByRiskBasedPolicy`、`adminDismissedAllRiskForUser`、`adminConfirmedSigninCompromised`、`unknownFutureValue`。 値 `none` は、ユーザーについて実行されたアクションまたはサインインが今のところないことを意味しています。 <br>**注:** このプロパティの詳細には、Azure AD Premium P2 ライセンスが必要です。 他のライセンスは値`hidden`を返します。|
|riskEventTypes|riskEventTypes|サインインに関連付けられているリスクイベントの種類。 使用可能な値: `unlikelyTravel`、`anonymizedIPAddress`、`maliciousIPAddress`、`unfamiliarFeatures`、`malwareInfectedIPAddress`、`suspiciousIPAddress`、`leakedCredentials`、`investigationsThreatIntelligence`、`generic`、`unknownFutureValue`。|
|riskLevelAggregated|riskLevel|集計リスクレベル。 使用可能な値: `none`、`low`、`medium`、`high`、`hidden`、`unknownFutureValue`。 値 `hidden` は、ユーザーまたはサインインが Azure AD Identity Protection で有効になっていないことを意味します。 **注:** このプロパティの詳細は、Azure AD Premium P2 のお客様のみ利用可能です。 その他のお客様には `hidden` が返されます。|
|riskLevelDuringSignIn|riskLevel|サインイン中のリスクレベル。 使用可能な値: `none`、`low`、`medium`、`high`、`hidden`、`unknownFutureValue`。 値 `hidden` は、ユーザーまたはサインインが Azure AD Identity Protection で有効になっていないことを意味します。 **注:** このプロパティの詳細は、Azure AD Premium P2 のお客様のみ利用可能です。 その他のお客様には `hidden` が返されます。|
|riskState|riskState|危険なユーザー、サインイン、またはリスクイベントの状態を報告します。 使用可能な値: `none`、`confirmedSafe`、`remediated`、`dismissed`、`atRisk`、`confirmedCompromised`、`unknownFutureValue`。|
|status|[signInStatus](signinstatus.md)|サインイン状態。 使用可能な値は、`Success`、`Failure` です。|
|userDisplayName|String|サインインを開始したユーザーの表示名。|
|userId|文字列型 (String)|サインインを開始したユーザーの ID。|
|userPrincipalName|String|サインインを開始したユーザーのユーザープリンシパル名。|

## <a name="relationships"></a>リレーションシップ

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
  "appDisplayName": "String",
  "appId": "String",
  "ipAddress": "String",
  "clientAppUsed": "String",
  "correlationId": "String",
  "conditionalAccessStatus": "string",
  "appliedConditionalAccessPolicy": [{"@odata.type": "microsoft.graph.appliedConditionalAccessPolicy"}],
  "isInteractive": "String",
  "deviceDetail": {"@odata.type": "microsoft.graph.deviceDetail"},
  "location": {"@odata.type": "microsoft.graph.signInLocation"},
  "riskDetail": "string",
  "riskLevelAggregated": "string",
  "riskLevelDuringSignIn": "string",
  "riskState": "string",
  "riskEventTypes": "string",
  "resourceDisplayName": "string",
  "resourceId": "string",
  "status": {"@odata.type": "microsoft.graph.signInStatus"},
  "userDisplayName": "string",
  "userId": "string",
  "userPrincipalName": "string"
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
