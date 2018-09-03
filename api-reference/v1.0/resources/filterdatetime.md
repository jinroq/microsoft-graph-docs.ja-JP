# <a name="filterdatetime-resource-type"></a>FilterDatetime リソースの種類

値をフィルター処理するときに日付をフィルター処理する方法を表します。

## <a name="properties"></a>プロパティ
| プロパティ     | タイプ   |説明|
|:---------------|:--------|:----------|
|日付|文字列|データをフィルターをかけるための ISO8601 形式の日付です。|
|特定性|文字列|データを保持するのに、日付をどの程度詳細に使用するか。 たとえば、日付が 2005-04-02 で "month" に設定した場合、フィルター操作では 2009 年 4 月の日付データを含むすべての行が保持されます。 指定できる値は、  `Year`、`Monday`、`Day`、`Hour`、`Minute`、`Second` です。|

## <a name="relationships"></a>リレーションシップ
なし


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookFilterDateTime"
}-->

```json
{
  "date": "string",
  "specificity": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "FilterDatetime resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->