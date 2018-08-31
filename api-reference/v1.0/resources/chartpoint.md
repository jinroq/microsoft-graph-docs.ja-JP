# <a name="chartpoint-resource-type"></a><span data-ttu-id="09d2b-101">ChartPoint リソースの種類</span><span class="sxs-lookup"><span data-stu-id="09d2b-101">ChartPoint resource type</span></span>

<span data-ttu-id="09d2b-102">グラフの系列のポイントを表します。</span><span class="sxs-lookup"><span data-stu-id="09d2b-102">Represents a point of a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="09d2b-103">メソッド</span><span class="sxs-lookup"><span data-stu-id="09d2b-103">Methods</span></span>

| <span data-ttu-id="09d2b-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="09d2b-104">Method</span></span>           | <span data-ttu-id="09d2b-105">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="09d2b-105">Return Type</span></span>    |<span data-ttu-id="09d2b-106">説明</span><span class="sxs-lookup"><span data-stu-id="09d2b-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="09d2b-107">ChartPoint の取得</span><span class="sxs-lookup"><span data-stu-id="09d2b-107">Get ChartPoint</span></span>](../api/chartpoint_get.md) | [<span data-ttu-id="09d2b-108">WorkbookChartPoint</span><span class="sxs-lookup"><span data-stu-id="09d2b-108">WorkbookChartPoint</span></span>](chartpoint.md) |<span data-ttu-id="09d2b-109">chartPoint オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="09d2b-109">Read properties and relationships of chartPoint object.</span></span>|
|[<span data-ttu-id="09d2b-110">List</span><span class="sxs-lookup"><span data-stu-id="09d2b-110">List</span></span>](../api/chartpoint_list.md) | <span data-ttu-id="09d2b-111">[WorkbookChartPoint](chartpoint.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="09d2b-111">[WorkbookChartPoint](chartpoint.md) collection</span></span> |<span data-ttu-id="09d2b-112">chartPoint オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="09d2b-112">Get chartPoint object collection.</span></span> |
|[<span data-ttu-id="09d2b-113">Itemat</span><span class="sxs-lookup"><span data-stu-id="09d2b-113">Itemat</span></span>](../api/chartpointscollection_itemat.md)|[<span data-ttu-id="09d2b-114">WorkbookChartPoint</span><span class="sxs-lookup"><span data-stu-id="09d2b-114">WorkbookChartPoint</span></span>](chartpoint.md)|<span data-ttu-id="09d2b-115">データ系列内の位置に基づくポイントを取得します。</span><span class="sxs-lookup"><span data-stu-id="09d2b-115">Retrieve a point based on its position within the series.</span></span>|

## <a name="properties"></a><span data-ttu-id="09d2b-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="09d2b-116">Properties</span></span>
| <span data-ttu-id="09d2b-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="09d2b-117">Property</span></span>     | <span data-ttu-id="09d2b-118">タイプ</span><span class="sxs-lookup"><span data-stu-id="09d2b-118">Type</span></span>   |<span data-ttu-id="09d2b-119">説明</span><span class="sxs-lookup"><span data-stu-id="09d2b-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="09d2b-120">値</span><span class="sxs-lookup"><span data-stu-id="09d2b-120">value</span></span>|<span data-ttu-id="09d2b-121">Json</span><span class="sxs-lookup"><span data-stu-id="09d2b-121">Json</span></span>|<span data-ttu-id="09d2b-p101">グラフのポイントの値を返します。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="09d2b-p101">Returns the value of a chart point. Read-only.</span></span>|
|<span data-ttu-id="09d2b-124">ID</span><span class="sxs-lookup"><span data-stu-id="09d2b-124">id</span></span>|<span data-ttu-id="09d2b-125">文字列</span><span class="sxs-lookup"><span data-stu-id="09d2b-125">string</span></span>|<span data-ttu-id="09d2b-126">一意識別子</span><span class="sxs-lookup"><span data-stu-id="09d2b-126">unique identifier</span></span>|

## <a name="relationships"></a><span data-ttu-id="09d2b-127">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="09d2b-127">Relationships</span></span>
| <span data-ttu-id="09d2b-128">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="09d2b-128">Relationship</span></span> | <span data-ttu-id="09d2b-129">型</span><span class="sxs-lookup"><span data-stu-id="09d2b-129">Type</span></span>   |<span data-ttu-id="09d2b-130">説明</span><span class="sxs-lookup"><span data-stu-id="09d2b-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="09d2b-131">format</span><span class="sxs-lookup"><span data-stu-id="09d2b-131">format</span></span>|[<span data-ttu-id="09d2b-132">WorkbookChartPointFormat</span><span class="sxs-lookup"><span data-stu-id="09d2b-132">WorkbookChartPointFormat</span></span>](chartpointformat.md)|<span data-ttu-id="09d2b-p102">グラフのポイントの書式設定プロパティをカプセル化します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="09d2b-p102">Encapsulates the format properties chart point. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="09d2b-135">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="09d2b-135">JSON representation</span></span>

<span data-ttu-id="09d2b-136">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="09d2b-136">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartPoint"
}-->

```json
{
  "value": "string",
  "id": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartPoint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->