# <a name="sizerange-resource-type"></a>sizeRange リソースの種類


条件または例外を適用するために、受信メッセージに想定される最小サイズと最大サイズ (単位: キロバイト) を指定します。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
| maximumSize | Int32 | 条件または例外を適用するために、受信メッセージに想定される最大サイズ (単位: キロバイト)。 |
| minimumSize | Int32 | 条件または例外を適用するために、受信メッセージに想定される最小サイズ (単位: キロバイト)。 |


## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
   ],
  "@odata.type": "microsoft.graph.sizeRange"
}-->

```json
{
  "maximumSize": "Int32",
  "minimumSize": "Int32"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sizeRange resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->