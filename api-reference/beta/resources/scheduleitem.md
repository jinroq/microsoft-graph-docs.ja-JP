---
title: scheduleitem リソースの種類
description: ユーザーの既定の予定表にある実際のイベントに対応するユーザーの空き時間情報を示すアイテム。 この項目は、リソースにも適用されます。
localization_priority: Normal
ms.openlocfilehash: a39f45598ab3c427a741659aa93615317c3c57a7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563060"
---
# <a name="scheduleitem-resource-type"></a>scheduleitem リソースの種類

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
ユーザーの既定の予定表にある実際のイベントに対応するユーザーの空き時間情報を示すアイテム。 この項目は、リソース (会議室または備品) にも適用されます。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|end |[dateTimeTimeZone](datetimetimezone.md) |対応するイベントが終了する日付、時刻、タイムゾーン。 |
|isPrivate |Boolean |対応するイベントの感度。 イベントがマーク`private`されている場合は True、それ以外の場合は false。 省略可能。 |
|location |String | 対応するイベントが保持または参加している場所。 省略可能。|
|start |[dateTimeTimeZone](datetimetimezone.md) |対応するイベントが開始する日付、時刻、タイムゾーン。 |
|status |freeBusyStatus | 対応するイベント中のユーザーまたはリソースの空き時間状態。 使用可能な値は`free`、 `tentative`、 `busy` `oof` `workingElsewhere`、、、 `unknown`、です。 |
|subject |String | 対応するイベントの件名行。 省略可能。|


## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "isPrivate",
    "location",
    "subject"
  ],
  "@odata.type": "microsoft.graph.scheduleItem"
}-->

```json
{
  "end": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "isPrivate": true,
  "location": "String",
  "start": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "status": "String",
  "subject": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "scheduleItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
