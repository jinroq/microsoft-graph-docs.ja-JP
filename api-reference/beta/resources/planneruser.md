<a id="planneruser-resource-type" class="xliff"></a>
# plannerUser リソースの種類

**plannerUser** リソースは、[user](user.md) のプランナー リソースへのアクセスを提供します。使用可能なプロパティは含まれていません。


<a id="methods" class="xliff"></a>
## メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[plans を一覧表示する](../api/planneruser_list_plans.md) |[plannerPlan](plannerplan.md) コレクション| **plannerPlan** オブジェクト コレクションを取得します。|
|[List tasks](../api/planneruser_list_tasks.md) |[plannerTask](plannertask.md) コレクション| **plannerTask** オブジェクト コレクションを取得します。|

<a id="properties" class="xliff"></a>
## プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|id|String| 読み取り専用です。planenrUser の識別子|

<a id="relationships" class="xliff"></a>
## リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|plans|[plannerPlan](plannerplan.md) コレクション| 読み取り専用です。Null 許容型。ユーザーに割り当てられている [plannerTasks](plannertask.md) を返します。|
|tasks|[plannerTask](plannertask.md) コレクション| 読み取り専用です。Null 許容型。ユーザーと共有している [plannerPlans](plannerplan.md) を返します。|

<a id="json-representation" class="xliff"></a>
## JSON 表記
以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerUser"
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
  "description": "plannerUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->