# <a name="video-resource-type"></a>ビデオ リソースの種類

**ビデオ** リソースは、ビデオ関連のデータ項目を 1 つの構造にグループ化します。

[**DriveItem**](driveitem.md) に null 以外の**ビデオ** ファセットがある場合は、項目はビデオ ファイルを表します。**ビデオ** リソースのプロパティは、ファイルからメタデータを抽出することにより設定されます。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.video"
}-->

```json
{
  "bitrate": 1024,
  "duration": 1024,
  "height": 1024,
  "width": 1024
}
```

## <a name="properties"></a>プロパティ

| プロパティ | 型  | 説明                               |
|:---------|:------|:------------------------------------------|
| bitrate  | Int32 | 1 秒あたりのビデオのビット レート (ビット単位)。 |
| duration | Int64 | ファイルの継続時間 (ミリ秒単位)。     |
| height   | Int32 | ビデオの高さ (ピクセル単位)。           |
| width    | Int32 | ビデオの幅 (ピクセル単位)。            |

## <a name="remarks"></a>注釈 

DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。





<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "video resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
