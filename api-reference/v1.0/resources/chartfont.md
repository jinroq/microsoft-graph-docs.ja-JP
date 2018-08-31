# <a name="chartfont-resource-type"></a>ChartFont リソースの種類

このオブジェクトは、グラフ オブジェクトのフォント属性 (フォント名、フォント サイズ、色など) を表します。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[ChartFont の取得](../api/chartfont_get.md) | [WorkbookChartFont](chartfont.md) |chartFont オブジェクトのプロパティと関係を読み取ります。|
|[更新する](../api/chartfont_update.md) | [WorkbookChartFont](chartfont.md)   |ChartFont オブジェクトを更新します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | タイプ   |説明|
|:---------------|:--------|:----------|
|太字|ブール値|フォントの太字の状態を表します。|
|カラー|文字列|テキストの色の HTML カラー コード表記。たとえば、#FF0000 は赤を表します。|
|イタリック|ブール値|フォントの斜体の状態を表します。|
|名前|文字列|フォント名 (例: "Calibri")|
|サイズ|二重線|フォント サイズ (例: 11)|
|下線|文字列|フォントに適用する下線の種類です。 可能な値は、`None`、`Single` です。|

## <a name="relationships"></a>リレーションシップ
なし


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.workbookChartFont"
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
  "description": "ChartFont resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->