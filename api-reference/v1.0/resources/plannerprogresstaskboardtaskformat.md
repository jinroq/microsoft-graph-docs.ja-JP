# <a name="plannerprogresstaskboardtaskformat-resource-type"></a>plannerProgressTaskBoardTaskFormat リソースの種類

**plannerProgressTaskBoardTaskFormat** リソースは、タスク ボードの進行状況ビューにタスクを正しく表示するための情報を示します (ビューはタスク オブジェクトの [未開始]、[処理中]、[完了] の列に示す PercentComplete フィールドの状態で整理されます)。各 [task](plannertask.md) にはそれぞれ **plannerProgressTaskBoardTaskFormat** オブジェクトが 1 つ関連付けられています。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[plannerProgressTaskBoardTaskFormat の取得](../api/plannerprogresstaskboardtaskformat_get.md) | [plannerProgressTaskBoardTaskFormat](plannerprogresstaskboardtaskformat.md) |**plannerProgressTaskBoardTaskFormat** オブジェクトのプロパティとリレーションシップを読み取ります。|
|[更新](../api/plannerprogresstaskboardtaskformat_update.md) | [plannerProgressTaskBoardTaskFormat](plannerprogresstaskboardtaskformat.md)    |**plannerProgressTaskBoardTaskFormat** オブジェクトを更新します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | タイプ   |説明|
|:---------------|:--------|:----------|
|ID|文字列| 読み取り専用。 リソースの ID。 28 文字で大文字小文字を区別します。 サービスの[フォーマットの検証](planner_identifiers_disclaimer.md) が行われます。|
|orderHint|文字列|タスク ボードの進行状況ビューでタスクの順序付けに使用するヒントの値。形式は[ここ](planner_order_hint_format.md)の説明に従って定義されます。|

## <a name="relationships"></a>リレーションシップ
なし


## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.plannerProgressTaskBoardTaskFormat"
}-->

```json
{
  "id": "String (identifier)",
  "orderHint": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerProgressTaskBoardTaskFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->