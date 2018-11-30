---
title: impossibleTravelRiskEvent リソースの種類
description: Azure Active ディレクトリ Id 保護、ユーザーの典型的な場所から 2 つのアカウントのサインインの問題が発生して、に関する該当の記号の完全な情報の間の期間内の場所の間を移動することはできませんが検出されたリスク イベントリスク イベントは、Azure AD のアイデンティティ保護のマニュアルを参照しています。
ms.openlocfilehash: 38e61927121f520e79fd1fec8b8e6443fa8b76e7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066785"
---
# <a name="impossibletravelriskevent-resource-type"></a>impossibleTravelRiskEvent リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

[Azure Active Directory アイデンティティの保護](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/)ユーザーの典型的な場所から 2 つのアカウントのサインインの問題が発生して、記号再起動の完了の間の期間内の場所の間を移動することはできませんが検出されたリスク イベント[Azure AD のアイデンティティ保護マニュアル](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/)のリスクについての情報が見つかります。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[ImpossibleTravelRiskEvent を取得します。](../api/impossibletravelriskevent-get.md) | [impossibleTravelRiskEvent](impossibletravelriskevent.md) |ImpossibleTravelRiskEvent オブジェクトのプロパティと関係を参照してください。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|closedDateTime|dateTimeOffset| リスク イベントが終了したときの日時|
|createdDateTime|dateTimeOffset| 日付とイベントが作成された時刻です。 以上のリスク イベント自体の日付と時刻を常にです。 これは、リスク イベントを照会するときにフィルターとして使用する適切なプロパティです。|
|deviceInformation|文字列| デバイスに関する情報|
|ID|文字列| 読み取り専用|
|ipAddress|文字列| 2 つ目のサインインの IP アドレス|
|isAtypicalLocation|ブール| ユーザーの典型的な場所のいずれかの場合|
|location|文字列| 2 つ目のサインインの IP アドレスに接続されている場所|
|previousIPAddress|文字列| 最初のサインインの IP アドレス|
|previousLocation|文字列| 最初のサインインの IP アドレスに接続されている場所|
|previousSigninDateTime|dateTimeOffset| 日付と時刻の最初のサインイン|
|riskEventDateTime|dateTimeOffset| 日付と時刻の 2 つ目のサインイン|
|riskEventStatus|文字列| 可能な値は、`active`、`remediated`、`dismissedAsFixed`、`dismissedAsFalsePositive`、`dismissedAsIgnore`、`loginBlocked`、`closedMfaAuto`、`closedMultipleReasons` です。|
|riskLevel|文字列| 使用可能な値: `low`、`medium`、`high`。|
|riskEventType|文字列| リスクの種類|
|userAgent|文字列| ブラウザーのユーザー エージェント文字列|
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
  "userPrincipalName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "impossibleTravelRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->