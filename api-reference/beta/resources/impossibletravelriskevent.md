---
title: impossibleTravelRiskEvent リソースの種類
description: ユーザーにとって特殊な場所から2つのアカウントのサインインが発生する、Azure Active Directory Id 保護によって検出されたリスクイベント。また、サインイン間の期間内にある場所間を移動できません。詳細な情報リスクイベントについては、「Azure AD Identity Protection」のドキュメントを参照してください。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 2b66755924022b4fa30637cc8e97c4f944ad2d79
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36005773"
---
# <a name="impossibletravelriskevent-resource-type"></a>impossibleTravelRiskEvent リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

ユーザーにとって特殊な場所から2つのアカウントのサインインが発生する[Azure Active Directory Id 保護](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/)によって検出されるリスクイベント。これは、サインイン間の期間内で場所間を移動できません。リスクイベントに関する情報については、「 [AZURE AD Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/)」のドキュメントを参照してください。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[impossibleTravelRiskEvent を取得する](../api/impossibletravelriskevent-get.md) | [impossibleTravelRiskEvent](impossibletravelriskevent.md) |ImpossibleTravelRiskEvent オブジェクトのプロパティとリレーションシップを読み取ります。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|closedDateTime|dateTimeOffset| リスクイベントが終了した日付と時刻|
|createdDateTime|dateTimeOffset| リスクイベントが作成された日時。 これは常に、リスクイベント自体の datetime と同じかそれよりも大きくなります。 これは、リスクイベントを照会するときにフィルターとして使用する適切なプロパティです。|
|deviceInformation|string| デバイスに関する情報|
|id|string| 読み取り専用|
|ipAddress|string| 2番目のサインインの IP アドレス|
|isAtypicalLocation|ブール値| ユーザーのいずれかの場所が例外的である場合|
|location|string| 2番目のサインインの IP アドレスに接続されている場所|
|previousIPAddress|string| 最初のサインインの IP アドレス|
|previousLocation|string| 最初のサインインの IP アドレスに接続されている場所|
|previousSigninDateTime|dateTimeOffset| 最初のサインインの日付と時刻|
|riskEventDateTime|dateTimeOffset| 2番目のサインインの日付と時刻|
|riskEventStatus|string| 可能な値は、`active`、`remediated`、`dismissedAsFixed`、`dismissedAsFalsePositive`、`dismissedAsIgnore`、`loginBlocked`、`closedMfaAuto`、`closedMultipleReasons` です。|
|riskLevel|string| 使用可能な値: `low`、`medium`、`high`。|
|riskEventType|string| リスクの種類|
|userAgent|string| ブラウザーのユーザーエージェント文字列|
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
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.impossibleTravelRiskEvent"
}-->

```json
{
  "closedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "deviceInformation": "string",
  "id": "string (identifier)",
  "ipAddress": "string",
  "isAtypicalLocation": true,
  "location": "string",
  "previousIPAddress": "string",
  "previousLocation": "string",
  "previousSigninDateTime": "String (timestamp)",
  "riskEventDateTime": "String (timestamp)",
  "riskEventStatus": "string",
  "riskLevel": "string",
  "riskType": "string",
  "userAgent": "string",
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
  "description": "impossibleTravelRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
