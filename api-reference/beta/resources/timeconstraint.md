---
title: timeConstraint リソースの種類
description: 指定されたアクティビティの性質および開いている時間帯に従って、会議時間の提案を特定の時間と曜日に制限します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 680ada778ea64f982e9ed5fac11c935a6cce55d5
ms.sourcegitcommit: a90abf5b89dbbdfefb1b7794d1f12c6e2bfb0cda
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/28/2019
ms.locfileid: "30937792"
---
# <a name="timeconstraint-resource-type"></a>timeConstraint リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

指定されたアクティビティの性質および開いている時間帯に従って、会議時間の提案を特定の時間と曜日に制限します。


## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeConstraint"
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
|activityDomain|activityDomain|活動の性質です (省略可能)。 可能な値は`work`、 `personal`、 `unrestricted`、、 `unknown`またはです。|
|timeslots|[timeSlot](timeslot.md) コレクション|期間の配列。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeConstraint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/timeconstraint.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->