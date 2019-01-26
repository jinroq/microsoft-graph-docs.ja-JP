---
title: riskyUsers リソースの種類
description: 危険にさらされている Azure AD ユーザーを表します。 Azure AD を継続的には、さまざまな信号と機械学習に基づくユーザーのリスクを評価します。 この API では、Azure の AD に問題が生じているすべてのユーザーにプログラムによるアクセスを提供します。
author: cloudhandler
localization_priority: Normal
ms.prod: security
ms.openlocfilehash: 875df6db36e4075d0d02a682ede5c177d49cfe7d
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572186"
---
# <a name="riskyusers-resource-type"></a>riskyUsers リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

危険にさらされている Azure AD ユーザーを表します。 Azure AD を継続的には、さまざまな信号と機械学習に基づくユーザーのリスクを評価します。 この API では、Azure の AD に問題が生じているすべてのユーザーにプログラムによるアクセスを提供します。

> **注:** この API には、Azure AD プレミアム P2 ライセンスが必要です。

リスク イベントの詳細については、 [Azure Active Directory Id 保護](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/)を参照してください。

## <a name="methods"></a>メソッド

| メソッド   | 戻り値の型|説明|
|:---------------|:--------|:----------|
|[リスト riskyUsers](../api/riskyusers-list.md) | [riskyUsers](riskyuser.md) |危険なユーザーとそのプロパティを一覧表示します。|
|[RiskyUsers を取得します。](../api/riskyusers-get.md) | [riskyUsers](riskyuser.md)|特定のリスクの高いユーザーとそのプロパティを取得します。|

## <a name="properties"></a>プロパティ

| プロパティ   | 型|説明|
|:---------------|:--------|:----------|
|`id`|`string`|リスクのユーザーの一意の id|
|`isDeleted`|`bool`|ユーザーを削除するかどうかを示します。 使用可能な値: `true`、`false`|
|`isGuest`|`bool`|ユーザーが guest ユーザーであるかを示します。 使用可能な値は、`true`、`false` です。 におけるテナント以外のユーザーの id が存在する場合は true。 このユーザーは、id を使用して、B2B または B2C Azure AD、MSA のまたはサード パーティの id プロバイダー。 におけるテナント内のユーザーの id が存在する場合は false。|
|`riskDetail`|`riskDetail`|危険なユーザー、サインインまたはリスク事象の特定の状態の背後にある '理由' を提供します。 可能な値: `none`、 `adminGeneratedTemporaryPassword`、 `userPerformedSecuredPasswordChange`、 `userPerformedSecuredPasswordReset`、 `adminConfirmedSigninSafe`、 `aiConfirmedSigninSafe`、 `userPassedMFADrivenByRiskBasedPolicy`、 `adminDismissedAllRiskForUser`、 `adminConfirmedSigninCompromised`、 `unknownFutureValue`。 値`none`アクションが実行されたことなしに、ユーザーまたはのサインインでこれまでにすることを意味します。|
|`riskLevel`|`riskLevel`|危険なユーザー、サインインまたはリスク事象の全体的なリスクのレベルを提供します。 可能な値: `none`、 `low`、 `medium`、 `high`、`hidden`と`unknownFutureValue`。 値`hidden`ユーザーまたはサインインが有効ではなかった Azure AD のアイデンティティ保護のことを意味します。|
|`riskState`|`riskState`|危険なユーザー、サインインまたはリスク イベントの 'リスク状態' を提供します。 使用可能な値: `none`、`confirmedSafe`、`remediated`、`dismissed`、`atRisk`、`confirmedCompromised`、`unknownFutureValue`。|
|`riskLastUpdatedDateTime`|`datetime`|危険なユーザーが最後に更新されたときの日時|
|`userDisplayName`|`string`|危険なユーザーの表示名|
|`userPrincipalName`|`string`|危険なユーザー プリンシパル名|

## <a name="relationships"></a>関係

| リレーションシップ | 型 |説明|
|:---------------|:--------|:----------|
|id|文字列| 特定のリスク イベントに関連付けられたユーザーの一意の識別子です。|
|isGuest|boolean| 危険なユーザーは、ホーム ユーザー (B2E) または (B2B、B2C) は、ゲスト ユーザーのいずれかです。|
|isDeleted|boolean| ユーザーは、可能性があります。 または削除できません。 |
|riskState|riskState| 危険なユーザーは、複数の状態のいずれかに存在でした。 |
|riskDetail|riskDetail| 危険なユーザーは複数の理由により、特定の状態にします。 |
|riskLevel|riskLevel| リスクの高いユーザーと考えられます複数のリスク レベルのいずれかです。 |

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
"isDeleted": "boolean",
"riskDetail":  {"@odata.type": "microsoft.graph.riskDetail"},
"riskLevel":  {"@odata.type": "microsoft.graph.riskLevel"},
"riskState":  {"@odata.type": "microsoft.graph.riskState"},
"userDisplayName": "string",
"userPrincipalName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "riskyusers resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/riskyuser.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
