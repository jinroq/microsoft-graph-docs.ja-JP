---
title: timeoffreason リソースの種類
description: スケジュールでタイムアウトになる有効な理由。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 72597fa1678110a40b9dd1a0ea6e6235625144ab
ms.sourcegitcommit: 081cacecb4960aabc9e1011d12f06fe9ecf7d188
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/16/2019
ms.locfileid: "30657533"
---
# <a name="timeoffreason-resource-type"></a>timeoffreason リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[スケジュール](schedule.md)内の[timeoff](timeoff.md)インスタンスの有効な理由。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[timeoffreason の作成](../api/schedule-post-timeoffreasons.md) | [timeoffreason](timeoffreason.md) | 新しい`timeOffReason`を作成します。|
|[リスト timeoffreason](../api/schedule-list-timeoffreasons.md) | [timeoffreason](timeoffreason.md)コレクション | スケジュールに含まれる`timeOffReasons`のリストを取得します。|
|[timeoffreason を取得する](../api/timeoffreason-get.md) | [timeoffreason](timeoffreason.md) | ID `timeOffReason`で取得します。|
|[timeoffreason を置換する](../api/timeoffreason-put.md) | [timeoffreason](timeoffreason.md) | を`timeOffReason`置き換えます。|
|[timeoffreason の削除](../api/timeoffreason-delete.md) | なし | 非`timeOffReason`アクティブとしてマークします。|

## <a name="properties"></a>プロパティ
|名前          |型           |説明                                                                                 |
|--------------|---------------|--------------------------------------------------------------------------------------------|
| id            |`string`      |の ID `timeOffReason`。|
| displayName               | `string`                  | の名前`timeOffReason`。 必須。 |
| icontype | `enum`   | サポートされているアイコンの種類: なし、故障]起動平面ファイヤな id;診察notworking;レコーダーjuryDuty;世界中カップ代わり天気予報付piggyBank;エサケーキtrafficCone;pin晴れ. 必須。 |
| isActive          |`bool`      | 新しいエンティティを`timeOffReason`作成するとき、または既存のエンティティを更新するときに、を使用できるかどうかを示します。 必須。 |
| createdDateTime       |`DateTimeOffset`        |これ`timeOffReason`が最初に作成されたタイムスタンプ。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。 たとえば、2014年1月1日午前0時 (UTC) は次のようになります。 ' 2014-01-01t00:00: 00z ' のようになります。 |
| lastModifiedDateTime      |`DateTimeOffset`         |これ`timeOffReason`が最後に更新されたタイムスタンプ。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。 たとえば、2014年1月1日午前0時 (UTC) は次のようになります。 ' 2014-01-01t00:00: 00z ' のようになります。 |
| lastModifiedBy        |`microsoft.graph.identitySet`        |最後に更新`timeOffReason`した id。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.timeOffReason"
}-->

```json
{
  "id": "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
  "createdDateTime": "2019-03-12T22:10:38.242Z",
  "lastModifiedDateTime": "2019-03-12T22:10:38.242Z",
  "displayName": "Vacation",
  "iconType": "plane",
  "isActive": true,
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "conversation": null,
    "user": {
      "id": "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
      "displayName": "John Doe"
    }
  }
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
  "suppressions": [
    "Error: /api-reference/beta/resources/timeoffreason.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
