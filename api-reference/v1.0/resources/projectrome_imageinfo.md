# <a name="imageinfo-resource-type"></a>imageInfo リソースの種類

 ** アクティビティ** オブジェクトの [visualInfo](../resources/projectrome_visualinfo.md) の一部の [ 属性](../resources/projectrome_activity.md) のプロパティを表すための複合型です。

## <a name="properties"></a>プロパティ

|名前 | 型 | 説明|
|:----|:-----|:-----------|
|iconUrl | 文字列 | 省略可能です。活動を生成するために使用するアプリケーションを表すアイコンをポイントする URI|
|alternateText | 文字列 | 省略可能です。イメージの alt テキストのアクセス可能なコンテンツ|
|addImageQuery | ブーリアン | 省略可能です。サーバーを指定するためのパラメーターは、パラメーターへの応答に動的にイメージをレンダリングすることです。 例: ハイコントラスト イメージ|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "iconUrl",
    "alternateText",
    "addImageQuery"
  ],
  "@odata.type": "microsoft.graph.imageInfo"
}-->

```json
{
    "@odata.type": "microsoft.graph.imageInfo",
    "iconUrl": "String (URL)",
    "alternateText": "String",
    "addImageQuery": "boolean"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "imageinfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->