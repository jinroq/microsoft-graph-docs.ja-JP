# <a name="photo-resource-type"></a><span data-ttu-id="ac561-101">写真リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ac561-101">Photo resource type</span></span>

<span data-ttu-id="ac561-102">**写真**リソースは、EXIF メタデータなどの写真とカメラのプロパティを [driveItem](driveitem.md) で提供します。</span><span class="sxs-lookup"><span data-stu-id="ac561-102">The **photo** resource provides photo and camera properties, for example, EXIF metadata, on a [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="ac561-103">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ac561-103">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="ac561-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ac561-104">Properties</span></span>
| <span data-ttu-id="ac561-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ac561-105">Property</span></span>                | <span data-ttu-id="ac561-106">型</span><span class="sxs-lookup"><span data-stu-id="ac561-106">Type</span></span>                      | <span data-ttu-id="ac561-107">説明</span><span class="sxs-lookup"><span data-stu-id="ac561-107">Description</span></span>                                                     |
|:------------------------|:--------------------------|:----------------------------------------------------------------|
| <span data-ttu-id="ac561-108">**takenDateTime**</span><span class="sxs-lookup"><span data-stu-id="ac561-108">**takenDateTime**</span></span>       | <span data-ttu-id="ac561-109">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ac561-109">DateTimeOffset</span></span>            | <span data-ttu-id="ac561-p101">写真の撮影日時を表します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ac561-p101">Represents the date and time the photo was taken. Read-only.</span></span>               |
| <span data-ttu-id="ac561-112">**cameraMake**</span><span class="sxs-lookup"><span data-stu-id="ac561-112">**cameraMake**</span></span>          | <span data-ttu-id="ac561-113">String</span><span class="sxs-lookup"><span data-stu-id="ac561-113">String</span></span>                    | <span data-ttu-id="ac561-p102">カメラの製造元。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ac561-p102">Camera manufacturer. Read-only.</span></span>                                            |
| <span data-ttu-id="ac561-116">**cameraModel**</span><span class="sxs-lookup"><span data-stu-id="ac561-116">**cameraModel**</span></span>         | <span data-ttu-id="ac561-117">String</span><span class="sxs-lookup"><span data-stu-id="ac561-117">String</span></span>                    | <span data-ttu-id="ac561-p103">カメラのモデル。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ac561-p103">Camera model. Read-only.</span></span>                                                   |
| <span data-ttu-id="ac561-120">**fNumber**</span><span class="sxs-lookup"><span data-stu-id="ac561-120">**fNumber**</span></span>             | <span data-ttu-id="ac561-121">Double</span><span class="sxs-lookup"><span data-stu-id="ac561-121">Double</span></span>                    | <span data-ttu-id="ac561-p104">カメラの絞り値。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ac561-p104">The F-stop value from the camera. Read-only.</span></span>                               |
| <span data-ttu-id="ac561-124">**exposureDenominator**</span><span class="sxs-lookup"><span data-stu-id="ac561-124">**exposureDenominator**</span></span> | <span data-ttu-id="ac561-125">Int32</span><span class="sxs-lookup"><span data-stu-id="ac561-125">Int32</span></span>                     | <span data-ttu-id="ac561-p105">カメラの露出時間の分数の分母。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ac561-p105">The denominator for the exposure time fraction from the camera. Read-only.</span></span> |
| <span data-ttu-id="ac561-128">**exposureNumerator**</span><span class="sxs-lookup"><span data-stu-id="ac561-128">**exposureNumerator**</span></span>   | <span data-ttu-id="ac561-129">Int32</span><span class="sxs-lookup"><span data-stu-id="ac561-129">Int32</span></span>                     | <span data-ttu-id="ac561-p106">カメラの露出時間の分数の分子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ac561-p106">The numerator for the exposure time fraction from the camera. Read-only.</span></span>   |
| <span data-ttu-id="ac561-132">**focalLength**</span><span class="sxs-lookup"><span data-stu-id="ac561-132">**focalLength**</span></span>         | <span data-ttu-id="ac561-133">Double</span><span class="sxs-lookup"><span data-stu-id="ac561-133">Double</span></span>                    | <span data-ttu-id="ac561-p107">カメラの焦点距離。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ac561-p107">The focal length from the camera. Read-only.</span></span>                               |
| <span data-ttu-id="ac561-136">**iso**</span><span class="sxs-lookup"><span data-stu-id="ac561-136">**iso**</span></span>                 | <span data-ttu-id="ac561-137">Int32</span><span class="sxs-lookup"><span data-stu-id="ac561-137">Int32</span></span>                     | <span data-ttu-id="ac561-p108">カメラの ISO 値。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ac561-p108">The ISO value from the camera. Read-only.</span></span>                                  |

## <a name="remarks"></a><span data-ttu-id="ac561-140">注釈</span><span class="sxs-lookup"><span data-stu-id="ac561-140">Remarks</span></span>
<span data-ttu-id="ac561-141">OneDrive for Business と SharePoint は、**takenDateTime** プロパティのみを返します。</span><span class="sxs-lookup"><span data-stu-id="ac561-141">OneDrive for Business and SharePoint only return the **takenDateTime** property.</span></span>

<span data-ttu-id="ac561-142">DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ac561-142">For more information about the facets on a [driveItem](driveitem.md), see driveItem.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "photo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
