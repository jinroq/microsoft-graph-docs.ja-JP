# <a name="thumbnailset-resource-type"></a>ThumbnailSet リソースの種類

**ThumbnailSet** リソースは、[サムネイル](thumbnail.md) リソースのキー付きコレクションです。DriveItem に関連付けられているサムネイルのセットを表すために使用されます。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": ["source", "small", "medium", "large"],
  "openType": true,
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.thumbnailSet"
} -->

```json
{
  "id": "string (identifier)",
  "large": {"@odata.type": "microsoft.graph.thumbnail"},
  "medium": {"@odata.type": "microsoft.graph.thumbnail"},
  "small": {"@odata.type": "microsoft.graph.thumbnail"},
  "source": {"@odata.type": "microsoft.graph.thumbnail"}
}
```

## <a name="properties"></a>プロパティ

| プロパティ | 型                      | 説明                                                                       |
|:---------|:--------------------------|:----------------------------------------------------------------------------------|
| id       | String                    | アイテム内の ID。読み取り専用です。                                                |
| large    | [Thumbnail](thumbnail.md) | 1920 x 1920 にスケーリングされたサムネイル。                                                     |
| medium   | [Thumbnail](thumbnail.md) | 176x176 にスケーリングされたサムネイル。                                                       |
| small    | [Thumbnail](thumbnail.md) | 48 x 48 にトリミングされたサムネイル。                                                        |
| source   | [Thumbnail](thumbnail.md) | カスタムのサムネイル イメージ、または他のサムネイルを生成するために使用する元のイメージ。 |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "thumbnailSet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
