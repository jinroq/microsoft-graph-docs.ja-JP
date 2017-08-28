# <a name="thumbnailset-resource-type"></a><span data-ttu-id="c2ab1-101">ThumbnailSet リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c2ab1-101">ThumbnailSet resource type</span></span>

<span data-ttu-id="c2ab1-p101">**ThumbnailSet** リソースは、[サムネイル](thumbnail.md) リソースのキー付きコレクションです。DriveItem に関連付けられているサムネイルのセットを表すために使用されます。</span><span class="sxs-lookup"><span data-stu-id="c2ab1-p101">The **ThumbnailSet** resource is a keyed collection of [thumbnail](thumbnail.md) resources. It is used to represent a set of thumbnails associated with a DriveItem.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c2ab1-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c2ab1-104">JSON representation</span></span>

<span data-ttu-id="c2ab1-105">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c2ab1-105">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="c2ab1-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c2ab1-106">Properties</span></span>

| <span data-ttu-id="c2ab1-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c2ab1-107">Property</span></span> | <span data-ttu-id="c2ab1-108">型</span><span class="sxs-lookup"><span data-stu-id="c2ab1-108">Type</span></span>                      | <span data-ttu-id="c2ab1-109">説明</span><span class="sxs-lookup"><span data-stu-id="c2ab1-109">Description</span></span>                                                                       |
|:---------|:--------------------------|:----------------------------------------------------------------------------------|
| <span data-ttu-id="c2ab1-110">id</span><span class="sxs-lookup"><span data-stu-id="c2ab1-110">id</span></span>       | <span data-ttu-id="c2ab1-111">String</span><span class="sxs-lookup"><span data-stu-id="c2ab1-111">String</span></span>                    | <span data-ttu-id="c2ab1-p102">アイテム内の ID。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="c2ab1-p102">The id within the item. Read-only.</span></span>                                                |
| <span data-ttu-id="c2ab1-114">large</span><span class="sxs-lookup"><span data-stu-id="c2ab1-114">large</span></span>    | [<span data-ttu-id="c2ab1-115">Thumbnail</span><span class="sxs-lookup"><span data-stu-id="c2ab1-115">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="c2ab1-116">1920 x 1920 にスケーリングされたサムネイル。</span><span class="sxs-lookup"><span data-stu-id="c2ab1-116">A 1920x1920 scaled thumbnail.</span></span>                                                     |
| <span data-ttu-id="c2ab1-117">medium</span><span class="sxs-lookup"><span data-stu-id="c2ab1-117">medium</span></span>   | [<span data-ttu-id="c2ab1-118">Thumbnail</span><span class="sxs-lookup"><span data-stu-id="c2ab1-118">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="c2ab1-119">176x176 にスケーリングされたサムネイル。</span><span class="sxs-lookup"><span data-stu-id="c2ab1-119">A 176x176 scaled thumbnail.</span></span>                                                       |
| <span data-ttu-id="c2ab1-120">small</span><span class="sxs-lookup"><span data-stu-id="c2ab1-120">small</span></span>    | [<span data-ttu-id="c2ab1-121">Thumbnail</span><span class="sxs-lookup"><span data-stu-id="c2ab1-121">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="c2ab1-122">48 x 48 にトリミングされたサムネイル。</span><span class="sxs-lookup"><span data-stu-id="c2ab1-122">A 48x48 cropped thumbnail.</span></span>                                                        |
| <span data-ttu-id="c2ab1-123">source</span><span class="sxs-lookup"><span data-stu-id="c2ab1-123">source</span></span>   | [<span data-ttu-id="c2ab1-124">Thumbnail</span><span class="sxs-lookup"><span data-stu-id="c2ab1-124">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="c2ab1-125">カスタムのサムネイル イメージ、または他のサムネイルを生成するために使用する元のイメージ。</span><span class="sxs-lookup"><span data-stu-id="c2ab1-125">A custom thumbnail image or the original image used to generate other thumbnails.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "thumbnailSet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
