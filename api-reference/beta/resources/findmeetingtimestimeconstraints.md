---
title: findMeetingTimesTimeConstraints リソースの種類
description: 指定したアクティビティの性質と空き時間帯に従って、会議の日時の候補を、特定の時間と曜日に限定します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: e5790faf49fea03040dca05d457fededf5fdd683
ms.sourcegitcommit: 539ed08adf3b7ad3253c98636d4ab303ce00176e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/15/2019
ms.locfileid: "30057404"
---
# <a name="findmeetingtimestimeconstraints-resource-type"></a>findMeetingTimesTimeConstraints リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

会議時間の提案を、活動の性質と特定の範囲の時間に制限します。 |

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.findMeetingTimesTimeConstraints"
}-->

```json
{
  "activityDomain": "String",
  "timeslots": [{"@odata.type": "microsoft.graph.timeSlot"}]
}

```
## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|activityDomain|activityDomain|アクティビティの性質です (省略可能)。使用可能な値: `work`、`personal`、`unrestricted`、`unknown`。|
|timeslots|[searchwindowtimeslot](searchwindowtimeslot.md)コレクション|可能な会議時間を検索する時間範囲の配列。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "findMeetingTimesTimeConstraints resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/findmeetingtimestimeconstraints.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->