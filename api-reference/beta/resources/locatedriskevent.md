---
title: locatedRiskEvent リソースの種類
description: 場所データに基づく Azure Active Directory id 保護によって検出されたリスクイベント。 存在するリスクイベントの種類は次のとおりです。
localization_priority: Normal
ms.openlocfilehash: 2c7503c08700a0d7c2d2ad67e8868901bdb008e2
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345371"
---
# <a name="locatedriskevent-resource-type"></a>locatedRiskEvent リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

場所データに基づく[Azure Active Directory id 保護](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/)によって検出されたリスクイベント。 存在するリスクイベントの種類は次のとおりです。
* [匿名 IP アドレスからのサインイン](anonymousipriskevent.md)
* [マルウェアに感染したデバイスからのサインイン](malwareriskevent.md)
* [例外的でない場所への移動は不可能](impossibletravelriskevent.md)
* [疑わしい IP アドレスからのサインイン](suspiciousipriskevent.md)
* [見慣れない場所からのサインイン](unfamiliarlocationriskevent.md)リスクイベントに関する詳細な情報については、「 [Azure AD Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/)」のドキュメントを参照してください。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[locatedRiskEvent を取得する](../api/locatedriskevent-get.md) | [locatedRiskEvent](locatedriskevent.md) |locatedRiskEvent オブジェクトのプロパティとリレーションシップを読み取ります。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|closeddatetime|dateTimeOffset| リスクイベントが終了した日付と時刻|
|createdDateTime|dateTimeOffset| リスクイベントが作成された日時。 これは常に、リスクイベント自体の datetime と同じかそれよりも大きくなります。 これは、リスクイベントを照会するときにフィルターとして使用する適切なプロパティです。|
|id|文字列| 読み取り専用|
|ipAddress|string| サインインの IP アドレス|
|location|string| サインインの IP アドレスに関連付けられている場所|
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
|impactedUser|[user](user.md)| 読み取り専用。Null 許容型です。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
   "abstract": true,
   "keyProperty": "id",
   "baseType":"microsoft.graph.identityRiskEvent",
  "@odata.type": "microsoft.graph.locatedRiskEvent"
}-->

```json
{
  "closedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "ipAddress": "string",
  "location": "string",
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
  "description": "locatedRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
