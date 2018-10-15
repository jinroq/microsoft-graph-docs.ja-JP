# <a name="chartaxis-resource-type"></a><span data-ttu-id="3899d-101">ChartAxis リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3899d-101">ChartAxis resource type</span></span>

<span data-ttu-id="3899d-102">グラフの 1 つの軸を表します。</span><span class="sxs-lookup"><span data-stu-id="3899d-102">Represents a single axis in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="3899d-103">メソッド</span><span class="sxs-lookup"><span data-stu-id="3899d-103">Methods</span></span>

| <span data-ttu-id="3899d-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="3899d-104">Method</span></span>           | <span data-ttu-id="3899d-105">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="3899d-105">Return Type</span></span>    |<span data-ttu-id="3899d-106">説明</span><span class="sxs-lookup"><span data-stu-id="3899d-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3899d-107">Get ChartAxis</span><span class="sxs-lookup"><span data-stu-id="3899d-107">Get ChartAxis</span></span>](../api/chartaxis_get.md) | [<span data-ttu-id="3899d-108">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="3899d-108">WorkbookChartAxis</span></span>](chartaxis.md) |<span data-ttu-id="3899d-109">chartAxis オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="3899d-109">Read properties and relationships of chartAxis object.</span></span>|
|[<span data-ttu-id="3899d-110">Update</span><span class="sxs-lookup"><span data-stu-id="3899d-110">Update</span></span>](../api/chartaxis_update.md) | [<span data-ttu-id="3899d-111">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="3899d-111">WorkbookChartAxis</span></span>](chartaxis.md)   |<span data-ttu-id="3899d-112">ChartAxis オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="3899d-112">Update ChartAxis object.</span></span> |

## <a name="properties"></a><span data-ttu-id="3899d-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3899d-113">Properties</span></span>
| <span data-ttu-id="3899d-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3899d-114">Property</span></span>     | <span data-ttu-id="3899d-115">タイプ</span><span class="sxs-lookup"><span data-stu-id="3899d-115">Type</span></span>   |<span data-ttu-id="3899d-116">説明</span><span class="sxs-lookup"><span data-stu-id="3899d-116">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3899d-117">ID</span><span class="sxs-lookup"><span data-stu-id="3899d-117">id</span></span>       |<span data-ttu-id="3899d-118">文字列</span><span class="sxs-lookup"><span data-stu-id="3899d-118">string</span></span>   | <span data-ttu-id="3899d-119">一意の識別子</span><span class="sxs-lookup"><span data-stu-id="3899d-119">Unique Identifier</span></span> <span data-ttu-id="3899d-120">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="3899d-120">Read-only.</span></span>|
|<span data-ttu-id="3899d-121">majorUnit</span><span class="sxs-lookup"><span data-stu-id="3899d-121">majorUnit</span></span>|<span data-ttu-id="3899d-122">Json</span><span class="sxs-lookup"><span data-stu-id="3899d-122">Json</span></span>|<span data-ttu-id="3899d-p102">2 つの大きい目盛の間隔を表します。数値の値または空の文字列を設定できます。戻り値は常に数値です。</span><span class="sxs-lookup"><span data-stu-id="3899d-p102">Represents the interval between two major tick marks. Can be set to a numeric value or an empty string.  The returned value is always a number.</span></span>|
|<span data-ttu-id="3899d-126">maximum</span><span class="sxs-lookup"><span data-stu-id="3899d-126">maximum</span></span>|<span data-ttu-id="3899d-127">Json</span><span class="sxs-lookup"><span data-stu-id="3899d-127">Json</span></span>|<span data-ttu-id="3899d-p103">数値軸の最大値を表します。数値の値または空の文字列を設定できます (軸の値が自動の場合)。戻り値は常に数値です。</span><span class="sxs-lookup"><span data-stu-id="3899d-p103">Represents the maximum value on the value axis.  Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="3899d-131">minimum</span><span class="sxs-lookup"><span data-stu-id="3899d-131">minimum</span></span>|<span data-ttu-id="3899d-132">Json</span><span class="sxs-lookup"><span data-stu-id="3899d-132">Json</span></span>|<span data-ttu-id="3899d-p104">数値軸の最小値を表します。数値の値または空の文字列を設定できます (軸の値が自動の場合)。戻り値は常に数値です。</span><span class="sxs-lookup"><span data-stu-id="3899d-p104">Represents the minimum value on the value axis. Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="3899d-136">minorUnit</span><span class="sxs-lookup"><span data-stu-id="3899d-136">minorUnit</span></span>|<span data-ttu-id="3899d-137">Json</span><span class="sxs-lookup"><span data-stu-id="3899d-137">Json</span></span>|<span data-ttu-id="3899d-p105">2 つの小さい目盛の間隔を表します。"数値の値または空の文字列を設定できます (軸の値が自動の場合)。戻り値は常に数値です。</span><span class="sxs-lookup"><span data-stu-id="3899d-p105">Represents the interval between two minor tick marks. "Can be set to a numeric value or an empty string (for automatic axis values). The returned value is always a number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3899d-141">関係</span><span class="sxs-lookup"><span data-stu-id="3899d-141">Relationships</span></span>
| <span data-ttu-id="3899d-142">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="3899d-142">Relationship</span></span> | <span data-ttu-id="3899d-143">型</span><span class="sxs-lookup"><span data-stu-id="3899d-143">Type</span></span>   |<span data-ttu-id="3899d-144">説明</span><span class="sxs-lookup"><span data-stu-id="3899d-144">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3899d-145">format</span><span class="sxs-lookup"><span data-stu-id="3899d-145">format</span></span>|[<span data-ttu-id="3899d-146">WorkbookChartAxisFormat</span><span class="sxs-lookup"><span data-stu-id="3899d-146">WorkbookChartAxisFormat</span></span>](chartaxisformat.md)|<span data-ttu-id="3899d-p106">グラフ オブジェクトの書式設定を表します。これには線とフォントの書式設定などがあります。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="3899d-p106">Represents the formatting of a chart object, which includes line and font formatting. Read-only.</span></span>|
|<span data-ttu-id="3899d-149">majorGridlines</span><span class="sxs-lookup"><span data-stu-id="3899d-149">majorGridlines</span></span>|[<span data-ttu-id="3899d-150">WorkbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="3899d-150">WorkbookChartGridlines</span></span>](chartgridlines.md)|<span data-ttu-id="3899d-p107">指定された軸の目盛線を表す gridlines オブジェクトを返します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="3899d-p107">Returns a gridlines object that represents the major gridlines for the specified axis. Read-only.</span></span>|
|<span data-ttu-id="3899d-153">minorGridlines</span><span class="sxs-lookup"><span data-stu-id="3899d-153">minorGridlines</span></span>|[<span data-ttu-id="3899d-154">WorkbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="3899d-154">WorkbookChartGridlines</span></span>](chartgridlines.md)|<span data-ttu-id="3899d-p108">指定された軸の小さい目盛線を表す gridlines オブジェクトを返します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="3899d-p108">Returns a Gridlines object that represents the minor gridlines for the specified axis. Read-only.</span></span>|
|<span data-ttu-id="3899d-157">title</span><span class="sxs-lookup"><span data-stu-id="3899d-157">title</span></span>|[<span data-ttu-id="3899d-158">WorkbookChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="3899d-158">WorkbookChartAxisTitle</span></span>](chartaxistitle.md)|<span data-ttu-id="3899d-p109">軸タイトルを表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="3899d-p109">Represents the axis title. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3899d-161">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3899d-161">JSON representation</span></span>

<span data-ttu-id="3899d-162">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3899d-162">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartAxis"
}-->

```json
{
  "id": "string",
  "majorUnit": "string",
  "maximum": "string",
  "minimum": "string",
  "minorUnit": "string",
   "format": {"@odata.type": "microsoft.graph.workbookChartAxisFormat"},
  "majorGridlines": {"@odata.type": "microsoft.graph.workbookChartGridlines"},
  "minorGridlines": {"@odata.type": "microsoft.graph.workbookChartGridlines"},
  "title": {"@odata.type": "microsoft.graph.workbookChartAxisTitle"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartAxis resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->