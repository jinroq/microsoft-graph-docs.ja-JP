# <a name="rangefill-resource-type"></a><span data-ttu-id="9337f-101">RangeFill リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9337f-101">RangeFill resource type</span></span>

<span data-ttu-id="9337f-102">範囲オブジェクトの背景を表します。</span><span class="sxs-lookup"><span data-stu-id="9337f-102">Represents the background of a range object.</span></span>


## <a name="methods"></a><span data-ttu-id="9337f-103">メソッド</span><span class="sxs-lookup"><span data-stu-id="9337f-103">Methods</span></span>

| <span data-ttu-id="9337f-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="9337f-104">Method</span></span>           | <span data-ttu-id="9337f-105">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="9337f-105">Return Type</span></span>    |<span data-ttu-id="9337f-106">説明</span><span class="sxs-lookup"><span data-stu-id="9337f-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9337f-107">RangeFill を取得する</span><span class="sxs-lookup"><span data-stu-id="9337f-107">Get RangeFill</span></span>](../api/rangefill_get.md) | [<span data-ttu-id="9337f-108">WorkbookRangeFill</span><span class="sxs-lookup"><span data-stu-id="9337f-108">WorkbookRangeFill</span></span>](rangefill.md) |<span data-ttu-id="9337f-109">rangeFill オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="9337f-109">Read properties and relationships of rangeFill object.</span></span>|
|[<span data-ttu-id="9337f-110">更新する</span><span class="sxs-lookup"><span data-stu-id="9337f-110">Update</span></span>](../api/rangefill_update.md) | [<span data-ttu-id="9337f-111">WorkbookRangeFill</span><span class="sxs-lookup"><span data-stu-id="9337f-111">WorkbookRangeFill</span></span>](rangefill.md)   |<span data-ttu-id="9337f-112">RangeFill オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="9337f-112">Update RangeFill object.</span></span> |
|[<span data-ttu-id="9337f-113">クリア</span><span class="sxs-lookup"><span data-stu-id="9337f-113">Clear</span></span>](../api/rangefill_clear.md)|<span data-ttu-id="9337f-114">なし</span><span class="sxs-lookup"><span data-stu-id="9337f-114">None</span></span>|<span data-ttu-id="9337f-115">範囲の背景をリセットします。</span><span class="sxs-lookup"><span data-stu-id="9337f-115">Resets the range background.</span></span>|

## <a name="properties"></a><span data-ttu-id="9337f-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9337f-116">Properties</span></span>
| <span data-ttu-id="9337f-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9337f-117">Property</span></span>     | <span data-ttu-id="9337f-118">タイプ</span><span class="sxs-lookup"><span data-stu-id="9337f-118">Type</span></span>   |<span data-ttu-id="9337f-119">説明</span><span class="sxs-lookup"><span data-stu-id="9337f-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9337f-120">color</span><span class="sxs-lookup"><span data-stu-id="9337f-120">color</span></span>|<span data-ttu-id="9337f-121">文字列</span><span class="sxs-lookup"><span data-stu-id="9337f-121">string</span></span>|<span data-ttu-id="9337f-122">枠線の色を表す HTML カラー コード。形式は #RRGGBB (例: "FFA500")、または名前付きの HTML 色 (例: "オレンジ")</span><span class="sxs-lookup"><span data-stu-id="9337f-122">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange")</span></span>|

## <a name="relationships"></a><span data-ttu-id="9337f-123">関係</span><span class="sxs-lookup"><span data-stu-id="9337f-123">Relationships</span></span>
<span data-ttu-id="9337f-124">なし</span><span class="sxs-lookup"><span data-stu-id="9337f-124">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="9337f-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9337f-125">JSON representation</span></span>

<span data-ttu-id="9337f-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="9337f-126">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookRangeFill"
}-->

```json
{
  "color": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeFill resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->