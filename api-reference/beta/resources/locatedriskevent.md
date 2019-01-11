---
title: locatedRiskEvent リソースの種類
description: Azure Active ディレクトリ Id 保護場所データに基づくによって検出されたリスク イベントです。 あるリスク イベントの種類は次のとおりです。
localization_priority: Normal
ms.openlocfilehash: 256c7a980fb9540e7e80337a5b8aad29fe73f26a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27867558"
---
# <a name="locatedriskevent-resource-type"></a>locatedRiskEvent リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

場所データに基づく[Azure Active Directory アイデンティティ保護](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/)によって検出されたリスク イベントです。 あるリスク イベントの種類は次のとおりです。
* [匿名の IP アドレスからサインイン](anonymousipriskevent.md)
* [マルウェアに感染したデバイスからのサインインの問題](malwareriskevent.md)
* [典型的な場所に旅行を不可能になります。](impossibletravelriskevent.md)
* [不審な IP アドレスからサインイン](suspiciousipriskevent.md)
* [未知の場所からサインイン](unfamiliarlocationriskevent.md)リスク イベントの詳細については、 [Azure AD のアイデンティティ保護のマニュアル](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/)を参照しています。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[LocatedRiskEvent を取得します。](../api/locatedriskevent-get.md) | [locatedRiskEvent](locatedriskevent.md) |LocatedRiskEvent オブジェクトのプロパティと関係を参照してください。|

## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|closedDateTime|dateTimeOffset| リスク イベントが終了したときの日時|
|createdDateTime|dateTimeOffset| 日付とイベントが作成された時刻です。 以上のリスク イベント自体の日付と時刻を常にです。 これは、リスク イベントを照会するときにフィルターとして使用する適切なプロパティです。|
|ID|文字列| 読み取り専用です。|
|ipAddress|文字列| サインイン用の IP アドレス|
|location|文字列| サインイン用の IP アドレスに接続されている場所|
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
  "userPrincipalName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "locatedRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
