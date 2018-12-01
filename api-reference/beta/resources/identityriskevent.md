---
title: identityRiskEvent リソースの種類
description: Azure Active Directory アイデンティティ保護によって検出されたリスク イベントです。 特定のリスク イベントの種類ごとの基本型です。
ms.openlocfilehash: e61f5e0dc2dae2c055636e3fd3737e16b2558458
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068167"
---
# <a name="identityriskevent-resource-type"></a>identityRiskEvent リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

[Azure Active Directory アイデンティティ保護](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/)によって検出されたリスク イベントです。 特定のリスク イベントの種類ごとの基本型です。

| イベントの種類         | 説明|
|:---------------|:-----------|
|[anonymousipRiskEvent](anonymousipriskevent.md) | 匿名の IP アドレスからサインインの問題です。 |
|[malwareRiskEvent](malwareriskevent.md) | サインインがマルウェアに感染したデバイスから。 |
|[impossibleTravelRiskEvent](impossibletravelriskevent.md) | 典型的な場所に旅行を不可能になります。 |
|[leakedCredentialsRiskEvent](leakedcredentialsriskevent.md) | リークした資格情報を持つユーザーです。 |
|[suspiciousIpRiskEvent](suspiciousipriskevent.md) | 不審な IP アドレスからサインインの問題です。 |
|[unfamiliarLocationRiskEvent](unfamiliarlocationriskevent.md) | 未知の場所からサインインの問題です。 |

リスク イベントの詳細については、 [Azure AD のアイデンティティ保護のマニュアル](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-risk-events)を参照しています。

## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[IdentityRiskEvent を取得します。](../api/identityriskevent-get.md) | [identityRiskEvent](identityriskevent.md) |IdentityRiskEvent オブジェクトのプロパティと関係を参照してください。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|closedDateTime|dateTimeOffset| リスク イベントが終了したときの日時|
|createdDateTime|dateTimeOffset| 日付とイベントが作成された時刻です。 以上のリスク イベント自体の日付と時刻を常にです。 これは、リスク イベントを照会するときにフィルターとして使用する適切なプロパティです。|
|ID|文字列| 読み取り専用|
|riskEventDateTime|dateTimeOffset| リスク イベントが発生したときの日時|
|riskEventStatus|文字列| 可能な値は、`active`、`remediated`、`dismissedAsFixed`、`dismissedAsFalsePositive`、`dismissedAsIgnore`、`loginBlocked`、`closedMfaAuto`、`closedMultipleReasons` です。|
|riskLevel|文字列| 使用可能な値: `low`、`medium`、`high`。|
|riskEventType|文字列| リスクの種類|
|userDisplayName|文字列| リスクのユーザーの名前|
|userId|文字列| リスクのユーザーの id|
|userPrincipalName|文字列| リスクのユーザーのユーザー プリンシパル名|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|impactedUser|[user](user.md)| 読み取り専用です。Null 許容型。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。 

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.identityRiskEvent"
}-->

```json
{
  "closedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "riskEventDateTime": "String (timestamp)",
  "riskEventStatus": "string",
  "riskLevel": "string",
  "riskType": "string",
  "userDisplayName": "string",
  "userId": "string",
  "userPrincipalName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "identityRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->