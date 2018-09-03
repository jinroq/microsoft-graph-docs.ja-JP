# <a name="chartseries-resource-type"></a><span data-ttu-id="ada97-101">ChartSeries リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ada97-101">ChartSeries resource type</span></span>

<span data-ttu-id="ada97-102">グラフのデータ系列を表します。</span><span class="sxs-lookup"><span data-stu-id="ada97-102">Represents a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="ada97-103">メソッド</span><span class="sxs-lookup"><span data-stu-id="ada97-103">Methods</span></span>

| <span data-ttu-id="ada97-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="ada97-104">Method</span></span>           | <span data-ttu-id="ada97-105">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ada97-105">Return Type</span></span>    |<span data-ttu-id="ada97-106">説明</span><span class="sxs-lookup"><span data-stu-id="ada97-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ada97-107">ChartSeries を取得する</span><span class="sxs-lookup"><span data-stu-id="ada97-107">Get ChartSeries</span></span>](../api/chartseries_get.md) | [<span data-ttu-id="ada97-108">WorkbookChartSeries</span><span class="sxs-lookup"><span data-stu-id="ada97-108">WorkbookChartSeries</span></span>](chartseries.md) |<span data-ttu-id="ada97-109">chartSeries オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="ada97-109">Read properties and relationships of chartSeries object.</span></span>|
|[<span data-ttu-id="ada97-110">ChartPoints を作成する</span><span class="sxs-lookup"><span data-stu-id="ada97-110">Create ChartPoints</span></span>](../api/chartseries_post_points.md) |[<span data-ttu-id="ada97-111">ChartPoints</span><span class="sxs-lookup"><span data-stu-id="ada97-111">ChartPoints</span></span>](chartpoint.md)| <span data-ttu-id="ada97-112">ポイント コレクションに投稿して、新しい ChartPoints を作成します。</span><span class="sxs-lookup"><span data-stu-id="ada97-112">Create a new ChartPoints by posting to the points collection.</span></span>|
|[<span data-ttu-id="ada97-113">ポイントを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="ada97-113">List points</span></span>](../api/chartseries_list_points.md) |<span data-ttu-id="ada97-114">[ChartPoints](chartpoint.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ada97-114">[ChartPoints](chartpoint.md) collection</span></span>| <span data-ttu-id="ada97-115">ChartPoints オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="ada97-115">Get a ChartPoints object collection.</span></span>|
|[<span data-ttu-id="ada97-116">更新する</span><span class="sxs-lookup"><span data-stu-id="ada97-116">Update</span></span>](../api/chartseries_update.md) | [<span data-ttu-id="ada97-117">WorkbookChartSeries</span><span class="sxs-lookup"><span data-stu-id="ada97-117">WorkbookChartSeries</span></span>](chartseries.md) |<span data-ttu-id="ada97-118">ChartSeries オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="ada97-118">Update ChartSeries object.</span></span> |
|[<span data-ttu-id="ada97-119">リスト</span><span class="sxs-lookup"><span data-stu-id="ada97-119">List</span></span>](../api/chartseries_list.md) | <span data-ttu-id="ada97-120">[WorkbookChartSeries](chartseries.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ada97-120">[WorkbookChartSeries](chartseries.md) collection</span></span> |<span data-ttu-id="ada97-121">chartSeries オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="ada97-121">Get chartSeries object collection.</span></span> |
|[<span data-ttu-id="ada97-122">Itemat</span><span class="sxs-lookup"><span data-stu-id="ada97-122">Itemat</span></span>](../api/chartseriescollection_itemat.md)|[<span data-ttu-id="ada97-123">WorkbookChartSeries</span><span class="sxs-lookup"><span data-stu-id="ada97-123">WorkbookChartSeries</span></span>](chartseries.md)|<span data-ttu-id="ada97-124">コレクション内の位置に基づいてデータ系列を取得します。</span><span class="sxs-lookup"><span data-stu-id="ada97-124">Retrieves a series based on its position in the collection</span></span>|

## <a name="properties"></a><span data-ttu-id="ada97-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ada97-125">Properties</span></span>
| <span data-ttu-id="ada97-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ada97-126">Property</span></span>     | <span data-ttu-id="ada97-127">タイプ</span><span class="sxs-lookup"><span data-stu-id="ada97-127">Type</span></span>   |<span data-ttu-id="ada97-128">説明</span><span class="sxs-lookup"><span data-stu-id="ada97-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ada97-129">名前</span><span class="sxs-lookup"><span data-stu-id="ada97-129">name</span></span>|<span data-ttu-id="ada97-130">文字列</span><span class="sxs-lookup"><span data-stu-id="ada97-130">string</span></span>|<span data-ttu-id="ada97-131">グラフのデータ系列の名前を表します。</span><span class="sxs-lookup"><span data-stu-id="ada97-131">Represents the name of a series in a chart.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ada97-132">関係</span><span class="sxs-lookup"><span data-stu-id="ada97-132">Relationships</span></span>
| <span data-ttu-id="ada97-133">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ada97-133">Relationship</span></span> | <span data-ttu-id="ada97-134">型</span><span class="sxs-lookup"><span data-stu-id="ada97-134">Type</span></span>   |<span data-ttu-id="ada97-135">説明</span><span class="sxs-lookup"><span data-stu-id="ada97-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ada97-136">形式</span><span class="sxs-lookup"><span data-stu-id="ada97-136">format</span></span>|[<span data-ttu-id="ada97-137">WorkbookChartSeriesFormat</span><span class="sxs-lookup"><span data-stu-id="ada97-137">WorkbookChartSeriesFormat</span></span>](chartseriesformat.md)|<span data-ttu-id="ada97-p101">グラフ の系列の書式設定を表します。これには塗りつぶしと線の書式設定などがあります。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="ada97-p101">Represents the formatting of a chart series, which includes fill and line formatting. Read-only.</span></span>|
|<span data-ttu-id="ada97-140">ポイント</span><span class="sxs-lookup"><span data-stu-id="ada97-140">points</span></span>|<span data-ttu-id="ada97-141">[WorkbookChartPoint](chartpoint.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ada97-141">[WorkbookChartPoint](chartpoint.md) collection</span></span>|<span data-ttu-id="ada97-p102">データ系列にあるすべてのポイントのコレクションを返します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="ada97-p102">Represents a collection of all points in the series. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ada97-144">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ada97-144">JSON representation</span></span>

<span data-ttu-id="ada97-145">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ada97-145">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookChartSeries"
}-->

```json
{
  "name": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartSeries resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->