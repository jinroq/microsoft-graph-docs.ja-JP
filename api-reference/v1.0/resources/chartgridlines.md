# <a name="chartgridlines-resource-type"></a><span data-ttu-id="fdbd9-101">ChartGridlines リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fdbd9-101">ChartGridlines resource type</span></span>

<span data-ttu-id="fdbd9-102">グラフの軸の目盛線または補助目盛線を表します。</span><span class="sxs-lookup"><span data-stu-id="fdbd9-102">Represents major or minor gridlines on a chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="fdbd9-103">メソッド</span><span class="sxs-lookup"><span data-stu-id="fdbd9-103">Methods</span></span>

| <span data-ttu-id="fdbd9-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="fdbd9-104">Method</span></span>           | <span data-ttu-id="fdbd9-105">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="fdbd9-105">Return Type</span></span>    |<span data-ttu-id="fdbd9-106">説明</span><span class="sxs-lookup"><span data-stu-id="fdbd9-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fdbd9-107">Get ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="fdbd9-107">Get ChartGridlines</span></span>](../api/chartgridlines_get.md) | [<span data-ttu-id="fdbd9-108">WorkbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="fdbd9-108">WorkbookChartGridlines</span></span>](chartgridlines.md) |<span data-ttu-id="fdbd9-109">chartGridlines オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="fdbd9-109">Read properties and relationships of chartGridlines object.</span></span>|
|[<span data-ttu-id="fdbd9-110">Update</span><span class="sxs-lookup"><span data-stu-id="fdbd9-110">Update</span></span>](../api/chartgridlines_update.md) | [<span data-ttu-id="fdbd9-111">WorkbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="fdbd9-111">WorkbookChartGridlines</span></span>](chartgridlines.md)    |<span data-ttu-id="fdbd9-112">ChartGridlines オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="fdbd9-112">Update ChartGridlines object.</span></span> |

## <a name="properties"></a><span data-ttu-id="fdbd9-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fdbd9-113">Properties</span></span>
| <span data-ttu-id="fdbd9-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fdbd9-114">Property</span></span>     | <span data-ttu-id="fdbd9-115">タイプ</span><span class="sxs-lookup"><span data-stu-id="fdbd9-115">Type</span></span>   |<span data-ttu-id="fdbd9-116">説明</span><span class="sxs-lookup"><span data-stu-id="fdbd9-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fdbd9-117">visible</span><span class="sxs-lookup"><span data-stu-id="fdbd9-117">visible</span></span>|<span data-ttu-id="fdbd9-118">boolean</span><span class="sxs-lookup"><span data-stu-id="fdbd9-118">boolean</span></span>|<span data-ttu-id="fdbd9-119">軸の目盛線を表示するか非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="fdbd9-119">Boolean value representing if the axis gridlines are visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fdbd9-120">関係</span><span class="sxs-lookup"><span data-stu-id="fdbd9-120">Relationships</span></span>
| <span data-ttu-id="fdbd9-121">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="fdbd9-121">Relationship</span></span> | <span data-ttu-id="fdbd9-122">型</span><span class="sxs-lookup"><span data-stu-id="fdbd9-122">Type</span></span>   |<span data-ttu-id="fdbd9-123">説明</span><span class="sxs-lookup"><span data-stu-id="fdbd9-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fdbd9-124">format</span><span class="sxs-lookup"><span data-stu-id="fdbd9-124">format</span></span>|[<span data-ttu-id="fdbd9-125">WorkbookChartGridlinesFormat</span><span class="sxs-lookup"><span data-stu-id="fdbd9-125">WorkbookChartGridlinesFormat</span></span>](chartgridlinesformat.md)|<span data-ttu-id="fdbd9-p101">グラフの目盛線の書式設定を表します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="fdbd9-p101">Represents the formatting of chart gridlines. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fdbd9-128">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fdbd9-128">JSON representation</span></span>

<span data-ttu-id="fdbd9-129">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="fdbd9-129">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookChartGridlines"
}-->

```json
{
  "visible": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartGridlines resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->