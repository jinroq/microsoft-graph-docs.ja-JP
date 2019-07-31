---
title: identityRiskEvent リソースの種類
description: Azure Active Directory Id 保護によって検出されたリスクイベント。 これは、各固有のリスクイベントの種類の基本型です。
author: cloudhandler
localization_priority: Normal
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 7ea0a11931021e828660cc7b03991b8ea96ef1f1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36005801"
---
# <a name="identityriskevent-resource-type"></a>identityRiskEvent リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[Azure Active Directory Id 保護](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/)によって検出されたリスクイベント。 これは、各固有のリスクイベントの種類の基本型です。

| イベントの種類         | 説明|
|:---------------|:-----------|
|[anonymousipRiskEvent](anonymousipriskevent.md) | 匿名 IP アドレスからのサインイン。 |
|[malwareRiskEvent](malwareriskevent.md) | マルウェアに感染したデバイスからのサインイン。 |
|[impossibleTravelRiskEvent](impossibletravelriskevent.md) | 例外的でない場所への移動は不可能です。 |
|[leakedCredentialsRiskEvent](leakedcredentialsriskevent.md) | 資格情報がリークしたユーザー。 |
|[suspiciousIpRiskEvent](suspiciousipriskevent.md) | 疑わしい IP アドレスからのサインイン。 |
|[unfamiliarLocationRiskEvent](unfamiliarlocationriskevent.md) | 見慣れない場所からのサインイン。 |

リスクイベントに関する詳細な情報については、「 [AZURE AD Identity Protection](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-risk-events)」のドキュメントを参照してください。

## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[identityRiskEvent を取得する](../api/identityriskevent-get.md) | [identityRiskEvent](identityriskevent.md) |IdentityRiskEvent オブジェクトのプロパティとリレーションシップを読み取ります。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|closedDateTime|dateTimeOffset| リスクイベントが終了した日付と時刻|
|createdDateTime|dateTimeOffset| リスクイベントが作成された日時。 これは常に、リスクイベント自体の datetime と同じかそれよりも大きくなります。 これは、リスクイベントを照会するときにフィルターとして使用する適切なプロパティです。|
|id|string| 読み取り専用|
|riskEventDateTime|dateTimeOffset| リスクイベントが発生した日付と時刻|
|riskEventStatus|string| 可能な値は、`active`、`remediated`、`dismissedAsFixed`、`dismissedAsFalsePositive`、`dismissedAsIgnore`、`loginBlocked`、`closedMfaAuto`、`closedMultipleReasons` です。|
|riskLevel|string| 使用可能な値: `low`、`medium`、`high`。|
|riskEventType|string| リスクの種類|
|userDisplayName|string| リスクのあるユーザーの名前|
|userId|string| リスクがあるユーザーの id|
|userPrincipalName|string| リスクがあるユーザーのユーザープリンシパル名|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|impactedUser|[ユーザー](user.md)| 読み取り専用。Null 許容型です。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。 

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
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
  "userPrincipalName": "string",
  "riskEventType": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "identityRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
