# <a name="rangefont-resource-type"></a>RangeFont リソースの種類

このオブジェクトは、オブジェクトのフォントの属性 (フォント名、フォント サイズ、色など) を表します。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[Get RangeFont](../api/rangefont_get.md) | [WorkbookRangeFont](rangefont.md) |rangeFont オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Update](../api/rangefont_update.md) | [WorkbookRangeFont](rangefont.md)   |RangeFont オブジェクトを更新します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | タイプ   |説明|
|:---------------|:--------|:----------|
|bold|boolean|フォントの太字の状態を表します。|
|color|string|テキストの色の HTML カラー コード表記。たとえば、#FF0000 は赤を表します。|
|italic|boolean|フォントの斜体の状態を表します。|
|name|string|フォント名 (例: "Calibri")|
|size|double|フォント サイズ|
|underline|string|フォントに適用する下線の種類です。 可能な値は、`None`、`Single`、`Double`、`SingleAccountant`、`DoubleAccountant` です。|

## <a name="relationships"></a>リレーションシップ
なし


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookRangeFont"
}-->

```json
{
  "bold": true,
  "color": "string",
  "italic": true,
  "name": "string",
  "size": 1024,
  "underline": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeFont resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->