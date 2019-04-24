---
title: identityRiskEvent リソースの種類
description: Azure Active Directory id 保護によって検出されたリスクイベント。 これは、各固有のリスクイベントの種類の基本型です。
author: cloudhandler
localization_priority: Normal
ms.prod: security
ms.openlocfilehash: b5c36ab898805c0638cc199ff8cfb893444f04ec
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32506401"
---
# <a name="identityriskevent-resource-type"></a>identityRiskEvent リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[Azure Active Directory id 保護](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/)によって検出されたリスクイベント。 これは、各固有のリスクイベントの種類の基本型です。

| イベントの種類         | 説明|
|:---------------|:-----------|
|[anonymousipRiskEvent](anonymousipriskevent.md) | 匿名 IP アドレスからのサインイン。 |
|[malwareRiskEvent](malwareriskevent.md) | マルウェアに感染したデバイスからのサインイン。 |
|[impossibleTravelRiskEvent](impossibletravelriskevent.md) | 例外的でない場所への移動は不可能です。 |
|[leakedCredentialsRiskEvent](leakedcredentialsriskevent.md) | 資格情報がリークしたユーザー。 |
|[suspiciousIpRiskEvent](suspiciousipriskevent.md) | 疑わしい IP アドレスからのサインイン。 |
|[unfamiliarLocationRiskEvent](unfamiliarlocationriskevent.md) | 見慣れない場所からのサインイン。 |

リスクイベントに関する詳細な情報については、「 [Azure AD Identity Protection](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-risk-events)」のドキュメントを参照してください。

## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[identityRiskEvent を取得する](../api/identityriskevent-get.md) | [identityRiskEvent](identityriskevent.md) |identityRiskEvent オブジェクトのプロパティとリレーションシップを読み取ります。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|closeddatetime|dateTimeOffset| リスクイベントが終了した日付と時刻|
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
<!--
{
  "type": "#page.annotation",
  "description": "identityRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/identityriskevent.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
