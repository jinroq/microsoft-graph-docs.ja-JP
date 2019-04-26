---
title: riskyUsers リソースの種類
description: 危険にさらされている Azure AD ユーザーを表します。 Azure AD は、さまざまなシグナルやマシン学習に基づいて、ユーザーのリスクを継続的に評価します。 この API は、プログラムによって Azure AD 内のすべてのリスクユーザーにアクセスを提供します。
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 927e4eb519f8a849ac2cb259bed962bad44d9a6d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563175"
---
# <a name="riskyusers-resource-type"></a>riskyUsers リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

危険にさらされている Azure AD ユーザーを表します。 Azure AD は、さまざまなシグナルやマシン学習に基づいて、ユーザーのリスクを継続的に評価します。 この API は、プログラムによって Azure AD 内のすべてのリスクユーザーにアクセスを提供します。

リスクイベントの詳細については、「 [Azure Active Directory id 保護](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/)」を参照してください。

>**注:** riskyUsers API を使用するには、Azure AD Premium P2 ライセンスが必要です。

## <a name="methods"></a>メソッド

| メソッド   | 戻り値の型|説明|
|:---------------|:--------|:----------|
|[リスト riskyUsers](../api/riskyusers-list.md) | [riskyUser](riskyUser.md)コレクション|リスクの高いユーザーとそのプロパティを一覧表示します。|
|[riskyUser を取得する](../api/riskyusers-get.md) | [riskyUser](riskyUser.md)|特定の危険なユーザーおよびそのプロパティを取得します。|
|[riskyUsers が侵害されたことを確認する](../api/riskyusers-confirmcompromised.md)|なし |危険なユーザーが侵害されていることを確認します。|
|[riskyUsers を閉じる](../api/riskyusers-dismiss.md)|なし | 危険なユーザーのリスクを無視します。|

## <a name="properties"></a>プロパティ

| プロパティ   | 型|説明|
|:---------------|:--------|:----------|
|`id`|`string`|危険にさらされているユーザーの一意の id|
|`isDeleted`|`bool`|ユーザーが削除されるかどうかを示します。 可能な値は`true`、です。`false`|
|`isGuest`|`bool`|ユーザーがゲストユーザーであるかどうかを示します。 可能な値は、`true`、`false` です。 True の場合は、ユーザーの id がテナントの外部にある場合に考慮します。 このユーザーは、Azure AD、MSA、またはサードパーティの id プロバイダーで id を持つ B2B または B2C ユーザーの場合があります。 False 場合は、ユーザーの id がテナントの内側にある場合|
|`isProcessing`|`bool`|ユーザーの危険な状態がバックエンドによって処理されていることを示します。|
|`riskLastUpdatedDateTime`|`datetime`|危険性のあるユーザーが最後に更新された日時|
|`riskLevel`|`riskLevel`| 使用可能な値は、low、medium、high、hidden、none、unknownfuturevalue というです。  |
|`riskState`|`riskState`| 使用可能な値は、none、confirmedSafe、修復済み、atrisk、unknownfuturevalue というです。  |
|`riskDetail`|`riskDetail`| 使用可能な値は、none、adminGeneratedTemporaryPassword、userPerformedSecuredPasswordChange、userPerformedSecuredPasswordReset、adminConfirmedSigninSafe、aiConfirmedSigninSafe、userPassedMFADrivenByRiskBasedPolicy、adminDismissedAllRiskForUser、adminConfirmedSigninCompromised、hidden、adminConfirmedUserCompromised、unknownfuturevalue という。  |
|`userDisplayName`|`string`|危険ユーザーの表示名|
|`userPrincipalName`|`string`|危険ユーザープリンシパル名|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|履歴|[riskyUserHistoryItem](riskyuserhistoryitem.md)コレクション| |

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.riskyUser"
}-->

```json
{
"id": "string",
"riskLastUpdatedDateTime": "dateTimeOffset",
"isGuest": "boolean",
"isProcessing": "boolean",
"isDeleted": "boolean",
"riskDetail":  "string",
"riskLevel":  "string",
"riskState":  "string",
"userDisplayName": "string",
"userPrincipalName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "riskyusers resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
