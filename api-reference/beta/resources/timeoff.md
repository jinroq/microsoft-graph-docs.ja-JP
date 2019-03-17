---
title: リソースの種類の timeoff
description: スケジュールに含まれる非稼働時間の単位。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 933c940e25c772cede7918dabf62b52ee58f18d2
ms.sourcegitcommit: 081cacecb4960aabc9e1011d12f06fe9ecf7d188
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/16/2019
ms.locfileid: "30657799"
---
# <a name="timeoff-resource-type"></a>リソースの種類の timeoff

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

スケジュールに含まれる非稼働時間の単位。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[timeoff の作成](../api/schedule-post-timesoff.md) | [timeoff](timeOff.md) | 新しい `timeOff` オブジェクトを作成します。|
|[timeoffs のリスト](../api/schedule-list-timesoff.md) | [timeoff](timeOff.md)コレクション | このスケジュールでオブジェクト`timeOff`のリストを取得します。|
|[timeoff を取得する](../api/timeoff-get.md) | [timeoff](timeOff.md) | ID `timeOff`で取得します。|
|[timeoff を置換する](../api/timeoff-put.md) | [timeoff](timeOff.md) | を`timeOff`置き換えます。|
|[timeoff の削除](../api/timeoff-delete.md) | なし | スケジュールから`timeOff`を削除します。|

## <a name="properties"></a>プロパティ
|名前          |型           |説明                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| id            |`string`      |の ID `timeOff`。|
| userId            |`string`      |に割り当てられているユーザー `timeOff`の ID。 必須。|
| sharedtimeoff     |`[timeOffItem](timeoffitem.md)`  |従業員とマネージャーの両方`timeOff`に表示される共有バージョン。 必須。|
| draftTimeOff      |`[timeOffItem](timeoffitem.md)`        |この`timeOff`の下書きバージョンは、マネージャーが表示できます。 必須。|
| createdDateTime       |`DateTimeOffset`        |これ`timeOff`が最初に作成されたタイムスタンプ。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。 たとえば、2014年1月1日午前0時 (UTC) は次のようになります。 ' 2014-01-01t00:00: 00z ' のようになります。 |
| lastModifiedDateTime      |`DateTimeOffset`        |これ`timeOff`が最後に更新されたタイムスタンプ。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。 たとえば、2014年1月1日午前0時 (UTC) は次のようになります。 ' 2014-01-01t00:00: 00z ' のようになります。 |
| lastModifiedBy        |`microsoft.graph.identitySet`        |最後に更新`timeOff`した id。 |

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.timeOff"
}-->

```json
{
  "userId": "c5d0c76b-80c4-481c-be50-923cd8d680a1",
  "createdDateTime": "2019-03-14T05:35:57.755Z",
  "lastModifiedDateTime": "2019-03-14T05:36:08.381Z",
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "conversation": null,
    "user": {
      "id": "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
      "displayName": "John Doe"
    }
  },
  "sharedTimeOff": {
    "timeOffReasonId": "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
    "startDateTime": "2019-03-11T07:00:00Z",
    "endDateTime": "2019-03-12T07:00:00Z",
    "theme": "white"
  },
  "draftTimeOff": {
    "timeOffReasonId": "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
    "startDateTime": "2019-03-11T07:00:00Z",
    "endDateTime": "2019-03-12T07:00:00Z",
    "theme": "pink"
  }
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeOff resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/timeoff.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
