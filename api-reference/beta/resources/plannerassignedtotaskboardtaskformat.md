---
title: plannerAssignedToTaskBoardTaskFormat リソースの種類
description: '**plannerAssignedToTaskBoardTaskFormat**リソースは、タスクボードの担当者ビューでタスクを正しくレンダリングするために使用される情報を表します (タスクが割り当てられるユーザーによって整理されたビュー)。 各タスクには、1つの**plannerAssignedToTaskBoardTaskFormat**オブジェクトが関連付けられています。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 6a7aa230a610ec63559797d058cbc3f64ffe843d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32461193"
---
# <a name="plannerassignedtotaskboardtaskformat-resource-type"></a>plannerAssignedToTaskBoardTaskFormat リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**plannerAssignedToTaskBoardTaskFormat**リソースは、タスクボードの担当者ビューでタスクを正しくレンダリングするために使用される情報を表します (タスクが割り当てられるユーザーによって整理されたビュー)。 各[タスク](plannertask.md)には、1つの**plannerAssignedToTaskBoardTaskFormat**オブジェクトが関連付けられています。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[Get plannerAssignedToTaskBoardTaskFormat](../api/plannerassignedtotaskboardtaskformat-get.md) | [plannerAssignedToTaskBoardTaskFormat](plannerassignedtotaskboardtaskformat.md) |**plannerAssignedToTaskBoardTaskFormat**オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Update](../api/plannerassignedtotaskboardtaskformat-update.md) | [plannerAssignedToTaskBoardTaskFormat](plannerassignedtotaskboardtaskformat.md)  |**plannerAssignedToTaskBoardTaskFormat**オブジェクトを更新します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|id|String| 読み取り専用です。 リソースの ID。 28 文字長で、大文字と小文字の区別があります。 [書式検証](tasks-identifiers-disclaimer.md)はサービスによって行われます。|
|orderHintsByAssignee|[plannerOrderHintsByAssignee](plannerorderhintsbyassignee.md)|タスク ボードの AssignedTo ビューでのタスクの順序付けに使用するヒントのディクショナリ。各エントリのキーは、タスクが割り当てられているユーザーのいずれかであり、値は順序のヒントです。それぞれの値の形式は[ここ](planner-order-hint-format.md)で説明するとおり定義されます。|
|unassignedOrderHint|String|タスクが誰にも割り当てられていない場合、または orderHintsByAssignee ディクショナリに、タスクが割り当てられているユーザーのヒントの順序が指定されない場合に、タスク ボードの AssignedTo ビューでのタスクの順序付けに使用するヒントの値。形式は[ここ](planner-order-hint-format.md)の説明に従って定義されます。|

## <a name="relationships"></a>リレーションシップ
なし


## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
<!--
{
  "type": "#page.annotation",
  "description": "plannerAssignedToTaskBoardTaskFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerassignedtotaskboardtaskformat.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
