---
title: scheduleItem リソースの種類
description: ユーザーの既定の予定表にある実際のイベントに対応するユーザーの空き時間情報を示すアイテム。 この項目は、リソースにも適用されます。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-teams
author: ''
ms.openlocfilehash: f2901412dcf1d52d8b117afa214da159b4553a8a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008643"
---
# <a name="scheduleitem-resource-type"></a>scheduleItem リソースの種類

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
ユーザーの既定の予定表にある実際のイベントに対応するユーザーの空き時間情報を示すアイテム。 この項目は、リソース (会議室または備品) にも適用されます。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|end |[dateTimeTimeZone](datetimetimezone.md) |対応するイベントが終了する日付、時刻、タイムゾーン。 |
|isPrivate |Boolean |対応するイベントの感度。 イベントがマーク`private`されている場合は True、それ以外の場合は false。 省略可能。 |
|location |String | 対応するイベントが保持または参加している場所。 省略可能。|
|開始 |[dateTimeTimeZone](datetimetimezone.md) |対応するイベントが開始する日付、時刻、タイムゾーン。 |
|status |freeBusyStatus | 対応するイベント中のユーザーまたはリソースの空き時間状態。 使用可能な値: `free`、`tentative`、`busy`、`oof`、`workingElsewhere`、`unknown`。 |
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
