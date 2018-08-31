# <a name="tablecolumn-resource-type"></a>TableColumn リソースの種類

テーブル内にある 1 つの列を表します。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[TableColumn を取得する](../api/tablecolumn_get.md) | [WorkbookTableColumn](tablecolumn.md) |tableColumn オブジェクトのプロパティと関係を読み取ります。|
|[更新する](../api/tablecolumn_update.md) | [WorkbookTableColumn](tablecolumn.md) |TableColumn オブジェクトを更新します。 |
|[Databodyrange](../api/tablecolumn_databodyrange.md)|[範囲](range.md)|列のデータ本体に関連付けられた範囲オブジェクトを取得します。|
|[Headerrowrange](../api/tablecolumn_headerrowrange.md)|[範囲](range.md)|列のヘッダー行に関連付けられた範囲オブジェクトを取得します。|
|[範囲](../api/tablecolumn_range.md)|[範囲](range.md)|列全体に関連付けられた範囲オブジェクトを取得します。|
|[Totalrowrange](../api/tablecolumn_totalrowrange.md)|[範囲](range.md)|列の集計行に関連付けられた範囲オブジェクトを取得します。|
|[削除する](../api/tablecolumn_delete.md)|なし|テーブルから列を削除します。|
|[リスト](../api/tablecolumn_list.md) | [WorkbookTableColumn](tablecolumn.md) コレクション |tableColumn オブジェクトのコレクションを取得します。 |
|[Itemat](../api/tablecolumncollection_itemat.md)|[WorkbookTableColumn](tablecolumn.md)|コレクション内の位置に基づいて列を取得します。|
|[追加する](../api/tablecolumncollection_add.md)|[WorkbookTableColumn](tablecolumn.md)|テーブルに新しい列を追加します。|

## <a name="properties"></a>プロパティ
| プロパティ     | タイプ   |説明|
|:---------------|:--------|:----------|
|ID|文字列|テーブル内の列を識別する一意のキーを返します。 このプロパティは符号化文字列値として解釈し、その他の型に解析すべきではありません。 読み取り専用。|
|インデックス|int|テーブルの列コレクション内の列のインデックス番号を返します。0 を起点とする番号になります。読み取り専用です。|
|名前|文字列|テーブル列の名前を取得します。読み取り専用です。|
|値|Json|指定した範囲の Raw 値を表します。返されるデータの型は、文字列、数値、またはブール値のいずれかになります。エラーが含まれているセルは、エラー文字列を返します。|

## <a name="relationships"></a>関係
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|フィルター|[WorkbookFilter](filter.md)|列に適用されるフィルターを取得します。読み取り専用です。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookTableColumn"
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
