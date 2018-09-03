# <a name="tablerow-resource-type"></a>TableRow リソースの種類

表の行を表します。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[TableRow を取得する](../api/tablerow_get.md) | [WorkbookTableRow](tablerow.md) |tableRow オブジェクトのプロパティと関係を読み取ります。|
|[更新する](../api/tablerow_update.md) | [WorkbookTableRow](tablerow.md)  |TableRow を更新します。 |
|[範囲](../api/tablerow_range.md)|[範囲](range.md)|行全体に関連付けられた範囲オブジェクトを返します。|
|[削除](../api/tablerow_delete.md)|なし|テーブルから行を削除します。|
|[リスト](../api/tablerow_list.md) | [WorkbookTableRow](tablerow.md) コレクション |tableRow オブジェクトのコレクションを取得します。 |
|[Itemat](../api/tablerowcollection_itemat.md)|[WorkbookTableRow](tablerow.md)|コレクション内の位置を基に行を取得します。|
|[追加](../api/tablerowcollection_add.md)|[WorkbookTableRow](tablerow.md)|新しい行をテーブルに追加します。|

## <a name="properties"></a>プロパティ
| プロパティ     | タイプ   |説明|
|:---------------|:--------|:----------|
|index|int|テーブルの行コレクション内の行のインデックス番号を返します。0 を起点とする番号になります。読み取り専用。|
|values|Json|指定した範囲の Raw 値を表します。返されるデータの型は、文字列、数値、またはブール値のいずれかになります。エラーが含まれているセルは、エラー文字列を返します。|

## <a name="relationships"></a>関係
なし


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookTableRow"
}-->

```json
{
  "index": 1024,
  "values": "json"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableRow resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->