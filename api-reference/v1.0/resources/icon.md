# <a name="icon-resource-type"></a>アイコン リソースの種類

セルのアイコンを表します。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[アイコンを取得する](../api/icon_get.md) | [アイコン](icon.md) |アイコン オブジェクトのプロパティと関係を読み取ります。|
|[更新する](../api/icon_update.md) | [アイコン](icon.md)  |アイコン オブジェクトを更新します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | タイプ   |説明|
|:---------------|:--------|:----------|
|インデックス|int|指定したセット内のアイコンのインデックスを表します。|
|set|文字列|一部であるアイコンのセットを表します。 可能な値は、 `Invalid`、 `ThreeArrows`、 `ThreeArrowsGray`、 `ThreeFlags`、 `ThreeTrafficLights1`、 `ThreeTrafficLights2`、 `ThreeSigns`、 `ThreeSymbols`、 `ThreeSymbols2`、 `FourArrows`、 `FourArrowsGray`、 `FourRedToBlack`、 `FourRating`、 `FourTrafficLights`、 `FiveArrows`、 `FiveArrowsGray`、 `FiveRating`、 `FiveQuarters`、 `ThreeStars`, `ThreeTriangles`, `FiveBoxes`です。|

## <a name="relationships"></a>リレーションシップ
なし


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookIcon"
}-->

```json
{
  "index": 1024,
  "set": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Icon resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->