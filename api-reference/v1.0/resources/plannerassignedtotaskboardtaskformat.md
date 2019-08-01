---
title: plannerAssignedToTaskBoardTaskFormat リソースの種類
description: '**PlannerAssignedToTaskBoardTaskFormat**リソースは、タスクボードの担当者ビューでタスクを正しくレンダリングするために使用される情報を表します (タスクが割り当てられるユーザーによって整理されたビュー)。 各タスクには、1つの**plannerAssignedToTaskBoardTaskFormat**オブジェクトが関連付けられています。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: c85a68a3a9c17a35bc94ee32ebff156198029bed
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035351"
---
# <a name="plannerassignedtotaskboardtaskformat-resource-type"></a>plannerAssignedToTaskBoardTaskFormat リソースの種類

**PlannerAssignedToTaskBoardTaskFormat**リソースは、タスクボードの担当者ビューでタスクを正しくレンダリングするために使用される情報を表します (タスクが割り当てられるユーザーによって整理されたビュー)。 各[タスク](plannertask.md)には、1つの**plannerAssignedToTaskBoardTaskFormat**オブジェクトが関連付けられています。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[Get plannerAssignedToTaskBoardTaskFormat](../api/plannerassignedtotaskboardtaskformat-get.md) | [plannerAssignedToTaskBoardTaskFormat](plannerassignedtotaskboardtaskformat.md) |**PlannerAssignedToTaskBoardTaskFormat**オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Update](../api/plannerassignedtotaskboardtaskformat-update.md) | [plannerAssignedToTaskBoardTaskFormat](plannerassignedtotaskboardtaskformat.md)  |**PlannerAssignedToTaskBoardTaskFormat**オブジェクトを更新します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|id|String| 読み取り専用です。 リソースの ID。 28 文字長で、大文字と小文字の区別があります。 [書式検証](planner-identifiers-disclaimer.md)はサービスによって行われます。|
|orderHintsByAssignee|[plannerOrderHintsByAssignee](plannerorderhintsbyassignee.md)|タスク ボードの AssignedTo ビューでのタスクの順序付けに使用するヒントのディクショナリ。各エントリのキーは、タスクが割り当てられているユーザーのいずれかであり、値は順序のヒントです。それぞれの値の形式は[ここ](planner-order-hint-format.md)で説明するとおり定義されます。|
|unassignedOrderHint|String|タスクが誰にも割り当てられていない場合、または orderHintsByAssignee ディクショナリに、タスクが割り当てられているユーザーのヒントの順序が指定されない場合に、タスク ボードの AssignedTo ビューでのタスクの順序付けに使用するヒントの値。形式は[ここ](planner-order-hint-format.md)の説明に従って定義されます。|

## <a name="relationships"></a>リレーションシップ
なし


## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.plannerAssignedToTaskBoardTaskFormat"
}-->

```json
{
  "id": "String (identifier)",
  "orderHintsByAssignee": {"@odata.type": "microsoft.graph.plannerOrderHintsByAssignee"},
  "unassignedOrderHint": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerAssignedToTaskBoardTaskFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
