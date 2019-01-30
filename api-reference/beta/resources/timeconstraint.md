---
title: timeConstraint リソースの種類
description: 指定したアクティビティの性質と空き時間帯に従って、会議の日時の候補を、特定の時間と曜日に限定します。
localization_priority: Normal
ms.openlocfilehash: 88035d0617523c51bb01ee0a467e8c84785ad6aa
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643567"
---
# <a name="timeconstraint-resource-type"></a>timeConstraint リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

指定したアクティビティの性質と空き時間帯に従って、会議の日時の候補を、特定の時間と曜日に限定します。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeconstraint"
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
|activityDomain|String|アクティビティの性質です (省略可能)。使用可能な値: `work`、`personal`、`unrestricted`、`unknown`。|
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
