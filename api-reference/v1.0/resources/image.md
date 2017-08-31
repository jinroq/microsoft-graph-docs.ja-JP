# <a name="image-resource-type"></a>イメージ リソースの種類

**イメージ** リソースは、イメージ関連のプロパティを 1 つの構造にグループ化します。[**DriveItem**](driveitem.md) に null 以外の**イメージ** ファセットがある場合は、アイテムはビットマップ イメージを表します。

**注:**サービスがイメージの幅と高さを決定できない場合は、**イメージ** リソースが空になる可能性があります。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@odata.type": "microsoft.graph.image"
}-->

```json
{
  "height": 1024,
  "width": 1024
}
```

## <a name="properties"></a>プロパティ

| プロパティ   | 型  | 説明                                |
|:-----------|:------|:-------------------------------------------|
| **height** | Int32 | 省略可能。イメージの高さ (ピクセル単位)。読み取り専用です。 |
| **width**  | Int32 | 省略可能。イメージの幅 (ピクセル単位)。読み取り専用です。  |

## <a name="remarks"></a>注釈

OneDrive for Business では、このリソースは、ファイル拡張子に基づいてイメージであると予期されるアイテム上に返されます。OneDrive for Business では、このリソースはいずれのプロパティも返しません。

DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "image resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
