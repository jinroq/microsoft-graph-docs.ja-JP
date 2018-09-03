# <a name="plannerassignedtotaskboardtaskformat-resource-type"></a>plannerAssignedToTaskBoardTaskFormat リソースの種類

**PlannerAssignedToTaskBoardTaskFormat** リソースは、タスク ボードの AssignedTo ビューを正しく表示するための情報を示します (ビューはタスクが割り当てられているユーザーごとに整理されます)。各 [task](plannertask.md) にはそれぞれ **plannerAssignedToTaskBoardTaskFormat** オブジェクトが 1 つ関連付けられています。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[plannerAssignedToTaskBoardTaskFormat の取得](../api/plannerassignedtotaskboardtaskformat_get.md) | [plannerAssignedToTaskBoardTaskFormat](plannerassignedtotaskboardtaskformat.md) |**plannerAssignedToTaskBoardTaskFormat** オブジェクトのプロパティとリレーションシップを読み取ります。|
|[更新する](../api/plannerassignedtotaskboardtaskformat_update.md) | [plannerAssignedToTaskBoardTaskFormat](plannerassignedtotaskboardtaskformat.md)  |**plannerAssignedToTaskBoardTaskFormat** オブジェクトを更新します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | タイプ   |説明|
|:---------------|:--------|:----------|
|ID|文字列| 読み取り専用。 リソースの ID。 28 文字で大文字小文字を区別します。 サービスの[フォーマットの検証](planner_identifiers_disclaimer.md) が行われます。|
|orderHintsByAssignee|[plannerOrderHintsByAssignee](plannerorderhintsbyassignee.md)|タスク ボードの AssignedTo ビューでのタスクの順序付けに使用するヒントのディクショナリ。各エントリのキーは、タスクが割り当てられているユーザーのいずれかであり、値は順序のヒントです。それぞれの値の形式は[ここ](planner_order_hint_format.md)で説明するとおり定義されます。|
|unassignedOrderHint|文字列|タスクが誰にも割り当てられていない場合、または orderHintsByAssignee ディクショナリに、タスクが割り当てられているユーザーのヒントの順序が指定されない場合に、タスク ボードの AssignedTo ビューでのタスクの順序付けに使用するヒントの値。形式は[ここ](planner_order_hint_format.md)の説明に従って定義されます。|

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