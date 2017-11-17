# <a name="alternativesecurityid-resource-type"></a>alternativeSecurityId リソースの種類

デバイスに関連付けられている代替のセキュリティ ID が含まれています。[デバイス](device.md) エンティティの **alternativeSecurityIds** プロパティは、**alternativeSecurityId** のコレクションです。

## <a name="properties"></a>プロパティ
| プロパティ       | 型    |説明|
|:---------------|:--------|:----------|
|identityProvider|String|            |
|key|Binary|            |
|type|Int32|            |


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.alternativeSecurityId"
}-->

```json
{
  "identityProvider": "string",
  "key": "binary",
  "type": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "alternativeSecurityId resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
