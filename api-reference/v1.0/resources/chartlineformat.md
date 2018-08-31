# <a name="chartlineformat-resource-type"></a><span data-ttu-id="3b0bc-101">ChartLineFormat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3b0bc-101">ChartLineFormat resource type</span></span>

<span data-ttu-id="3b0bc-102">直線要素の書式設定オプションをカプセル化します。</span><span class="sxs-lookup"><span data-stu-id="3b0bc-102">Enapsulates the formatting options for line elements.</span></span>


## <a name="methods"></a><span data-ttu-id="3b0bc-103">メソッド</span><span class="sxs-lookup"><span data-stu-id="3b0bc-103">Methods</span></span>

| <span data-ttu-id="3b0bc-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="3b0bc-104">Method</span></span>           | <span data-ttu-id="3b0bc-105">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="3b0bc-105">Return Type</span></span>    |<span data-ttu-id="3b0bc-106">説明</span><span class="sxs-lookup"><span data-stu-id="3b0bc-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3b0bc-107">ChartLineFormat を取得する</span><span class="sxs-lookup"><span data-stu-id="3b0bc-107">Get ChartLineFormat</span></span>](../api/chartlineformat_get.md) | [<span data-ttu-id="3b0bc-108">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="3b0bc-108">WorkbookChartLineFormat</span></span>](chartlineformat.md) |<span data-ttu-id="3b0bc-109">chartLineFormat オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="3b0bc-109">Read properties and relationships of chartLineFormat object.</span></span>|
|[<span data-ttu-id="3b0bc-110">更新</span><span class="sxs-lookup"><span data-stu-id="3b0bc-110">Update</span></span>](../api/chartlineformat_update.md) | [<span data-ttu-id="3b0bc-111">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="3b0bc-111">WorkbookChartLineFormat</span></span>](chartlineformat.md) |<span data-ttu-id="3b0bc-112">ChartLineFormat オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="3b0bc-112">Update ChartLineFormat object.</span></span> |
|[<span data-ttu-id="3b0bc-113">Clear</span><span class="sxs-lookup"><span data-stu-id="3b0bc-113">Clear</span></span>](../api/chartlineformat_clear.md)|<span data-ttu-id="3b0bc-114">なし</span><span class="sxs-lookup"><span data-stu-id="3b0bc-114">None</span></span>|<span data-ttu-id="3b0bc-115">グラフ要素の線の書式をクリアします。</span><span class="sxs-lookup"><span data-stu-id="3b0bc-115">Clear the line format of a chart element.</span></span>|

## <a name="properties"></a><span data-ttu-id="3b0bc-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3b0bc-116">Properties</span></span>
| <span data-ttu-id="3b0bc-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3b0bc-117">Property</span></span>     | <span data-ttu-id="3b0bc-118">タイプ</span><span class="sxs-lookup"><span data-stu-id="3b0bc-118">Type</span></span>   |<span data-ttu-id="3b0bc-119">説明</span><span class="sxs-lookup"><span data-stu-id="3b0bc-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3b0bc-120">color</span><span class="sxs-lookup"><span data-stu-id="3b0bc-120">color</span></span>|<span data-ttu-id="3b0bc-121">文字列</span><span class="sxs-lookup"><span data-stu-id="3b0bc-121">string</span></span>|<span data-ttu-id="3b0bc-122">グラフの線の色を表す HTML カラー コード。</span><span class="sxs-lookup"><span data-stu-id="3b0bc-122">HTML color code representing the color of lines in the chart.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3b0bc-123">関係</span><span class="sxs-lookup"><span data-stu-id="3b0bc-123">Relationships</span></span>
<span data-ttu-id="3b0bc-124">なし</span><span class="sxs-lookup"><span data-stu-id="3b0bc-124">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="3b0bc-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3b0bc-125">JSON representation</span></span>

<span data-ttu-id="3b0bc-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3b0bc-126">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.workbookChartLineFormat"
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
  "description": "ChartLineFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->