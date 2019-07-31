---
title: meetingTimeSuggestionsResult リソースの種類
description: 会議の提案がある場合は、そのコレクション。また、存在しない場合は理由があります。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 7f9759347c4b27131c3a305658dd3c5b360841f9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966853"
---
# <a name="meetingtimesuggestionsresult-resource-type"></a>meetingTimeSuggestionsResult リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

会議の提案がある場合は、そのコレクション。また、存在しない場合は理由があります。

[findMeetingTimes](../api/user-findmeetingtimes.md) が会議の提案を何も返さない理由として考えられるものを以下に示します。

|**emptySuggestionsReason value**|**理由**|
|:-----|:-----|
| attendeesUnavailable | すべての出席者の空き時間情報がわかっていますが、[会議の信頼度](../api/user-findmeetingtimes.md#the-confidence-of-a-meeting-suggestion)のしきい値 (既定では 50%) に到達できる十分な出席者がいません。|
| attendeesUnavailableOrUnknown | 一部またはすべての出席者の空き時間情報が不明なため、会議の確実性が設定されているしきい値 (既定では 50%) を下回っています。出席者が組織外の場合、または空き時間情報の取得でエラーが生じる場合には、出席者の空き時間情報が不明になることがあります。|
| locationsUnavailable | **LocationConstraint**パラメーターの**isRequired**プロパティは true と指定されていますが、計算された時間帯に使用可能な場所がありません。 |
| 組織が利用できません | **IsOrganizerOptional** パラメーターが false で、要求された時間枠では、主催者が現時点で出席可能ではありません。 |
| 不明 | 会議提案が 1 つも返されない理由が不明です。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingTimeSuggestionsResult"
}-->

```json
{
  "emptySuggestionsReason": "String",
  "meetingTimeSuggestions": [{"@odata.type": "microsoft.graph.meetingTimeSuggestion"}]
}

```
## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|emptySuggestionsReason|String|会議提案が 1 つも返されない理由。 可能な値は、`attendeesUnavailable`、`attendeesUnavailableOrUnknown`、`locationsUnavailable`、`organizerUnavailable`、`unknown` です。 会議の**タイム Times/Ge/アドオン**プロパティに会議の提案が含まれている場合、このプロパティは空の文字列になります。|
|会議のタイムスパン|[meetingTimeSuggestion](meetingtimesuggestion.md) コレクション|会議提案の配列。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "meetingTimeSuggestionsResult resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
