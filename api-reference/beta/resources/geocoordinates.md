# <a name="geocoordinates-resource-type"></a>GeoCoordinates リソースの種類

**GeoCoordinates** リソースは、ファイル内に含まれるメタデータに基づいて場所の地理座標系と高度を提供します。[**DriveItem**](driveitem.md) に null でない**場所**のファセットがある場合は、アイテムは、それに関連付けられている既知の場所を含むファイルを表します。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.geoCoordinates"
}-->

```json
{
  "altitude": 1024.13,
  "latitude": 26.13246,
  "longitude": 24.34616
}
```

## <a name="properties"></a>プロパティ

| プロパティ  | 型   | 説明                                                    |
|:----------|:-------|:---------------------------------------------------------------|
| altitude  | Double | 省略可能。アイテムの海抜をフィート単位で表した高度 (高さ)。読み取り専用です。 |
| latitude  | Double | 省略可能。アイテムの緯度 (10 進数)。読み取り専用です。   |
| longitude | Double | 省略可能。アイテムの経度 (10 進数)。読み取り専用です。  |


## <a name="remarks"></a>注釈

DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "geoCoordinates resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
