# <a name="rangeborder-resource-type"></a><span data-ttu-id="a561c-101">RangeBorder リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a561c-101">RangeBorder resource type</span></span>

<span data-ttu-id="a561c-102">オブジェクトの輪郭を表します。</span><span class="sxs-lookup"><span data-stu-id="a561c-102">Represents the border of an object.</span></span>


## <a name="methods"></a><span data-ttu-id="a561c-103">メソッド</span><span class="sxs-lookup"><span data-stu-id="a561c-103">Methods</span></span>

| <span data-ttu-id="a561c-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="a561c-104">Method</span></span>           | <span data-ttu-id="a561c-105">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="a561c-105">Return Type</span></span>    |<span data-ttu-id="a561c-106">説明</span><span class="sxs-lookup"><span data-stu-id="a561c-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a561c-107">Get RangeBorder</span><span class="sxs-lookup"><span data-stu-id="a561c-107">Get RangeBorder</span></span>](../api/rangeborder_get.md) | [<span data-ttu-id="a561c-108">WorkbookRangeBorder</span><span class="sxs-lookup"><span data-stu-id="a561c-108">WorkbookRangeBorder</span></span>](rangeborder.md) |<span data-ttu-id="a561c-109">rangeBorder オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="a561c-109">Read properties and relationships of rangeBorder object.</span></span>|
|[<span data-ttu-id="a561c-110">Update</span><span class="sxs-lookup"><span data-stu-id="a561c-110">Update</span></span>](../api/rangeborder_update.md) | [<span data-ttu-id="a561c-111">WorkbookRangeBorder</span><span class="sxs-lookup"><span data-stu-id="a561c-111">WorkbookRangeBorder</span></span>](rangeborder.md) |<span data-ttu-id="a561c-112">RangeBorder オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="a561c-112">Update RangeBorder object.</span></span> |
|[<span data-ttu-id="a561c-113">List</span><span class="sxs-lookup"><span data-stu-id="a561c-113">List</span></span>](../api/rangeborder_list.md) | <span data-ttu-id="a561c-114">[WorkbookRangeBorder](rangeborder.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a561c-114">[WorkbookRangeBorder](rangeborder.md) collection</span></span> |<span data-ttu-id="a561c-115">rangeBorder オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="a561c-115">Get rangeBorder object collection.</span></span> |
|[<span data-ttu-id="a561c-116">Itemat</span><span class="sxs-lookup"><span data-stu-id="a561c-116">Itemat</span></span>](../api/rangebordercollection_itemat.md)|[<span data-ttu-id="a561c-117">WorkbookRangeBorder</span><span class="sxs-lookup"><span data-stu-id="a561c-117">WorkbookRangeBorder</span></span>](rangeborder.md)|<span data-ttu-id="a561c-118">オブジェクトのインデックスを使用して、罫線オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="a561c-118">Gets a border object using its index</span></span>|

## <a name="properties"></a><span data-ttu-id="a561c-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a561c-119">Properties</span></span>
| <span data-ttu-id="a561c-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a561c-120">Property</span></span>     | <span data-ttu-id="a561c-121">タイプ</span><span class="sxs-lookup"><span data-stu-id="a561c-121">Type</span></span>   |<span data-ttu-id="a561c-122">説明</span><span class="sxs-lookup"><span data-stu-id="a561c-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a561c-123">color</span><span class="sxs-lookup"><span data-stu-id="a561c-123">color</span></span>|<span data-ttu-id="a561c-124">文字列</span><span class="sxs-lookup"><span data-stu-id="a561c-124">string</span></span>|<span data-ttu-id="a561c-125">枠線の色を表す HTML カラー コード。形式は #RRGGBB (例: "FFA500")、または名前付きの HTML 色 (例: "オレンジ") です。</span><span class="sxs-lookup"><span data-stu-id="a561c-125">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange").</span></span>|
|<span data-ttu-id="a561c-126">id</span><span class="sxs-lookup"><span data-stu-id="a561c-126">id</span></span>|<span data-ttu-id="a561c-127">string</span><span class="sxs-lookup"><span data-stu-id="a561c-127">string</span></span>|<span data-ttu-id="a561c-128">罫線の識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="a561c-128">Represents border identifier. Possible values are: , , , , , , , . Read-only.</span></span> <span data-ttu-id="a561c-129">指定できる値は、`EdgeTop`、`EdgeBottom`、`EdgeLeft`、`EdgeRight`、`InsideVertical`、`InsideHorizontal`、`DiagonalDown`、`DiagonalUp` です。</span><span class="sxs-lookup"><span data-stu-id="a561c-129">The possible values are `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`, , , , or .</span></span> <span data-ttu-id="a561c-130">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="a561c-130">Read-only.</span></span>|
|<span data-ttu-id="a561c-131">sideIndex</span><span class="sxs-lookup"><span data-stu-id="a561c-131">sideIndex</span></span>|<span data-ttu-id="a561c-132">string</span><span class="sxs-lookup"><span data-stu-id="a561c-132">string</span></span>|<span data-ttu-id="a561c-133">罫線の特定の側面を示す定数値です。</span><span class="sxs-lookup"><span data-stu-id="a561c-133">Constant value that indicates the specific side of the border. Possible values are: , , , , , , , . Read-only.</span></span> <span data-ttu-id="a561c-134">指定できる値は、`EdgeTop`、`EdgeBottom`、`EdgeLeft`、`EdgeRight`、`InsideVertical`、`InsideHorizontal`、`DiagonalDown`、`DiagonalUp` です。</span><span class="sxs-lookup"><span data-stu-id="a561c-134">The possible values are `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`, , , , or .</span></span> <span data-ttu-id="a561c-135">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="a561c-135">Read-only.</span></span>|
|<span data-ttu-id="a561c-136">style</span><span class="sxs-lookup"><span data-stu-id="a561c-136">style</span></span>|<span data-ttu-id="a561c-137">string</span><span class="sxs-lookup"><span data-stu-id="a561c-137">string</span></span>|<span data-ttu-id="a561c-138">罫線の線スタイルを指定する、線スタイルの定数の 1 つです。</span><span class="sxs-lookup"><span data-stu-id="a561c-138">One of the constants of line style specifying the line style for the border. Possible values are: , , , , , , , .</span></span> <span data-ttu-id="a561c-139">指定できる値は、`None`、`Continuous`、`Dash`、`DashDot`、`DashDotDot`、`Dot`、`Double`、`SlantDashDot` です。</span><span class="sxs-lookup"><span data-stu-id="a561c-139">The possible values are `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`, , , , or .</span></span>|
|<span data-ttu-id="a561c-140">weight</span><span class="sxs-lookup"><span data-stu-id="a561c-140">weight</span></span>|<span data-ttu-id="a561c-141">string</span><span class="sxs-lookup"><span data-stu-id="a561c-141">string</span></span>|<span data-ttu-id="a561c-142">範囲周辺の罫線の太さを指定します。</span><span class="sxs-lookup"><span data-stu-id="a561c-142">Specifies the weight of the border around a range.</span></span> <span data-ttu-id="a561c-143">指定できる値は、  `Hairline`、  `Thin`、  `Medium`、  `Thick` です。</span><span class="sxs-lookup"><span data-stu-id="a561c-143">The possible values are `Hairline`, `Thin`, `Medium`, `Thick`, , , , , , , , or .</span></span>|

## <a name="relationships"></a><span data-ttu-id="a561c-144">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a561c-144">Relationships</span></span>
<span data-ttu-id="a561c-145">なし</span><span class="sxs-lookup"><span data-stu-id="a561c-145">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="a561c-146">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a561c-146">JSON representation</span></span>

<span data-ttu-id="a561c-147">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a561c-147">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookRangeBorder"
}-->

```json
{
  "color": "string",
  "id": "string",
  "sideIndex": "string",
  "style": "string",
  "weight": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeBorder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->