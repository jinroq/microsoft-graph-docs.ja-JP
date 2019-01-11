---
title: meetingTimeSuggestion リソースの種類
description: '提案された会議の時間、出勤の可能性、個人情報が含まれる会議 '
localization_priority: Normal
ms.openlocfilehash: d1cca365c66c114063fbf859e241a5d9a81303e2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845998"
---
# <a name="meetingtimesuggestion-resource-type"></a>meetingTimeSuggestion リソースの種類

会議時間、出席の可能性、各自の空き時間情報、利用可能な会議場所を含む、会議の提案です。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingTimeSuggestion"
}-->

```json
{
  "attendeeAvailability": [{"@odata.type": "microsoft.graph.attendeeAvailability"}],
  "confidence": 100.0,
  "locations": [{"@odata.type": "microsoft.graph.location"}],
  "meetingTimeSlot": {"@odata.type": "microsoft.graph.timeSlot"},
  "organizerAvailability": "String",
  "suggestionReason": "String"
}

```
## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|attendeeAvailability|[attendeeAvailability](attendeeavailability.md) コレクション|この提案された会議の各出席者の空き時間情報の状態を示す配列。|
|confidence|Double|すべての出席者が出席する見込みを表すパーセンテージ。|
|locations|[location](location.md) コレクション|この提案された会議の各会議場所の名前と地理的な場所を指定する配列。|
|meetingTimeSlot|[timeSlot](timeslot.md)|会議の提案されている期間。|
|organizerAvailability|freeBusyStatus| この提案された会議の開催者の可用性。 可能な値: `free`、 `tentative`、 `busy`、 `oof`、 `workingElsewhere`、 `unknown`。|
|suggestionReason|String|会議時間を提案する理由。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingTimeSuggestion resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
