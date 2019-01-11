---
title: plannerOrderHintsByAssignee リソースの種類
description: '**PlannerOrderHintsByAssignee**は、タスクの掲示板のビューに割り当てられているタスクの順序を示すために、plannerTask のリソースの割り当て先の命令のヒントを含むリソースです。'
localization_priority: Normal
ms.openlocfilehash: 2de8b7d7fac6b524cccbed8ed2117754060c0d4c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816535"
---
# <a name="plannerorderhintsbyassignee-resource-type"></a>plannerOrderHintsByAssignee リソースの種類

**plannerOrderHintsByAssignee** には、タスク ボードの [割り当て先ユーザー/グループ] ビューのタスクの順序を示す、[plannerTask](plannertask.md) リソースの担当者の[順序に関するヒント](planner-order-hint-format.md)が含まれます。この型はオープン型です。プロパティは、タスクに割り当てられているユーザーの ID で、値は順序のヒントです。

## <a name="properties"></a>プロパティ
クライアントは、オープン型のプロパティを定義できます。この場合、クライアントは、タスクに割り当てられているユーザーの ID をプロパティ名として指定し、有効な[順序のヒント](planner-order-hint-format.md)を値として指定する必要があります。プロパティは、この型から削除できません。サービスは、含まれている [plannerTask](plannertask.md) の割り当てが更新されると、値を自動的に削除します

例:

<!-- {
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [ "ca2a1df2-e36b-4987-9f6b-0ea462f4eb47", "4e98f8f1-bb03-4015-b8e0-19bb370949d8" ],
  "@odata.type": "microsoft.graph.plannerOrderHintsByAssignee"
}-->

```json
{
  "ca2a1df2-e36b-4987-9f6b-0ea462f4eb47": "String",
  "4e98f8f1-bb03-4015-b8e0-19bb370949d8": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerOrderHintsByAssignee resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
