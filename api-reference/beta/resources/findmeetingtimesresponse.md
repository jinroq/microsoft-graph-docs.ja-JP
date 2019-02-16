---
title: findmeetingtimesresponse リソースの種類
description: 会議の提案がある場合にはそのコレクションを、ない場合にはその理由を示します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 0d52da8e5798932d4f78463d6e4bea08ecb7c793
ms.sourcegitcommit: 539ed08adf3b7ad3253c98636d4ab303ce00176e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/15/2019
ms.locfileid: "30057399"
---
# <a name="findmeetingtimesresponse-resource-type"></a>findmeetingtimesresponse リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

会議の提案がある場合は、そのコレクション。また、存在しない場合は理由があります。

[findMeetingTimes](../api/user-findmeetingtimes.md) が会議の提案を何も返さない理由として考えられるものを以下に示します。

|**emptySuggestionsReason value**|**理由**|
|:-----|:-----|
| attendeesUnavailable | すべての出席者の空き時間情報を把握していますが、[会議の確実性](../api/user-findmeetingtimes.md#the-confidence-of-a-meeting-suggestion)しきい値 (既定では 50%) に達するにはすべての時間帯で出席者が足りません。|
| attendeesUnavailableOrUnknown | 一部またはすべての出席者の空き時間情報が不明なため、会議の確実性が設定されているしきい値 (既定では 50%) を下回っています。出席者が組織外の場合、または空き時間情報の取得でエラーが生じる場合には、出席者の空き時間情報が不明になることがあります。|
| locationsUnavailable | **locationConstraint**パラメーターの**isRequired**プロパティは true と指定されていますが、計算された時間帯に使用可能な場所がありません。 |
| organizerUnavailable | **IsOrganizerOptional** パラメーターが false で、要求された時間枠では、主催者が現時点で出席可能ではありません。 |
| 不明 | 会議提案が 1 つも返されない理由が不明です。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.findMeetingTimesResponse"
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
|emptySuggestionsReason|String|会議提案が 1 つも返されない理由。使用可能な値: `attendeesUnavailable`、`attendeesUnavailableOrUnknown`、`locationsUnavailable`、`organizerUnavailable`、`unknown`。このプロパティは、**meetingTimeSuggestions** プロパティに会議提案が含まれる場合は空の文字列です。|
|meetingTimeSuggestions|[meetingTimeSuggestion](meetingtimesuggestion.md) コレクション|会議提案の配列。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "findMeetingTimesResponse resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/findmeetingtimesresponse.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->