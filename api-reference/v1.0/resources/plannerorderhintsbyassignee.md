---
title: plannerOrderHintsByAssignee リソースの種類
description: '**PlannerOrderHintsByAssignee**は、タスクに割り当てられたタスクの順序を示すために、タスクリソースの担当者の注文ヒントを含むリソースです。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: c4c5099485c75c41e9ebb6275a7ffa5fed3be5a2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035232"
---
# <a name="plannerorderhintsbyassignee-resource-type"></a>plannerOrderHintsByAssignee リソースの種類

**PlannerOrderHintsByAssignee**は、タスクに割り当てられたタスクの順序を示すために、[タスク](plannertask.md)リソースの担当者の注文[ヒント](planner-order-hint-format.md)を含むリソースです。
この型はオープン型です。 プロパティは、タスクに割り当てられたユーザーの id であり、値は order ヒントです。

## <a name="properties"></a>プロパティ
オープン型のプロパティは、クライアントで定義できます。 この場合、クライアントは、タスクに割り当てられているユーザーの id をプロパティ名として指定し、有効な[順序ヒント](planner-order-hint-format.md)を値として指定する必要があります。
プロパティをこの型から削除することはできません。 このサービスは、を含む[プランのタスク](plannertask.md)が更新されたときに、自動的に値を削除します。

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
