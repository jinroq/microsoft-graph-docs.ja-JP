# <a name="recurrencerange-resource-type"></a>recurrenceRange リソースの種類

イベントの期間。

## <a name="properties"></a>プロパティ

| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|endDate|Date|繰り返しの終了日です。|
|numberOfOccurrences|Int32|イベントを繰り返す回数。|
|recurrenceTimeZone|String |**startDate** プロパティと **endDate** プロパティのタイム ゾーン。 |
|startDate|Date|繰り返しの開始日です。|
|type|String|次のような繰り返し範囲があります。終了日 = 0、無制限 = 1、番号順 = 2。可能な値は、`EndDate`、`NoEnd`、`Numbered` です。||

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recurrencerange"
}-->

```json
{
  "endDate": "String (timestamp)",
  "numberOfOccurrences": 1024,
  "recurrenceTimeZone": "string",
  "startDate": "String (timestamp)",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "recurrenceRange resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
