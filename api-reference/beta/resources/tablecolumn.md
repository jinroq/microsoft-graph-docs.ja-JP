# <a name="tablecolumn-resource-type"></a>TableColumn リソースの種類

テーブル内にある 1 つの列を表します。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[TableColumn を取得する](../api/tablecolumn_get.md) | [TableColumn](tablecolumn.md) |tableColumn オブジェクトのプロパティと関係を読み取ります。|
|[Update](../api/tablecolumn_update.md) | [TableColumn](tablecolumn.md)    |TableColumn オブジェクトを更新します。 |
|[Databodyrange](../api/tablecolumn_databodyrange.md)|[Range](range.md)|列のデータ本体に関連付けられた範囲オブジェクトを取得します。|
|[Headerrowrange](../api/tablecolumn_headerrowrange.md)|[Range](range.md)|列のヘッダー行に関連付けられた範囲オブジェクトを取得します。|
|[Range](../api/tablecolumn_range.md)|[Range](range.md)|列全体に関連付けられた範囲オブジェクトを取得します。|
|[Totalrowrange](../api/tablecolumn_totalrowrange.md)|[Range](range.md)|列の集計行に関連付けられた範囲オブジェクトを取得します。|
|[Delete](../api/tablecolumn_delete.md)|なし|テーブルから列を削除します。|
|[List](../api/tablecolumn_list.md) | [TableColumn](tablecolumn.md) コレクション |tableColumn オブジェクトのコレクションを取得します。 |
|[Itemat](../api/tablecolumncollection_itemat.md)|[TableColumn](tablecolumn.md)|コレクション内の位置に基づいて列を取得します。|
|[Add](../api/tablecolumncollection_add.md)|[TableColumn](tablecolumn.md)|テーブルに新しい列を追加します。|


## <a name="properties"></a>プロパティ
| プロパティ       | 型    |説明|
|:---------------|:--------|:----------|
|id|int|テーブル内の列を識別する一意のキーを返します。読み取り専用です。|
|index|int|テーブルの列コレクション内の列のインデックス番号を返します。0 を起点とする番号になります。読み取り専用です。|
|name|string|テーブル列の名前を取得します。読み取り専用です。|
|values|json|指定した範囲の Raw 値を表します。返されるデータの型は、文字列、数値、またはブール値のいずれかになります。エラーが含まれているセルは、エラー文字列を返します。|

## <a name="relationships"></a>関係
| リレーションシップ | 型    |説明|
|:---------------|:--------|:----------|
|filter|[Filter](filter.md)|列に適用されるフィルターを取得します。読み取り専用です。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.tableColumn"
}-->

```json
{
  "id": 1024,
  "index": 1024,
  "name": "string",
  "values": "json"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableColumn resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->