---
title: impossibleTravelRiskEvent リソースの種類
description: Azure Active ディレクトリ Id 保護、ユーザーの典型的な場所から 2 つのアカウントのサインインの問題が発生して、に関する該当の記号の完全な情報の間の期間内の場所の間を移動することはできませんが検出されたリスク イベントリスク イベントは、Azure AD のアイデンティティ保護のマニュアルを参照しています。
localization_priority: Normal
ms.openlocfilehash: 517a09963570ce2c4a9e58edf7b73babaaff0426
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529384"
---
# <a name="impossibletravelriskevent-resource-type"></a>impossibleTravelRiskEvent リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
|deviceInformation|string| デバイスに関する情報|
|id|string| 読み取り専用|
|ipAddress|string| 2 つ目のサインインの IP アドレス|
|isAtypicalLocation|boolean| ユーザーの典型的な場所のいずれかの場合|
|location|string| 2 つ目のサインインの IP アドレスに接続されている場所|
|previousIPAddress|string| 最初のサインインの IP アドレス|
|PreviousLocation|string| 最初のサインインの IP アドレスに接続されている場所|
|previousSigninDateTime|dateTimeOffset| 日付と時刻の最初のサインイン|
|riskEventDateTime|dateTimeOffset| 日付と時刻の 2 つ目のサインイン|
|riskEventStatus|string| 可能な値は、`active`、`remediated`、`dismissedAsFixed`、`dismissedAsFalsePositive`、`dismissedAsIgnore`、`loginBlocked`、`closedMfaAuto`、`closedMultipleReasons` です。|
|riskLevel|string| 使用可能な値: `low`、`medium`、`high`。|
|riskEventType|string| リスクの種類|
|UserAgent|string| ブラウザーのユーザー エージェント文字列|
|userDisplayName|string| リスクのユーザーの名前|
|userId|string| リスクのユーザーの id|
|userPrincipalName|string| リスクのユーザーのユーザー プリンシパル名|

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
<!--
{
  "type": "#page.annotation",
  "description": "impossibleTravelRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/impossibletravelriskevent.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
