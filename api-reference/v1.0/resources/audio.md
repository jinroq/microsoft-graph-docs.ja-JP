# <a name="audio-resource-type"></a>オーディオ リソース型

**オーティオ** リソースは、アイテムのオーディオ関連のプロパティを単一の構造にグループ化します。

[**DriveItem**](driveitem.md) に null 以外の**オーディオ** ファセットがある場合、そのアイテムはオーディオ ファイルを表します。**オーディオ** リソースのプロパティは、ファイルからメタデータを抽出することで設定されます。 

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@odata.type": "microsoft.graph.audio"
}-->
```json
{
  "album": "string",
  "albumArtist": "string",
  "artist": "string",
  "bitrate": 1024,
  "composers": "string",
  "copyright": "string",
  "disc": 1024,
  "discCount": 1024,
  "duration": 1024,
  "genre": "string",
  "hasDrm": true,
  "isVariableBitrate": true,
  "title": "string",
  "track": 1024,
  "trackCount": 1024,
  "year": 1024
}
```

## <a name="properties"></a>プロパティ

| プロパティ          | 型    | 説明                                                          |
|:------------------|:--------|:---------------------------------------------------------------------|
| album             | string  | オーディオ ファイルのアルバムのタイトル。                          |
| albumArtist       | string  | オーディオ ファイルのアルバムに付けられたアーチスト名。                    |
| artist            | string  | オーディオ ファイルの歌手や奏者。                            |
| bitrate           | string  | kbps 単位で表されるビットレート。                                           |
| composers         | string  | オーディオ ファイルの作曲者の名前。                          |
| copyright         | string  | オーディオ ファイルの著作権情報。                            |
| disc              | number  | このオーディオ ファイルの元のディスクの番号。                    |
| discCount         | number  | このアルバムの合計ディスク数。                             |
| duration          | number  | オーディオ ファイルの継続時間。ミリ秒単位で表されます。                |
| genre             | string  | このオーディオ ファイルのジャンル。                                        |
| hasDrm            | boolean | ファイルがデジタル著作権管理で保護されているかどうかを示します。   |
| isVariableBitrate | boolean | ファイルが可変ビットレートでエンコードされているかどうかを示します。            |
| title             | string  | オーディオ ファイルのタイトル。                                         |
| track             | number  | このオーディオ ファイルの元のディスクでのトラック番号。    |
| trackCount        | number  | このオーディオ ファイルの元のディスクの合計トラック数。 |
| year              | number  | オーディオ ファイルが録音された年。                                |

## <a name="remarks"></a>備考 

DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "audio resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->