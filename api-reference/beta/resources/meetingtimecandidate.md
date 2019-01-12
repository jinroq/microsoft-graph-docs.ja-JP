---
title: meetingTimeCandidate リソースの種類
description: '提案された会議の時間、出勤の可能性、個人情報が含まれる会議 '
localization_priority: Normal
author: VinodRavichandran
ms.prod: microsoft-teams
ms.openlocfilehash: 13a4b9af442c8cde7a6db48d651946bbb88416e1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27922355"
---
# <a name="meetingtimecandidate-resource-type"></a>meetingTimeCandidate リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

会議時間、出席の可能性、各自の空き時間情報、利用可能な会議場所を含む、会議の提案です。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingTimeCandidate"
}-->

```json
{
  "attendeeAvailability": [{"@odata.type": "microsoft.graph.attendeeAvailability"}],
  "confidence": 1024.0,
  "locations": [{"@odata.type": "microsoft.graph.location"}],
  "meetingTimeSlot": {"@odata.type": "microsoft.graph.timeSlot"},
  "organizerAvailability": "String",
  "suggestionHint": "String"
}

```
## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|attendeeAvailability|[attendeeAvailability](attendeeavailability.md) コレクション|この提案された会議の各出席者の空き時間情報の状態を示す配列。|
|confidence|Double|すべての出席者が出席する見込みを表すパーセンテージ。|
|locations|[location](location.md) コレクション|この提案された会議の各会議場所の名前と地理的な場所を指定する配列。|
|meetingTimeSlot|[timeSlot](timeslot.md)|会議の提案されている期間。|
|organizerAvailability|String| この提案されている会議の開催者の空き時間情報。使用可能な値: `free`、`tentative`、`busy`、`oof`、`workingElsewhere`、`unknown`。|
|suggestionHint|String|会議時間を提案する理由。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingTimeCandidate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
