# <a name="plannerbucket-resource-type"></a>plannerBucket リソースの種類

**PlannerBucket** リソースは、Office 365 の計画におけるタスクのバケット (または "カスタム列") を表します。これは [plannerPlan](plannerPlan.md) に含まれており、[plannerTasks](plannerTask.md) のコレクションを持ちます。



## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[plannerBucket の取得](../api/plannerbucket_get.md) | [plannerBucket](plannerbucket.md) |**plannerBucket** オブジェクトのプロパティとリレーションシップを読み取ります。|
|[plannerTasks のリスト](../api/plannerbucket_list_tasks.md) |[plannerTask](plannertask.md) コレクション| **plannerTask** オブジェクト コレクションを取得します。|
|[作成](../api/planner_post_buckets.md) | [plannerBucket](plannerbucket.md)   | 新しい **plannerBucket** オブジェクトを作成します。 |
|[更新](../api/plannerbucket_update.md) | [plannerBucket](plannerbucket.md)   |**plannerBucket** オブジェクトを更新します。 |
|[削除](../api/plannerbucket_delete.md) | なし |**plannerBucket** オブジェクトを削除します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | タイプ   |説明|
|:---------------|:--------|:----------|
|id|文字列| 読み取り専用。 バケットの ID です。 28 文字で大文字小文字を区別します。 サービスの[フォーマットの検証](planner_identifiers_disclaimer.md) が行われます。|
|name|文字列|バケットの名前。|
|orderHint|文字列|リスト ビューでこの種類の項目の順序付けに使用するヒント。形式は[ここ](planner_order_hint_format.md)の説明に従って定義されます。|
|planId|文字列|バケットが所属する計画の ID。|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|tasks|[plannerTask](plannertask.md) コレクション| 読み取り専用です。Null 許容型。バケットに含まれるタスクのコレクション。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerBucket"
}-->

```json
{
  "id": "String (identifier)",
  "name": "String",
  "orderHint": "String",
  "planId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerBucket resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->