---
title: サインイン リソースの種類
description: 'このリソースは、ユーザーまたはアプリケーションにサインイン活動、ディレクトリ内を詳しく説明します。 '
ms.openlocfilehash: 2bc6c8b961f0626a6409d9be868235f285f48e52
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073340"
---
# <a name="signin-resource-type"></a>サインイン リソースの種類
このリソースは、ユーザーまたはアプリケーションにサインイン活動、ディレクトリ内を詳しく説明します。 

## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[リストのサイン](../api/signin-list.md) | [サイン](signin.md) |サイン オブジェクトのプロパティと関係を参照してください。|
|[サインインを取得します。](../api/signin-get.md) | [サイン](signin.md) |サイン オブジェクトのプロパティと関係を参照してください。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|appDisplayName|String|Azure ポータルに表示されるアプリケーション名を参照します。|
|appId|文字列型 (String)|Azure Active Directory 内のアプリケーションの Id を表す一意の GUID を参照します。|
|authenticationProcessingDetails|`authenticationProcessingDetails`|認証プロセッサに関連付けられている詳細情報を提供します。|
|clientAppUsed|String|Activty.E.g サインインに使用されるレガシ クライアントを提供します。 ブラウザー、作業中の同期を Exchange、IMAP、MAPI、SMTP、POP の最近のクライアントが含まれています。|
|appliedConditionalAccessPolicy|[conditionalAccessPolicy](conditionalaccesspolicy.md)コレクション|対応する記号の活動によってトリガーされる条件付きのアクセス ポリシーの一覧を示します。|
|conditionalAccessStatus|文字列| トリガーの条件付きのアクセス ポリシーのステータスを提供します。 可能な値は、`success`、`failure`、`notApplied`、`unknownFutureValue` です。|
|originalRequestId|String|認証シーケンス内の最初の要求の要求 id です。|
|isInteractive|ブール値|サインインがインタラクティブかどうかを示します。|
|tokenIssuerName|String|Id プロバイダー (例えば sts.microsoft.com) の名前|
|tokenIssuerType|String|IdentityProvider の種類を提供します。 使用可能な値は、 `AzureAD`、 `ADFederationServices`、 `UnknownFutureValue`。|
|correlationId|String|サインインが開始されると、クライアントから送信される ID を参照します。 ヘルプ デスクやサポートを呼び出すときに、対応する記号の活動をトラブルシューティングに使用されます。|
|createdDateTime|DateTimeOffset|サインインが開始されたときの日時を提供します。 タイムスタンプ型が、常に UTC 時刻です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|deviceDetail|[deviceDetail](devicedetail.md)|サインインが発生した場所からデバイス情報を提供します。 DeviceId、OS、ブラウザーのように inclules の情報です。 |
|id|String|サインインの活動を表す一意の ID を示します。|
|ipAddress|文字列型 (String)|サインインが発生した場所からクライアントの IP アドレスを提供します。|
|location|[signInLocation](signinlocation.md)|市区町村、都道府県、およびサインインが発生した場所から 2 文字の国コードを提供します。|
|processingTimeInMilliseconds|整数型 (Int)|AD の STS でのミリ秒単位の時間の処理要求を提供します。|
|riskDetail|`riskDetail`|危険なユーザー、サインインまたはリスク事象の特定の状態の背後にある '理由' を提供します。 可能な値: `none`、 `adminGeneratedTemporaryPassword`、 `userPerformedSecuredPasswordChange`、 `userPerformedSecuredPasswordReset`、 `adminConfirmedSigninSafe`、 `aiConfirmedSigninSafe`、 `userPassedMFADrivenByRiskBasedPolicy`、 `adminDismissedAllRiskForUser`、 `adminConfirmedSigninCompromised`、 `unknownFutureValue`。 値`none`アクションが実行されたことなしに、ユーザーまたはのサインインでこれまでにすることを意味します。|
|riskLevelAggregated|`riskLevel`|集約されたリスクのレベルを提供します。 可能な値: `none`、 `low`、 `medium`、 `high`、`hidden`と`unknownFutureValue`。 値`hidden`ユーザーまたはサインインが有効ではなかった Azure AD のアイデンティティ保護のことを意味します。|
|riskLevelDuringSignIn|`riskLevel`|サインイン中に、リスクのレベルを提供します。 可能な値: `none`、 `low`、 `medium`、 `high`、`hidden`と`unknownFutureValue`。 値`hidden`ユーザーまたはサインインが有効ではなかった Azure AD のアイデンティティ保護のことを意味します。|
|riskEventTypes|`riskEventTypes`|記号に関連付けられているリスク イベントの種類の一覧を提供します。 可能な値: `none`、 `adminGeneratedTemporaryPassword`、 `userPerformedSecurePasswordChange`、 `userPerformedSecuredPasswordReset`、 `adminConfirmedSigninSafe`、 `aiConfirmedSigninSafe`、 `userPassedMFADrivenByRiskBasedPolicy`、 `adminDismissedAllRiskForUser`、 `adminConfirmedSigninCompromised`、`hidden`と`unknownFutureValue`。 値`hidden`ユーザーまたはサインインが有効ではなかった Azure AD のアイデンティティ保護のことを意味します。|
|riskState|`riskState`|危険なユーザー、サインインまたはリスク イベントの 'リスク状態' を提供します。 可能な値: `none`、 `confirmedSafe`、 `remediated`、 `dismissed`、 `atRisk`、 `confirmedCompromised`、 `unknownFutureValue`。|
|mfaDetail|[mfaDetail](mfadetail.md)|関連する MFA を提供情報が必要な MFA、MFA の状態に対応する記号のようにします。|
|networkLocationDetail|[networkLocationDetail](networklocationdetail.md)|ネットワーク上の場所に関する詳細情報を提供します。|
|riskLevel|文字列| 記号に関連付けられているリスクのレベルを提供します。使用可能な値: `low`、 `medium`、 `high`。|
|status|[signInStatus](signinstatus.md)|サインイン状態を提供します。 可能な値は`Success`と`Failure`。|
|userDisplayName|String|表示、ユーザーの名前を示します。|
|userId|String|ユーザーのユーザー Id を示します。|
|userPrincipalName|String|ユーザーの UPN を指定します。|
|resourceDisplayName|String|ユーザーが署名されているリソースの名前を示します|
|resourceId|文字列型 (String)|ユーザーが署名されているリソースの Id を示します。|
|authenticationMethodsUsed|String|使用される認証方法の一覧を示します|

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
  "riskLevel": "string",
  "status": {"@odata.type": "microsoft.graph.signInStatus"},
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