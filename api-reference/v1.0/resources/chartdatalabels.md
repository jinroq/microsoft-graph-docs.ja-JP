# <a name="chartdatalabels-resource-type"></a><span data-ttu-id="3698e-101">ChartDataLabels リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3698e-101">ChartDataLabels resource type</span></span>

<span data-ttu-id="3698e-102">グラフのポイントにあるすべてのデータ ラベルのコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="3698e-102">Represents a collection of all the data labels on a chart point.</span></span>


## <a name="methods"></a><span data-ttu-id="3698e-103">メソッド</span><span class="sxs-lookup"><span data-stu-id="3698e-103">Methods</span></span>

| <span data-ttu-id="3698e-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="3698e-104">Method</span></span>           | <span data-ttu-id="3698e-105">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="3698e-105">Return Type</span></span>    |<span data-ttu-id="3698e-106">説明</span><span class="sxs-lookup"><span data-stu-id="3698e-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3698e-107">Get ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="3698e-107">Get ChartDataLabels</span></span>](../api/chartdatalabels_get.md) | [<span data-ttu-id="3698e-108">WorkbookChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="3698e-108">WorkbookChartDataLabels</span></span>](chartdatalabels.md) |<span data-ttu-id="3698e-109">chartDataLabels オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="3698e-109">Read properties and relationships of chartDataLabels object.</span></span>|
|[<span data-ttu-id="3698e-110">Update</span><span class="sxs-lookup"><span data-stu-id="3698e-110">Update</span></span>](../api/chartdatalabels_update.md) | [<span data-ttu-id="3698e-111">WorkbookChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="3698e-111">WorkbookChartDataLabels</span></span>](chartdatalabels.md) |<span data-ttu-id="3698e-112">ChartDataLabels オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="3698e-112">Update ChartDataLabels object.</span></span> |

## <a name="properties"></a><span data-ttu-id="3698e-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3698e-113">Properties</span></span>
| <span data-ttu-id="3698e-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3698e-114">Property</span></span>     | <span data-ttu-id="3698e-115">タイプ</span><span class="sxs-lookup"><span data-stu-id="3698e-115">Type</span></span>   |<span data-ttu-id="3698e-116">説明</span><span class="sxs-lookup"><span data-stu-id="3698e-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3698e-117">position</span><span class="sxs-lookup"><span data-stu-id="3698e-117">position</span></span>|<span data-ttu-id="3698e-118">string</span><span class="sxs-lookup"><span data-stu-id="3698e-118">string</span></span>|<span data-ttu-id="3698e-119">データ ラベルの位置を表すDataLabelPosition の値。</span><span class="sxs-lookup"><span data-stu-id="3698e-119">DataLabelPosition value that represents the position of the data label. Possible values are: , , , , , , , , , , .</span></span> <span data-ttu-id="3698e-120">可能な値は、`None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout` です。</span><span class="sxs-lookup"><span data-stu-id="3698e-120">The possible values are `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`, or .</span></span>|
|<span data-ttu-id="3698e-121">separator</span><span class="sxs-lookup"><span data-stu-id="3698e-121">separator</span></span>|<span data-ttu-id="3698e-122">string</span><span class="sxs-lookup"><span data-stu-id="3698e-122">string</span></span>|<span data-ttu-id="3698e-123">グラフのデータ ラベルに使用される区切り文字を表す文字列を設定します。</span><span class="sxs-lookup"><span data-stu-id="3698e-123">String representing the separator used for the data labels on a chart.</span></span>|
|<span data-ttu-id="3698e-124">showBubbleSize</span><span class="sxs-lookup"><span data-stu-id="3698e-124">showBubbleSize</span></span>|<span data-ttu-id="3698e-125">boolean</span><span class="sxs-lookup"><span data-stu-id="3698e-125">boolean</span></span>|<span data-ttu-id="3698e-126">データ ラベルのバブルのサイズを表示または非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="3698e-126">Boolean value representing if the data label bubble size is visible or not.</span></span>|
|<span data-ttu-id="3698e-127">showCategoryName</span><span class="sxs-lookup"><span data-stu-id="3698e-127">showCategoryName</span></span>|<span data-ttu-id="3698e-128">boolean</span><span class="sxs-lookup"><span data-stu-id="3698e-128">boolean</span></span>|<span data-ttu-id="3698e-129">データ ラベルのカテゴリ名を表示するか非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="3698e-129">Boolean value representing if the data label category name is visible or not.</span></span>|
|<span data-ttu-id="3698e-130">showLegendKey</span><span class="sxs-lookup"><span data-stu-id="3698e-130">showLegendKey</span></span>|<span data-ttu-id="3698e-131">boolean</span><span class="sxs-lookup"><span data-stu-id="3698e-131">boolean</span></span>|<span data-ttu-id="3698e-132">データ ラベルの凡例マーカーを表示するか非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="3698e-132">Boolean value representing if the data label legend key is visible or not.</span></span>|
|<span data-ttu-id="3698e-133">showPercentage</span><span class="sxs-lookup"><span data-stu-id="3698e-133">showPercentage</span></span>|<span data-ttu-id="3698e-134">boolean</span><span class="sxs-lookup"><span data-stu-id="3698e-134">boolean</span></span>|<span data-ttu-id="3698e-135">データ ラベルのパーセンテージを表示するか非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="3698e-135">Boolean value representing if the data label percentage is visible or not.</span></span>|
|<span data-ttu-id="3698e-136">showSeriesName</span><span class="sxs-lookup"><span data-stu-id="3698e-136">showSeriesName</span></span>|<span data-ttu-id="3698e-137">boolean</span><span class="sxs-lookup"><span data-stu-id="3698e-137">boolean</span></span>|<span data-ttu-id="3698e-138">データ ラベルの系列名を表示するか非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="3698e-138">Boolean value representing if the data label series name is visible or not.</span></span>|
|<span data-ttu-id="3698e-139">showValue</span><span class="sxs-lookup"><span data-stu-id="3698e-139">showValue</span></span>|<span data-ttu-id="3698e-140">boolean</span><span class="sxs-lookup"><span data-stu-id="3698e-140">boolean</span></span>|<span data-ttu-id="3698e-141">データ ラベルの値を表示するか非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="3698e-141">Boolean value representing if the data label value is visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3698e-142">関係</span><span class="sxs-lookup"><span data-stu-id="3698e-142">Relationships</span></span>
| <span data-ttu-id="3698e-143">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="3698e-143">Relationship</span></span> | <span data-ttu-id="3698e-144">型</span><span class="sxs-lookup"><span data-stu-id="3698e-144">Type</span></span>   |<span data-ttu-id="3698e-145">説明</span><span class="sxs-lookup"><span data-stu-id="3698e-145">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3698e-146">format</span><span class="sxs-lookup"><span data-stu-id="3698e-146">format</span></span>|[<span data-ttu-id="3698e-147">WorkbookChartDataLabelFormat</span><span class="sxs-lookup"><span data-stu-id="3698e-147">WorkbookChartDataLabelFormat</span></span>](chartdatalabelformat.md)|<span data-ttu-id="3698e-p102">グラフのデータ ラベルの書式 (塗りつぶしとフォントの書式設定を含む) を表します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="3698e-p102">Represents the format of chart data labels, which includes fill and font formatting. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3698e-150">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3698e-150">JSON representation</span></span>

<span data-ttu-id="3698e-151">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3698e-151">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.workbookChartDataLabels"
}-->

```json
{
  "position": "string",
  "separator": "string",
  "showBubbleSize": true,
  "showCategoryName": true,
  "showLegendKey": true,
  "showPercentage": true,
  "showSeriesName": true,
  "showValue": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartDataLabels resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->