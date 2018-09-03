# <a name="tablesort-resource-type"></a>TableSort リソースの種類

テーブル オブジェクトの並べ替え操作を管理します。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[Get TableSort](../api/tablesort_get.md) | [WorkbookTableSort](tablesort.md) |tableSort オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Apply](../api/tablesort_apply.md)|なし|並べ替え操作を実行します。|
|[Clear](../api/tablesort_clear.md)|なし|テーブルに現在設定されている並べ替えをクリアします。これにより表の順序が変更されることはありませんが、ヘッダーのボタンの状態がクリアされます。|
|[Reapply](../api/tablesort_reapply.md)|なし|テーブルに、現在の並べ替えパラメーターを再適用します。|

## <a name="properties"></a>プロパティ
| プロパティ     | タイプ   |説明|
|:---------------|:--------|:----------|
|fields|[WorkbookSortField](sortfield.md) コレクション|テーブルの最後の並べ替え操作に使用する現在の条件を表します。読み取り専用です。|
|matchCase|boolean|大文字小文字の区別が、テーブルの最後の並べ替え操作に影響を与えたかどうかを表します。読み取り専用です。|
|method|string|テーブルの最後の並べ替え操作に使用される中国語文字の順序の指定方法を表します。 可能な値は、`PinYin`、`StrokeCount` です。 読み取り専用。|

## <a name="json-representation"></a>JSON 表現

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookTableSort"
}-->

```json
{
  "matchCase": true,
  "method": "string",
  "fields": [{ "@odata.type": "microsoft.graph.workbookSortField" }]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableSort resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->