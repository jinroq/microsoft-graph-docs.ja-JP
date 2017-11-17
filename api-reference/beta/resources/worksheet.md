# <a name="worksheet-resource-type"></a>ワークシート リソースの種類

Excel のワークシートは、セルのグリッドになっています。そこに、データ、表、グラフなどを含めることができます。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[ワークシートを取得する](../api/worksheet_get.md) | [Worksheet](worksheet.md) |ワークシート オブジェクトのプロパティと関係を読み取ります。|
|[グラフを作成する](../api/worksheet_post_charts.md) |[Chart](chart.md)| グラフ コレクションに投稿して、新しいグラフを作成します。|
|[名前を一覧表示する](../api/worksheet_list_names.md) |[NamedItem](nameditem.md) コレクション| ワークシートに関連付けられている名前付きのアイテムのコレクションを取得します。|
|[グラフを一覧表示する](../api/worksheet_list_charts.md) |[Chart](chart.md) コレクション| グラフ オブジェクトのコレクションを取得します。|
|[テーブルを作成する](../api/worksheet_post_tables.md) |[Table](table.md)| テーブル コレクションに投稿して、新しいテーブルを作成します。|
|[テーブルを一覧表示する](../api/worksheet_list_tables.md) |[Table](table.md) コレクション| テーブル オブジェクトのコレクションを取得します。|
|[Update](../api/worksheet_update.md) | [Worksheet](worksheet.md)    |ワークシート オブジェクトを更新します。 |
|[Cell](../api/worksheet_cell.md)|[Range](range.md)|行と列の番号に基づいて、1 つのセルを含んだ範囲オブジェクトを取得します。このセルは、ワークシートのグリッド内であれば、親の範囲の境界の外のセルであってもかまいません。|
|[Range](../api/worksheet_range.md)|[Range](range.md)|アドレスまたは名前で指定された範囲オブジェクトを取得します。|
|[Usedrange](../api/worksheet_usedrange.md)|[Range](range.md)|使用範囲とは、値または書式設定が割り当たっているすべてのセルを包含する最小の範囲です。ワークシートが空白の場合、この関数は左上のセルを返します。|
|[Delete](../api/worksheet_delete.md)|なし|ブックからワークシートを削除します。|
|[List](../api/worksheet_list.md) | [Worksheet](worksheet.md) コレクション |ワークシート オブジェクトのコレクションを取得します。 |
|[Add](../api/worksheetcollection_add.md)|[Worksheet](worksheet.md)|新しいワークシートをブックに追加します。ワークシートは、既存のワークシートの末尾に追加されます。 |
|[pivotTables を一覧表示する](../api/workbookworksheet_list_pivottables.md) |[workbookPivotTable](workbookpivottable.md) コレクション| workbookPivotTable オブジェクト コレクションを取得します。|

## <a name="properties"></a>プロパティ
| プロパティ       | 型    |説明|
|:---------------|:--------|:----------|
|id|string|指定されたブックのワークシートを一意に識別する値を返します。この識別子の値は、ワークシートの名前を変更したり移動したりしても同じままです。値の取得のみ可能です。|
|name|string|ワークシートの表示名。|
|position|int|0 を起点とした、ブック内のワークシートの位置。|
|visibility|string|ワークシートの可視性。可能な値は、`Visible`、`Hidden`、`VeryHidden` です。|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型    |説明|
|:---------------|:--------|:----------|
|charts|[Chart](chart.md) コレクション|ワークシートの一部になっているグラフのコレクションを返します。読み取り専用です。|
|names|[NamedItem](nameditem.md) コレクション|ワークシートに関連付けられている名前のコレクションを返します。読み取り専用です。|
|pivotTables|[workbookPivotTable](workbookpivottable.md) コレクション| ワークシートの一部になっているピボットテーブルのコレクション。 |
|protection|[WorksheetProtection](worksheetprotection.md)|ワークシートのシート保護オブジェクトを返します。読み取り専用です。|
|tables|[Table](table.md) コレクション|ワークシートの一部になっているグラフのコレクション。値の取得のみ可能です。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.worksheet"
}-->

```json
{
  "id": "string",
  "name": "string",
  "position": 1024,
  "visibility": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Worksheet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
