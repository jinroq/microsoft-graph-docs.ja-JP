# planner リソースの種類
<a id="planner-resource-type" class="xliff"></a>

**planner** リソースは Planner オブジェクト モデルのエントリ ポイントです。単一の **planner** リソースを返します。使用可能なプロパティは含まれていません。


## メソッド
<a id="methods" class="xliff"></a>

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[Create plannerBucket](../api/planner_post_buckets.md) |[plannerBucket](plannerbucket.md)| バケット コレクションの投稿によって新しい **plannerBucket** を作成します。|
|[Create plannerPlan](../api/planner_post_plans.md) |[plannerPlan](plannerplan.md)| 計画コレクションの投稿によって新しい **plannerPlan** を作成します。|
|[Create plannerTask](../api/planner_post_tasks.md) |[plannerTask](plannertask.md)| タスク コレクションの投稿によって新しい **plannerTask** を作成します。|

## プロパティ
<a id="properties" class="xliff"></a>
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|id|String| 読み取り専用です。**planner** リソースの識別子。|

## リレーションシップ
<a id="relationships" class="xliff"></a>
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|buckets|[plannerBucket](plannerbucket.md) コレクション| 読み取り専用です。Null 許容型。指定されたバケットのコレクションを返します|
|plans|[plannerPlan](plannerplan.md) コレクション| 読み取り専用です。Null 許容型。指定された計画のコレクションを返します|
|tasks|[plannerTask](plannertask.md) コレクション| 読み取り専用です。Null 許容型。指定されたタスクのコレクションを返します|

## JSON 表記
<a id="json-representation" class="xliff"></a>
以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.planner"
}-->

```json
{
  "id": "String (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "planner resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->