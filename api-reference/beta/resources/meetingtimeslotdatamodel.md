---
title: meetingTimeSlotDataModel リソースの種類
description: 期間。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: acbd08da5e15dd733c63c0141db5b58cee896666
ms.sourcegitcommit: 539ed08adf3b7ad3253c98636d4ab303ce00176e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/15/2019
ms.locfileid: "30057396"
---
# <a name="meetingtimeslotdatamodel-resource-type"></a>meetingTimeSlotDataModel リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

会議の時間帯を表します。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingTimeSlotDataModel"
}-->

```json
{
  "end": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "start": {"@odata.type": "microsoft.graph.dateTimeTimeZone"}
}

```
## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|end|[dateTimeTimeZone](datetimetimezone.md)|期間が始まる日付、時刻、タイムゾーン。 |
|start|[dateTimeTimeZone](datetimetimezone.md)|期間が終了する日付、時刻、タイムゾーン。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "meetingTimeSlotDataModel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/meetingtimeslotdatamodel.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->