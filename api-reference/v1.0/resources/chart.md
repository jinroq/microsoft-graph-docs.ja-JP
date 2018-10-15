# <a name="chart-resource-type"></a><span data-ttu-id="a66a4-101">グラフ リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a66a4-101">Chart resource type</span></span>

<span data-ttu-id="a66a4-102">ブック内のグラフ オブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="a66a4-102">Represents a chart object in a workbook.</span></span>


## <a name="methods"></a><span data-ttu-id="a66a4-103">メソッド</span><span class="sxs-lookup"><span data-stu-id="a66a4-103">Methods</span></span>

| <span data-ttu-id="a66a4-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="a66a4-104">Method</span></span>           | <span data-ttu-id="a66a4-105">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="a66a4-105">Return Type</span></span>    |<span data-ttu-id="a66a4-106">説明</span><span class="sxs-lookup"><span data-stu-id="a66a4-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a66a4-107">Get Chart</span><span class="sxs-lookup"><span data-stu-id="a66a4-107">Get Chart</span></span>](../api/chart_get.md) | [<span data-ttu-id="a66a4-108">WorkbookChart</span><span class="sxs-lookup"><span data-stu-id="a66a4-108">WorkbookChart</span></span>](chart.md) |<span data-ttu-id="a66a4-109">グラフ オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="a66a4-109">Read properties and relationships of chart object.</span></span>|
|[<span data-ttu-id="a66a4-110">Create ChartSeries</span><span class="sxs-lookup"><span data-stu-id="a66a4-110">Create ChartSeries</span></span>](../api/chart_post_series.md) |[<span data-ttu-id="a66a4-111">WorkbookChartSeries</span><span class="sxs-lookup"><span data-stu-id="a66a4-111">WorkbookChartSeries</span></span>](chartseries.md)| <span data-ttu-id="a66a4-112">データ系列のコレクションに投稿して、新しい ChartSeries を作成します。</span><span class="sxs-lookup"><span data-stu-id="a66a4-112">Create a new ChartSeries by posting to the series collection.</span></span>|
|[<span data-ttu-id="a66a4-113">List series</span><span class="sxs-lookup"><span data-stu-id="a66a4-113">List series</span></span>](../api/chart_list_series.md) |<span data-ttu-id="a66a4-114">[WorkbookChartSeries](chartseries.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a66a4-114">[WorkbookChartSeries](chartseries.md) collection</span></span>| <span data-ttu-id="a66a4-115">ChartSeries オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="a66a4-115">Get a ChartSeries object collection.</span></span>|
|[<span data-ttu-id="a66a4-116">Update</span><span class="sxs-lookup"><span data-stu-id="a66a4-116">Update</span></span>](../api/chart_update.md) | [<span data-ttu-id="a66a4-117">WorkbookChart</span><span class="sxs-lookup"><span data-stu-id="a66a4-117">WorkbookChart</span></span>](chart.md)   |<span data-ttu-id="a66a4-118">グラフ オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="a66a4-118">Update Chart object.</span></span> |
|[<span data-ttu-id="a66a4-119">Image</span><span class="sxs-lookup"><span data-stu-id="a66a4-119">Image</span></span>](../api/chart_image.md)|<span data-ttu-id="a66a4-120">Base64 でエンコードされた文字列の画像</span><span class="sxs-lookup"><span data-stu-id="a66a4-120">Image base64 encoded string</span></span>|<span data-ttu-id="a66a4-121">指定したサイズに合わせてグラフを拡大・縮小することで、グラフを Base64 でエンコードされた画像としてレンダリングします。</span><span class="sxs-lookup"><span data-stu-id="a66a4-121">Renders the chart as a base64-encoded image by scaling the chart to fit the specified dimensions.</span></span>|
|[<span data-ttu-id="a66a4-122">Delete</span><span class="sxs-lookup"><span data-stu-id="a66a4-122">Delete</span></span>](../api/chart_delete.md)|<span data-ttu-id="a66a4-123">なし</span><span class="sxs-lookup"><span data-stu-id="a66a4-123">None</span></span>|<span data-ttu-id="a66a4-124">グラフ オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="a66a4-124">Deletes the chart object.</span></span>|
|[<span data-ttu-id="a66a4-125">Setdata</span><span class="sxs-lookup"><span data-stu-id="a66a4-125">Setdata</span></span>](../api/chart_setdata.md)|<span data-ttu-id="a66a4-126">なし</span><span class="sxs-lookup"><span data-stu-id="a66a4-126">None</span></span>|<span data-ttu-id="a66a4-127">グラフのソース データをリセットします。</span><span class="sxs-lookup"><span data-stu-id="a66a4-127">Resets the source data for the chart.</span></span>|
|[<span data-ttu-id="a66a4-128">Setposition</span><span class="sxs-lookup"><span data-stu-id="a66a4-128">Setposition</span></span>](../api/chart_setposition.md)|<span data-ttu-id="a66a4-129">なし</span><span class="sxs-lookup"><span data-stu-id="a66a4-129">None</span></span>|<span data-ttu-id="a66a4-130">ワークシート上のセルを基準にしてグラフを配置します。</span><span class="sxs-lookup"><span data-stu-id="a66a4-130">Positions the chart relative to cells on the worksheet.</span></span>|
|[<span data-ttu-id="a66a4-131">List</span><span class="sxs-lookup"><span data-stu-id="a66a4-131">List</span></span>](../api/chart_list.md) | <span data-ttu-id="a66a4-132">[WorkbookChart](chart.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a66a4-132">[WorkbookChart](chart.md) collection</span></span> |<span data-ttu-id="a66a4-133">グラフ オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="a66a4-133">Get chart object collection.</span></span> |
|[<span data-ttu-id="a66a4-134">Itemat</span><span class="sxs-lookup"><span data-stu-id="a66a4-134">Itemat</span></span>](../api/chartcollection_itemat.md)|[<span data-ttu-id="a66a4-135">WorkbookChart</span><span class="sxs-lookup"><span data-stu-id="a66a4-135">WorkbookChart</span></span>](chart.md)|<span data-ttu-id="a66a4-136">コレクション内での位置を基にグラフを取得します。</span><span class="sxs-lookup"><span data-stu-id="a66a4-136">Gets a chart based on its position in the collection.</span></span>|
|[<span data-ttu-id="a66a4-137">Add</span><span class="sxs-lookup"><span data-stu-id="a66a4-137">Add</span></span>](../api/chartcollection_add.md)|[<span data-ttu-id="a66a4-138">WorkbookChart</span><span class="sxs-lookup"><span data-stu-id="a66a4-138">WorkbookChart</span></span>](chart.md)|<span data-ttu-id="a66a4-139">新しいグラフを作成します。</span><span class="sxs-lookup"><span data-stu-id="a66a4-139">Creates a new chart.</span></span>|

## <a name="properties"></a><span data-ttu-id="a66a4-140">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a66a4-140">Properties</span></span>
| <span data-ttu-id="a66a4-141">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a66a4-141">Property</span></span>     | <span data-ttu-id="a66a4-142">タイプ</span><span class="sxs-lookup"><span data-stu-id="a66a4-142">Type</span></span>   |<span data-ttu-id="a66a4-143">説明</span><span class="sxs-lookup"><span data-stu-id="a66a4-143">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a66a4-144">height</span><span class="sxs-lookup"><span data-stu-id="a66a4-144">height</span></span>|<span data-ttu-id="a66a4-145">double</span><span class="sxs-lookup"><span data-stu-id="a66a4-145">double</span></span>|<span data-ttu-id="a66a4-146">グラフ オブジェクトの高さをポイント単位で表します。</span><span class="sxs-lookup"><span data-stu-id="a66a4-146">Represents the height, in points, of the chart object.</span></span>|
|<span data-ttu-id="a66a4-147">id</span><span class="sxs-lookup"><span data-stu-id="a66a4-147">id</span></span>|<span data-ttu-id="a66a4-148">文字列</span><span class="sxs-lookup"><span data-stu-id="a66a4-148">string</span></span>|<span data-ttu-id="a66a4-p101">コレクション内での位置を基にグラフを取得します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a66a4-p101">Gets a chart based on its position in the collection. Read-only.</span></span>|
|<span data-ttu-id="a66a4-151">left</span><span class="sxs-lookup"><span data-stu-id="a66a4-151">left</span></span>|<span data-ttu-id="a66a4-152">double</span><span class="sxs-lookup"><span data-stu-id="a66a4-152">double</span></span>|<span data-ttu-id="a66a4-153">グラフの左側からワークシートの原点までの距離 (ポイント単位)。</span><span class="sxs-lookup"><span data-stu-id="a66a4-153">The distance, in points, from the left side of the chart to the worksheet origin.</span></span>|
|<span data-ttu-id="a66a4-154">name</span><span class="sxs-lookup"><span data-stu-id="a66a4-154">name</span></span>|<span data-ttu-id="a66a4-155">文字列</span><span class="sxs-lookup"><span data-stu-id="a66a4-155">string</span></span>|<span data-ttu-id="a66a4-156">グラフ オブジェクトの名前を表します。</span><span class="sxs-lookup"><span data-stu-id="a66a4-156">Represents the name of a chart object.</span></span>|
|<span data-ttu-id="a66a4-157">top</span><span class="sxs-lookup"><span data-stu-id="a66a4-157">top</span></span>|<span data-ttu-id="a66a4-158">double</span><span class="sxs-lookup"><span data-stu-id="a66a4-158">double</span></span>|<span data-ttu-id="a66a4-159">オブジェクトの上端から (ワークシートの) 1 行目の上部または (グラフの) グラフ領域の上部までの距離をポイント単位で表します。</span><span class="sxs-lookup"><span data-stu-id="a66a4-159">Represents the distance, in points, from the top edge of the object to the top of row 1 (on a worksheet) or the top of the chart area (on a chart).</span></span>|
|<span data-ttu-id="a66a4-160">width</span><span class="sxs-lookup"><span data-stu-id="a66a4-160">width</span></span>|<span data-ttu-id="a66a4-161">double</span><span class="sxs-lookup"><span data-stu-id="a66a4-161">double</span></span>|<span data-ttu-id="a66a4-162">グラフ オブジェクトの幅をポイント単位で表します。</span><span class="sxs-lookup"><span data-stu-id="a66a4-162">Represents the width, in points, of the chart object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a66a4-163">関係</span><span class="sxs-lookup"><span data-stu-id="a66a4-163">Relationships</span></span>
| <span data-ttu-id="a66a4-164">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a66a4-164">Relationship</span></span> | <span data-ttu-id="a66a4-165">型</span><span class="sxs-lookup"><span data-stu-id="a66a4-165">Type</span></span>   |<span data-ttu-id="a66a4-166">説明</span><span class="sxs-lookup"><span data-stu-id="a66a4-166">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a66a4-167">axes</span><span class="sxs-lookup"><span data-stu-id="a66a4-167">axes</span></span>|[<span data-ttu-id="a66a4-168">WorkbookChartAxes</span><span class="sxs-lookup"><span data-stu-id="a66a4-168">WorkbookChartAxes</span></span>](chartaxes.md)|<span data-ttu-id="a66a4-p102">グラフの軸を表します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a66a4-p102">Represents chart axes. Read-only.</span></span>|
|<span data-ttu-id="a66a4-171">dataLabels</span><span class="sxs-lookup"><span data-stu-id="a66a4-171">dataLabels</span></span>|[<span data-ttu-id="a66a4-172">WorkbookChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="a66a4-172">WorkbookChartDataLabels</span></span>](chartdatalabels.md)|<span data-ttu-id="a66a4-p103">グラフ上のデータラベルを表します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a66a4-p103">Represents the datalabels on the chart. Read-only.</span></span>|
|<span data-ttu-id="a66a4-175">format</span><span class="sxs-lookup"><span data-stu-id="a66a4-175">format</span></span>|[<span data-ttu-id="a66a4-176">WorkbookChartAreaFormat</span><span class="sxs-lookup"><span data-stu-id="a66a4-176">WorkbookChartAreaFormat</span></span>](chartareaformat.md)|<span data-ttu-id="a66a4-p104">グラフ領域の書式設定プロパティをカプセル化します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a66a4-p104">Encapsulates the format properties for the chart area. Read-only.</span></span>|
|<span data-ttu-id="a66a4-179">legend</span><span class="sxs-lookup"><span data-stu-id="a66a4-179">legend</span></span>|[<span data-ttu-id="a66a4-180">WorkbookChartLegend</span><span class="sxs-lookup"><span data-stu-id="a66a4-180">WorkbookChartLegend</span></span>](chartlegend.md)|<span data-ttu-id="a66a4-p105">グラフの凡例を表します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a66a4-p105">Represents the legend for the chart. Read-only.</span></span>|
|<span data-ttu-id="a66a4-183">series</span><span class="sxs-lookup"><span data-stu-id="a66a4-183">series</span></span>|<span data-ttu-id="a66a4-184">[WorkbookChartSeries](chartseries.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a66a4-184">[WorkbookChartSeries](chartseries.md) collection</span></span>|<span data-ttu-id="a66a4-p106">グラフの 1 つのデータ系列またはデータ系列のコレクションを表します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a66a4-p106">Represents either a single series or collection of series in the chart. Read-only.</span></span>|
|<span data-ttu-id="a66a4-187">title</span><span class="sxs-lookup"><span data-stu-id="a66a4-187">title</span></span>|[<span data-ttu-id="a66a4-188">WorkbookChartTitle</span><span class="sxs-lookup"><span data-stu-id="a66a4-188">WorkbookChartTitle</span></span>](charttitle.md)|<span data-ttu-id="a66a4-p107">指定したグラフのタイトル (タイトルのテキスト、表示/非表示、位置、書式設定など) を表します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a66a4-p107">Represents the title of the specified chart, including the text, visibility, position and formating of the title. Read-only.</span></span>|
|<span data-ttu-id="a66a4-191">worksheet</span><span class="sxs-lookup"><span data-stu-id="a66a4-191">worksheet</span></span>|[<span data-ttu-id="a66a4-192">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="a66a4-192">WorkbookWorksheet</span></span>](worksheet.md)|<span data-ttu-id="a66a4-p108">現在のグラフを含んでいるワークシート。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a66a4-p108">The worksheet containing the current chart. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a66a4-195">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a66a4-195">JSON representation</span></span>

<span data-ttu-id="a66a4-196">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a66a4-196">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChart"
}-->

```json
{
  "height": 1024,
  "id": "string",
  "left": 1024,
  "name": "string",
  "top": 1024,
  "width": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Chart resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->