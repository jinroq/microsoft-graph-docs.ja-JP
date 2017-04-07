# <a name="responsestatus-resource-type"></a>responseStatus リソースの種類

会議出席依頼の応答状態です。


## <a name="properties"></a>プロパティ
| プロパティ       | 型    |説明|
|:---------------|:--------|:----------|
|response|String|次のような応答タイプがあります。なし = 0、主催者 = 1、一時承諾 = 2、承諾 = 3、辞退 = 4、無応答 = 5。可能な値は、`None`、`Organizer`、`TentativelyAccepted`、`Accepted`、`Declined`、`NotResponded` です。|
|time|DateTimeOffset|応答が返された日時。ISO 8601 形式を使って表され、常に UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.responseStatus"
}-->
```json
{
  "response": "String",
  "time": "String (timestamp)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "responseStatus resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
