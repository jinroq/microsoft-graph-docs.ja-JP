# <a name="geocoordinates-resource-type"></a><span data-ttu-id="3be59-101">GeoCoordinates リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3be59-101">GeoCoordinates resource type</span></span>

<span data-ttu-id="3be59-p101">**GeoCoordinates** リソースは、ファイル内に含まれるメタデータに基づいて場所の地理座標系と高度を提供します。[**DriveItem**](driveitem.md) に null でない**場所**のファセットがある場合は、アイテムは、それに関連付けられている既知の場所を含むファイルを表します。</span><span class="sxs-lookup"><span data-stu-id="3be59-p101">The **GeoCoordinates** resource provides geographic coordinates and elevation of a location based on metadata contained within the file. If a [**DriveItem**](driveitem.md) has a non-null **location** facet, the item represents a file with a known location assocaited with it.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3be59-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3be59-104">JSON representation</span></span>

<span data-ttu-id="3be59-105">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="3be59-105">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="3be59-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3be59-106">Properties</span></span>

| <span data-ttu-id="3be59-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3be59-107">Property</span></span>  | <span data-ttu-id="3be59-108">型</span><span class="sxs-lookup"><span data-stu-id="3be59-108">Type</span></span>   | <span data-ttu-id="3be59-109">説明</span><span class="sxs-lookup"><span data-stu-id="3be59-109">Description</span></span>                                                    |
|:----------|:-------|:---------------------------------------------------------------|
| <span data-ttu-id="3be59-110">altitude</span><span class="sxs-lookup"><span data-stu-id="3be59-110">altitude</span></span>  | <span data-ttu-id="3be59-111">Double</span><span class="sxs-lookup"><span data-stu-id="3be59-111">Double</span></span> | <span data-ttu-id="3be59-p102">省略可能。アイテムの海抜をフィート単位で表した高度 (高さ)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="3be59-p102">Optional. The altitude (height), in feet,  above sea level for the item. Read-only.</span></span> |
| <span data-ttu-id="3be59-115">latitude</span><span class="sxs-lookup"><span data-stu-id="3be59-115">latitude</span></span>  | <span data-ttu-id="3be59-116">Double</span><span class="sxs-lookup"><span data-stu-id="3be59-116">Double</span></span> | <span data-ttu-id="3be59-p103">省略可能。アイテムの緯度 (10 進数)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="3be59-p103">Optional. The latitude, in decimal, for the item. Read-only.</span></span>   |
| <span data-ttu-id="3be59-120">longitude</span><span class="sxs-lookup"><span data-stu-id="3be59-120">longitude</span></span> | <span data-ttu-id="3be59-121">Double</span><span class="sxs-lookup"><span data-stu-id="3be59-121">Double</span></span> | <span data-ttu-id="3be59-p104">省略可能。アイテムの経度 (10 進数)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="3be59-p104">Optional. The longitude, in decimal, for the item. Read-only.</span></span>  |

## <a name="remarks"></a><span data-ttu-id="3be59-125">注釈</span><span class="sxs-lookup"><span data-stu-id="3be59-125">Remarks</span></span>

<span data-ttu-id="3be59-126">DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3be59-126">For more information about the facets on a [driveItem](driveitem.md), see driveItem.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "geoCoordinates resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
