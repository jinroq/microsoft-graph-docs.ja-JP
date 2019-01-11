---
title: meetingTimeSuggestionsResult リソースの種類
description: 会議の提案がある場合にはそのコレクションを、ない場合にはその理由を示します。
localization_priority: Normal
ms.openlocfilehash: aff5abd69297cd466027c1a614b2609697c00ce6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27806840"
---
# <a name="meetingtimesuggestionsresult-resource-type"></a>meetingTimeSuggestionsResult リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

会議の提案がある場合にはそのコレクションを、ない場合にはその理由を示します。

[findMeetingTimes](../api/user-findmeetingtimes.md) が会議の提案を何も返さない理由として考えられるものを以下に示します。

|**emptySuggestionsReason value**|**理由**|
|:-----|:-----|
| attendeesUnavailable | すべての出席者の空き時間情報を把握していますが、[会議の確実性](../api/user-findmeetingtimes.md#the-confidence-of-a-meeting-suggestion)しきい値 (既定では 50%) に達するにはすべての時間帯で出席者が足りません。|
| attendeesUnavailableOrUnknown | 一部またはすべての出席者の空き時間情報が不明なため、会議の確実性が設定されているしきい値 (既定では 50%) を下回っています。出席者が組織外の場合、または空き時間情報の取得でエラーが生じる場合には、出席者の空き時間情報が不明になることがあります。|
| locationsUnavailable | [locationConstraint](locationconstraint.md) の **isRequired** プロパティが必須に指定されているものの、算出された時間範囲で利用可能な場所がありません。 |
| organizerUnavailable | **IsOrganizerOptional** パラメーターが false で、要求された時間枠では、主催者が現時点で出席可能ではありません。 |
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
| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|emptySuggestionsReason|String|会議提案が 1 つも返されない理由。使用可能な値: `attendeesUnavailable`、`attendeesUnavailableOrUnknown`、`locationsUnavailable`、`organizerUnavailable`、`unknown`。このプロパティは、**meetingTimeSuggestions** プロパティに会議提案が含まれる場合は空の文字列です。|
|meetingTimeSuggestions|[meetingTimeSuggestion](meetingtimesuggestion.md) コレクション|会議提案の配列。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingTimeSuggestionsResult resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
