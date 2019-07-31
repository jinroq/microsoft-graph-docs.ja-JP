---
title: リソースの種類の timeOff
description: スケジュールに含まれる非稼働時間の単位。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: 8c7d792b834125bdfb8a109c85b2c1f45b18230b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007656"
---
# <a name="timeoff-resource-type"></a>リソースの種類の timeOff

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

スケジュールに含まれる非稼働時間の単位。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[TimeOff の作成](../api/schedule-post-timesoff.md) | [timeOff](timeoff.md) | 新しい `timeOff` オブジェクトを作成します。|
|[TimeOffs のリスト](../api/schedule-list-timesoff.md) | [Timeoff](timeoff.md)コレクション | このスケジュールでオブジェクト`timeOff`のリストを取得します。|
|[TimeOff を取得する](../api/timeoff-get.md) | [timeOff](timeoff.md) | ID で `timeOff` を取得します。|
|[TimeOff を置換する](../api/timeoff-put.md) | [timeOff](timeoff.md) | `timeOff` を置き換えます。|
|[TimeOff の削除](../api/timeoff-delete.md) | None | スケジュールから`timeOff`を削除します。|

## <a name="properties"></a>プロパティ
|名前          |型           |説明                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| id            |`string`      |`timeOff` の ID。|
| userId            |`string`      |に割り当てられているユーザー `timeOff`の ID。 必須です。|
| sharedTimeOff     | [timeOffItem](timeoffitem.md)  |従業員とマネージャーの両方`timeOff`に表示される共有バージョン。 必須です。|
| draftTimeOff      | [timeOffItem](timeoffitem.md)        |この`timeOff`の下書きバージョンは、マネージャーが表示できます。 必須。|
| createdDateTime       |`DateTimeOffset`        |これ`timeOff`が最初に作成されたタイムスタンプ。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表します。これは常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、'2014-01-01T00:00:00Z'.のようになります。 |
| lastModifiedDateTime      |`DateTimeOffset`        |これ`timeOff`が最後に更新されたタイムスタンプ。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表します。これは常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、'2014-01-01T00:00:00Z'.のようになります。 |
| lastModifiedBy        | [identitySet](identityset.md)        |この `timeOff` を最後に更新した ID。 |

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.timeOff",
   "baseType":"microsoft.graph.changeTrackedEntity"
}-->

```json
{
  "userId": "string (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "lastModifiedBy": {"@odata.type":"microsoft.graph.identitySet"},
  "sharedTimeOff": {"@odata.type":"microsoft.graph.timeOffItem"},
  "draftTimeOff": {"@odata.type":"microsoft.graph.timeOffItem"}
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
  "suppressions": []
}
-->
