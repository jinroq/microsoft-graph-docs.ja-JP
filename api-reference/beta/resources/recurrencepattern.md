# <a name="recurrencepattern-resource-type"></a>recurrencePattern リソースの種類

イベントの頻度。


## <a name="properties"></a>プロパティ
| プロパティ       | 型    |説明|
|:---------------|:--------|:----------|
|dayOfMonth|Int32|イベントが発生する月の日付。|
|daysOfWeek|String collection|イベントが発生する曜日のコレクションです。可能な値は、`Sunday`、`Monday`、`Tuesday`、`Wednesday`、`Thursday`、`Friday`、`Saturday` です。|
|firstDayOfWeek|String|定期的なアイテムが開始される曜日です。可能な値は、`Sunday`、`Monday`、`Tuesday`、`Wednesday`、`Thursday`、`Friday`、`Saturday` です。|
|index|String|定期的なアイテムが発生する曜日のインデックス: `First`、`Second`、`Third`、`Fourth`、`Last`。|
|interval|Int32|発生と発生の間の指定された繰り返しタイプの単位数。|
|month|Int32|イベントが発生する月。これは、1 から 12 までの数字です。|
|型|String|定期的なパターンの種類: `Daily`、`Weekly`、`AbsoluteMonthly`、`RelativeMonthly`、`AbsoluteYearly`、`RelativeYearly`。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recurrencepattern"
}-->

```json
{
  "dayOfMonth": 1024,
  "daysOfWeek": ["String"],
  "firstDayOfWeek": "String",
  "index": "String",
  "interval": 1024,
  "month": 1024,
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "recurrencePattern resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->