# <a name="image-resource-type"></a><span data-ttu-id="d8c95-101">イメージ リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d8c95-101">Image resource type</span></span>

<span data-ttu-id="d8c95-p101">**イメージ** リソースは、イメージ関連のプロパティを 1 つの構造にグループ化します。[**DriveItem**](driveitem.md) に null 以外の**イメージ** ファセットがある場合は、アイテムはビットマップ イメージを表します。</span><span class="sxs-lookup"><span data-stu-id="d8c95-p101">The **Image** resource groups image-related properties into a single structure. If a [**DriveItem**](driveitem.md) has a non-null **image** facet, the item represents a bitmap image.</span></span>

<span data-ttu-id="d8c95-104">**注:**サービスがイメージの幅と高さを決定できない場合は、**イメージ** リソースが空になる可能性があります。</span><span class="sxs-lookup"><span data-stu-id="d8c95-104">**Note:** If the service is unable to determine the width and height of the image, the **Image** resource may be empty.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d8c95-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d8c95-105">JSON representation</span></span>

<span data-ttu-id="d8c95-106">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d8c95-106">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="d8c95-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d8c95-107">Properties</span></span>

| <span data-ttu-id="d8c95-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d8c95-108">Property</span></span>   | <span data-ttu-id="d8c95-109">型</span><span class="sxs-lookup"><span data-stu-id="d8c95-109">Type</span></span>  | <span data-ttu-id="d8c95-110">説明</span><span class="sxs-lookup"><span data-stu-id="d8c95-110">Description</span></span>                                |
|:-----------|:------|:-------------------------------------------|
| <span data-ttu-id="d8c95-111">**height**</span><span class="sxs-lookup"><span data-stu-id="d8c95-111">**height**</span></span> | <span data-ttu-id="d8c95-112">Int32</span><span class="sxs-lookup"><span data-stu-id="d8c95-112">Int32</span></span> | <span data-ttu-id="d8c95-p102">省略可能。イメージの高さ (ピクセル単位)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d8c95-p102">Optional. Height of the image, in pixels. Read-only.</span></span> |
| <span data-ttu-id="d8c95-116">**width**</span><span class="sxs-lookup"><span data-stu-id="d8c95-116">**width**</span></span>  | <span data-ttu-id="d8c95-117">Int32</span><span class="sxs-lookup"><span data-stu-id="d8c95-117">Int32</span></span> | <span data-ttu-id="d8c95-p103">省略可能。イメージの幅 (ピクセル単位)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d8c95-p103">Optional. Width of the image, in pixels. Read-only.</span></span>  |

## <a name="remarks"></a><span data-ttu-id="d8c95-121">注釈</span><span class="sxs-lookup"><span data-stu-id="d8c95-121">Remarks</span></span>

<span data-ttu-id="d8c95-p104">OneDrive for Business では、このリソースは、ファイル拡張子に基づいてイメージであると予期されるアイテム上に返されます。OneDrive for Business では、このリソースはいずれのプロパティも返しません。</span><span class="sxs-lookup"><span data-stu-id="d8c95-p104">In OneDrive for Business, this resource is returned on items that are expected to be images based on file extension. This resource returns no properties in OneDrive for Business.</span></span>

<span data-ttu-id="d8c95-124">DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d8c95-124">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "image resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
