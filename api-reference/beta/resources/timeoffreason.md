---
title: timeoffreason リソースの種類
description: スケジュールでタイムアウトになる有効な理由。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 8ba1e4bd596b82643ecbfa4b842e60232c182a4b
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341975"
---
# <a name="timeoffreason-resource-type"></a>timeoffreason リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[スケジュール](schedule.md)内の[timeoff](timeoff.md)インスタンスの有効な理由。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[timeoffreason の作成](../api/schedule-post-timeoffreasons.md) | [timeoffreason](timeoffreason.md) | 新しい `timeOffReason` を作成します。|
|[リスト timeoffreason](../api/schedule-list-timeoffreasons.md) | [timeoffreason](timeoffreason.md)コレクション | スケジュール内の `timeOffReasons` のリストを取得します。|
|[timeoffreason を取得する](../api/timeoffreason-get.md) | [timeoffreason](timeoffreason.md) | ID で `timeOffReason` を取得します。|
|[timeoffreason を置換する](../api/timeoffreason-put.md) | [timeoffreason](timeoffreason.md) | `timeOffReason` を置き換えます。|
|[timeoffreason の削除](../api/timeoffreason-delete.md) | なし | `timeOffReason` を非アクティブとしてマークします。|

## <a name="properties"></a>プロパティ
|名前          |型           |説明                                                                                 |
|--------------|---------------|--------------------------------------------------------------------------------------------|
| id            |`string`      |`timeOffReason` の ID。|
| displayName               | `string`                  | の名前`timeOffReason`。 必須です。 |
| icontype | `timeOffReasonIconType`   | サポートされているアイコンの種類: なし、故障]起動平面ファイヤな id;診察notworking;レコーダーjuryDuty;世界中カップ代わり天気予報付piggyBank;エサケーキtrafficCone;pin晴れ. 必須です。 |
| isActive          |`Boolean`      | 新しくエンティティを作成する場合や、既存のエンティティを更新する場合に `timeOffReason` を使用できるかどうかを示します。 必須。 |
| createdDateTime       |`DateTimeOffset`        |これ`timeOffReason`が最初に作成されたタイムスタンプ。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表します。これは常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、'2014-01-01T00:00:00Z'.のようになります。 |
| lastModifiedDateTime      |`DateTimeOffset`         |これ`timeOffReason`が最後に更新されたタイムスタンプ。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表します。これは常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、'2014-01-01T00:00:00Z'.のようになります。 |
| lastModifiedBy        | [identitySet](identityset.md)        |この `timeOffReason` を最後に更新した ID。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.timeOffReason",
  "baseType":"microsoft.graph.changeTrackedEntity"
}-->

```json
{
  "id": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "iconType": "String",
  "isActive": true,
  "lastModifiedBy": { "@odata.type":"microsoft.graph.identitySet"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeOffReason resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
