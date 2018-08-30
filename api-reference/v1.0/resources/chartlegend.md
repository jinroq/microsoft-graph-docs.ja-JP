# <a name="chartlegend-resource-type"></a><span data-ttu-id="a8134-101">ChartLegend リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a8134-101">ChartLegend resource type</span></span>

<span data-ttu-id="a8134-102">グラフに凡例を表します。</span><span class="sxs-lookup"><span data-stu-id="a8134-102">Represents the legend in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="a8134-103">メソッド</span><span class="sxs-lookup"><span data-stu-id="a8134-103">Methods</span></span>

| <span data-ttu-id="a8134-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="a8134-104">Method</span></span>           | <span data-ttu-id="a8134-105">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="a8134-105">Return Type</span></span>    |<span data-ttu-id="a8134-106">説明</span><span class="sxs-lookup"><span data-stu-id="a8134-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a8134-107">Get ChartLegend</span><span class="sxs-lookup"><span data-stu-id="a8134-107">Get ChartLegend</span></span>](../api/chartlegend_get.md) | [<span data-ttu-id="a8134-108">WorkbookChartLegend</span><span class="sxs-lookup"><span data-stu-id="a8134-108">WorkbookChartLegend</span></span>](chartlegend.md) |<span data-ttu-id="a8134-109">chartLegend オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="a8134-109">Read properties and relationships of chartLegend object.</span></span>|
|[<span data-ttu-id="a8134-110">Update</span><span class="sxs-lookup"><span data-stu-id="a8134-110">Update</span></span>](../api/chartlegend_update.md) | [<span data-ttu-id="a8134-111">WorkbookChartLegend</span><span class="sxs-lookup"><span data-stu-id="a8134-111">WorkbookChartLegend</span></span>](chartlegend.md) |<span data-ttu-id="a8134-112">ChartLegend オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="a8134-112">Update ChartLegend object.</span></span> |

## <a name="properties"></a><span data-ttu-id="a8134-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a8134-113">Properties</span></span>
| <span data-ttu-id="a8134-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a8134-114">Property</span></span>     | <span data-ttu-id="a8134-115">タイプ</span><span class="sxs-lookup"><span data-stu-id="a8134-115">Type</span></span>   |<span data-ttu-id="a8134-116">説明</span><span class="sxs-lookup"><span data-stu-id="a8134-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a8134-117">overlay</span><span class="sxs-lookup"><span data-stu-id="a8134-117">overlay</span></span>|<span data-ttu-id="a8134-118">boolean</span><span class="sxs-lookup"><span data-stu-id="a8134-118">boolean</span></span>|<span data-ttu-id="a8134-119">グラフの凡例をグラフの本体に重ねるかどうかを指定するブール型の値です。</span><span class="sxs-lookup"><span data-stu-id="a8134-119">Boolean value for whether the chart legend should overlap with the main body of the chart.</span></span>|
|<span data-ttu-id="a8134-120">position</span><span class="sxs-lookup"><span data-stu-id="a8134-120">position</span></span>|<span data-ttu-id="a8134-121">string</span><span class="sxs-lookup"><span data-stu-id="a8134-121">string</span></span>|<span data-ttu-id="a8134-122">グラフの凡例の位置を表します。</span><span class="sxs-lookup"><span data-stu-id="a8134-122">Represents the position of the legend on the chart. Possible values are: , , , , , .</span></span> <span data-ttu-id="a8134-123">可能な値は、`Top`、`Bottom`、`Left`、`Right`、`Corner`、`Custom` です。</span><span class="sxs-lookup"><span data-stu-id="a8134-123">The possible values are `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`, , , , , , or .</span></span>|
|<span data-ttu-id="a8134-124">visible</span><span class="sxs-lookup"><span data-stu-id="a8134-124">visible</span></span>|<span data-ttu-id="a8134-125">boolean</span><span class="sxs-lookup"><span data-stu-id="a8134-125">boolean</span></span>|<span data-ttu-id="a8134-126">ChartLegend オブジェクトを表示または非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="a8134-126">A boolean value the represents the visibility of a ChartLegend object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a8134-127">関係</span><span class="sxs-lookup"><span data-stu-id="a8134-127">Relationships</span></span>
| <span data-ttu-id="a8134-128">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a8134-128">Relationship</span></span> | <span data-ttu-id="a8134-129">型</span><span class="sxs-lookup"><span data-stu-id="a8134-129">Type</span></span>   |<span data-ttu-id="a8134-130">説明</span><span class="sxs-lookup"><span data-stu-id="a8134-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a8134-131">format</span><span class="sxs-lookup"><span data-stu-id="a8134-131">format</span></span>|[<span data-ttu-id="a8134-132">WorkbookChartLegendFormat</span><span class="sxs-lookup"><span data-stu-id="a8134-132">WorkbookChartLegendFormat</span></span>](chartlegendformat.md)|<span data-ttu-id="a8134-p102">グラフの凡例の書式設定を表します。これには塗りつぶしとフォントの書式設定などがあります。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a8134-p102">Represents the formatting of a chart legend, which includes fill and font formatting. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a8134-135">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a8134-135">JSON representation</span></span>

<span data-ttu-id="a8134-136">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a8134-136">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookChartLegend"
}-->

```json
{
  "overlay": true,
  "position": "string",
  "visible": true,
  "format": {"@odata.type":"microsoft.graph.workbookChartLegendFormat"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartLegend resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->