---
title: timeConstraint リソースの種類
description: 指定されたアクティビティの性質および開いている時間帯に従って、会議時間の提案を特定の時間と曜日に制限します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 8393e4b501815dcbd0195e04ca82cd639d1a84c8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964320"
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
  "suppressions": []
}
-->
