# <a name="timestamp-resource-type"></a>timestamp のリソースの種類

時間のポイントの日付と時刻情報です。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeStamp"
}-->

```json
{
  "date": "String (timestamp)",
  "time": "String (timestamp)",
  "timeZone": "string"
}

```
## <a name="properties"></a>プロパティ
| プロパティ       | タイプ    |説明|
|:---------------|:--------|:----------|
|date|日付|タイムスタンプの日付部分。|
|time|TimeOfDay|タイムスタンプの時刻部分。|
|timeZone|文字列|timestamp のタイム ゾーン部分。世界を 24 個の縦方向の領域に分けたうちのいずれかの領域です。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeStamp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->