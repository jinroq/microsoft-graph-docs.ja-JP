# <a name="thumbnail-resource-type"></a>サムネイル リソースの種類

**サムネイル** リソースの種類は、グラフィック表示を含む OneDrive 上にあるイメージ、ビデオ、ドキュメント、任意のファイルまたはフォルダーのサムネイルを表します。

## <a name="properties"></a>プロパティ

| プロパティ | 型   | 説明                                  |
|:---------|:-------|:---------------------------------------------|
| height   | Int32  | サムネイルの高さ (ピクセル単位)。      |
| url      | String | サムネイルのコンテンツをフェッチするために使用する URL。 |
| width    | Int32  | サムネイルの幅 (ピクセル単位)。       |


## <a name="relationships"></a>関係

| 名前    | 型   | 説明         |
|:--------|:-------|:--------------------|
| content | Stream | コンテンツ ストリーム。 |


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": ["content", "height", "width"],
  "@odata.type": "microsoft.graph.thumbnail"
}-->

```json
{
  "url": "string",
  "height": 1024,
  "width": 1024,
  "content": "stream"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "thumbnail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
