---
title: anonymousIpRiskEvent リソースの種類
description: Azure Active Directory Id 保護によって検出された、匿名の IP アドレスからアカウントのサインインが試行されるリスクイベント。 リスクイベントに関する詳細な情報については、「Azure AD Identity Protection」のドキュメントを参照してください。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 5016aac704feb35383dc34e58f3ed06657733edf
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013393"
---
# <a name="anonymousipriskevent-resource-type"></a>anonymousIpRiskEvent リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[Azure Active Directory Id 保護](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/)によって検出された、匿名の IP アドレスからアカウントのサインインが試行されるリスクイベント。 リスクイベントに関する詳細な情報については、「 [AZURE AD Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/)」のドキュメントを参照してください。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[anonymousIpRiskEvent を取得する](../api/anonymousipriskevent-get.md) | [anonymousIpRiskEvent](anonymousipriskevent.md) |AnonymousIpRiskEvent オブジェクトのプロパティとリレーションシップを読み取ります。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|closedDateTime|dateTimeOffset| リスクイベントが終了した日付と時刻|
|createdDateTime|dateTimeOffset| リスクイベントが作成された日時。 これは常に、リスクイベント自体の datetime と同じかそれよりも大きくなります。 これは、リスクイベントを照会するときにフィルターとして使用する適切なプロパティです。|
|id|string| 読み取り専用|
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
|impactedUser|[ユーザー](user.md)| 読み取り専用。Null 許容型です。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
   "baseType":"microsoft.graph.locatedRiskEvent",
  "@odata.type": "microsoft.graph.anonymousIpRiskEvent"
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
  "description": "anonymousIpRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
