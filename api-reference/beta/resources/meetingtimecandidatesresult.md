---
title: meetingTimeCandidatesResult リソースの種類
description: 会議の提案がある場合にはそのコレクションを、ない場合にはその理由を示します。
ms.openlocfilehash: 38ca5b6be15d3cd268403f7f95645a8aaf31cf9d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067195"
---
# <a name="meetingtimecandidatesresult-resource-type"></a>meetingTimeCandidatesResult リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

会議の提案がある場合にはそのコレクションを、ない場合にはその理由を示します。

[findMeetingTimes](../api/user-findmeetingtimes.md) が会議の提案を何も返さない理由として考えられるものを以下に示します。

|**emptySuggestionsHint 値**|**理由**|
|:-----|:-----|
| attendeesUnavailable | すべての出席者の空き時間情報を把握していますが、会議の確実性しきい値 (既定では 50%) に達するにはすべての時間帯で出席者が足りません。 このしきい値は、出席者の空き/予約済みの状態の提案された会議の期間、出勤、[不明] 状態の 50%、および 0% のビジー状態の可能性が 100% に対応する出席者の空きの状態に基づきます。|
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
  "@odata.type": "microsoft.graph.meetingTimeCandidatesResult"
}-->

```json
{
  "emptySuggestionsHint": "String",
  "meetingTimeSlots": [{"@odata.type": "microsoft.graph.meetingTimeCandidate"}]
}

```
## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|emptySuggestionsHint|String|会議提案が 1 つも返されない理由。可能な値: `attendeesUnavailable`、`attendeesUnavailableOrUnknown`、`locationsUnavailable`、`organizerUnavailable`、または `unknown`。|
|meetingTimeSlots|[meetingTimeCandidate](meetingtimecandidate.md)コレクション|会議提案の配列。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingTimeCandidatesResult resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->