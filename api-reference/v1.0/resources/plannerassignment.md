---
title: plannerAssignment リソースの種類
description: '**PlannerAssignment**リソースでは、ユーザーにタスクの割り当てを表します。 この型がオープン型の plannerAssignments で使用されます。'
localization_priority: Normal
ms.openlocfilehash: a2766653fdd7fe29c40529e77bbff2c72e8e6be7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27875685"
---
# <a name="plannerassignment-resource-type"></a>plannerAssignment リソースの種類

**PlannerAssignment** リソースは、ユーザーに対するタスクの割り当てを表します。この種類は、オープン型の [plannerAssignments](plannerassignments.md) で使用されます。


## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|assignedBy|[identitySet](identityset.md)|assignor など、タスクの割り当てを実行したユーザーの ID。|
|assignedDateTime|DateTimeOffset|タスクが割り当てられた時間。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|orderHint|String|タスクの担当者を並べ替えるために使用するヒント。形式は[ここ](planner-order-hint-format.md)の説明に従って定義されます。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerAssignment"
}-->

```json
{
  "assignedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "assignedDateTime": "String (timestamp)",
  "orderHint": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
