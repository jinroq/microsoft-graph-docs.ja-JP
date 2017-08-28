# <a name="photo-resource-type"></a>写真リソースの種類

**写真**リソースは、EXIF メタデータなどの写真とカメラのプロパティを [driveItem](driveitem.md) で提供します。

## <a name="json-representation"></a>JSON 表記

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.photo"
}-->
```json
{
  "cameraMake": "string",
  "cameraModel": "string",
  "exposureDenominator": 1024,
  "exposureNumerator": 1024,
  "fNumber": 1024,
  "focalLength": 1024,
  "iso": 1024,
  "takenDateTime": "String (timestamp)"
}
```

## <a name="properties"></a>プロパティ
| プロパティ                | 型                      | 説明                                                     |
|:------------------------|:--------------------------|:----------------------------------------------------------------|
| **takenDateTime**       | DateTimeOffset            | 写真の撮影日時を表します。読み取り専用です。               |
| **cameraMake**          | String                    | カメラの製造元。読み取り専用です。                                            |
| **cameraModel**         | String                    | カメラのモデル。読み取り専用です。                                                   |
| **fNumber**             | Double                    | カメラの絞り値。読み取り専用です。                               |
| **exposureDenominator** | Int32                     | カメラの露出時間の分数の分母。読み取り専用です。 |
| **exposureNumerator**   | Int32                     | カメラの露出時間の分数の分子。読み取り専用です。   |
| **focalLength**         | Double                    | カメラの焦点距離。読み取り専用です。                               |
| **iso**                 | Int32                     | カメラの ISO 値。読み取り専用です。                                  |

## <a name="remarks"></a>注釈
OneDrive for Business と SharePoint は、**takenDateTime** プロパティのみを返します。

DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "photo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
