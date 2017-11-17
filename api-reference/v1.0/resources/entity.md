# <a name="entity-resource-type"></a>エンティティ リソースの種類


## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[エンティティを取得する](../api/entity_get.md) | [entity](entity.md) |エンティティ オブジェクトのプロパティと関係を読み取ります。|
|[Delete](../api/entity_delete.md) | なし |エンティティ オブジェクトを削除します。 |

## <a name="properties"></a>プロパティ
| プロパティ       | 型    |説明|
|:---------------|:--------|:----------|
|id|String| 読み取り専用です。|

## <a name="relationships"></a>関係
なし





## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.entity"
}-->

```json
{
  "id": "string (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "entity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->