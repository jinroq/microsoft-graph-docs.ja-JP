# <a name="folder-resource-type"></a>フォルダー リソースの種類

**フォルダー**リソースは、アイテム上のフォルダー関連のデータを 1 つの構造にグループ化します。**フォルダー**ファセットが null 以外の [**DriveItems**](driveitem.md) は、他の DriveItems のコンテナーです。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.folder"
}-->

```json
{
  "childCount": 1024
}
```

## <a name="properties"></a>プロパティ

| プロパティ       | 型  | 説明                                                     |
|:---------------|:------|:----------------------------------------------------------------|
| **childCount** | Int64 | このコンテナーの中に含まれる子の数。 |

## <a name="remarks"></a>注釈 

DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "folder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
