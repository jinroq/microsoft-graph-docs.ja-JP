# <a name="chartaxes-resource-type"></a><span data-ttu-id="fc055-101">ChartAxes リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fc055-101">ChartAxes resource type</span></span>

<span data-ttu-id="fc055-102">グラフの軸を表します。</span><span class="sxs-lookup"><span data-stu-id="fc055-102">Represents the chart axes.</span></span>


## <a name="methods"></a><span data-ttu-id="fc055-103">メソッド</span><span class="sxs-lookup"><span data-stu-id="fc055-103">Methods</span></span>
<span data-ttu-id="fc055-104">なし</span><span class="sxs-lookup"><span data-stu-id="fc055-104">None</span></span>

## <a name="properties"></a><span data-ttu-id="fc055-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fc055-105">Properties</span></span>
<span data-ttu-id="fc055-106">なし</span><span class="sxs-lookup"><span data-stu-id="fc055-106">None</span></span>

## <a name="relationships"></a><span data-ttu-id="fc055-107">関係</span><span class="sxs-lookup"><span data-stu-id="fc055-107">Relationships</span></span>
| <span data-ttu-id="fc055-108">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="fc055-108">Relationship</span></span> | <span data-ttu-id="fc055-109">型</span><span class="sxs-lookup"><span data-stu-id="fc055-109">Type</span></span>   |<span data-ttu-id="fc055-110">説明</span><span class="sxs-lookup"><span data-stu-id="fc055-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fc055-111">categoryAxis</span><span class="sxs-lookup"><span data-stu-id="fc055-111">categoryAxis</span></span>|[<span data-ttu-id="fc055-112">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="fc055-112">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="fc055-p101">グラフの項目軸を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="fc055-p101">Represents the category axis in a chart. Read-only.</span></span>|
|<span data-ttu-id="fc055-115">seriesAxis</span><span class="sxs-lookup"><span data-stu-id="fc055-115">seriesAxis</span></span>|[<span data-ttu-id="fc055-116">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="fc055-116">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="fc055-p102">3 次元グラフの系列軸を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="fc055-p102">Represents the series axis of a 3-dimensional chart. Read-only.</span></span>|
|<span data-ttu-id="fc055-119">valueAxis</span><span class="sxs-lookup"><span data-stu-id="fc055-119">valueAxis</span></span>|[<span data-ttu-id="fc055-120">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="fc055-120">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="fc055-p103">軸の数値軸を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="fc055-p103">Represents the value axis in an axis. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fc055-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fc055-123">JSON representation</span></span>

<span data-ttu-id="fc055-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="fc055-124">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartAxes"
}-->

```json
{
  "categoryAxis": {"@odata.type": "microsoft.graph.workbookChartAxis"},
  "seriesAxis": {"@odata.type": "microsoft.graph.workbookChartAxis"},
  "valueAxis": {"@odata.type": "microsoft.graph.workbookChartAxis"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartAxes resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->