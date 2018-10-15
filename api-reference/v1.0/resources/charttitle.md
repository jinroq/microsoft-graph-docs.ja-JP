# <a name="charttitle-resource-type"></a><span data-ttu-id="80bbd-101">ChartTitle リソースの種類</span><span class="sxs-lookup"><span data-stu-id="80bbd-101">ChartTitle resource type</span></span>

<span data-ttu-id="80bbd-102">グラフのグラフ タイトル オブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="80bbd-102">Represents a chart title object of a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="80bbd-103">メソッド</span><span class="sxs-lookup"><span data-stu-id="80bbd-103">Methods</span></span>

| <span data-ttu-id="80bbd-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="80bbd-104">Method</span></span>           | <span data-ttu-id="80bbd-105">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="80bbd-105">Return Type</span></span>    |<span data-ttu-id="80bbd-106">説明</span><span class="sxs-lookup"><span data-stu-id="80bbd-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="80bbd-107">ChartTitle を取得する</span><span class="sxs-lookup"><span data-stu-id="80bbd-107">Get ChartTitle</span></span>](../api/charttitle_get.md) | [<span data-ttu-id="80bbd-108">WorkbookChartTitle</span><span class="sxs-lookup"><span data-stu-id="80bbd-108">WorkbookChartTitle</span></span>](charttitle.md) |<span data-ttu-id="80bbd-109">chartTitle オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="80bbd-109">Read properties and relationships of chartTitle object.</span></span>|
|[<span data-ttu-id="80bbd-110">更新する</span><span class="sxs-lookup"><span data-stu-id="80bbd-110">Update</span></span>](../api/charttitle_update.md) | [<span data-ttu-id="80bbd-111">WorkbookChartTitle</span><span class="sxs-lookup"><span data-stu-id="80bbd-111">WorkbookChartTitle</span></span>](charttitle.md)    |<span data-ttu-id="80bbd-112">ChartTitle オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="80bbd-112">Update ChartTitle object.</span></span> |

## <a name="properties"></a><span data-ttu-id="80bbd-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="80bbd-113">Properties</span></span>
| <span data-ttu-id="80bbd-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="80bbd-114">Property</span></span>     | <span data-ttu-id="80bbd-115">タイプ</span><span class="sxs-lookup"><span data-stu-id="80bbd-115">Type</span></span>   |<span data-ttu-id="80bbd-116">説明</span><span class="sxs-lookup"><span data-stu-id="80bbd-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="80bbd-117">overlay</span><span class="sxs-lookup"><span data-stu-id="80bbd-117">overlay</span></span>|<span data-ttu-id="80bbd-118">ブール値</span><span class="sxs-lookup"><span data-stu-id="80bbd-118">boolean</span></span>|<span data-ttu-id="80bbd-119">グラフのタイトルをグラフに重ねるかどうかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="80bbd-119">Boolean value representing if the chart title will overlay the chart or not.</span></span>|
|<span data-ttu-id="80bbd-120">テキスト</span><span class="sxs-lookup"><span data-stu-id="80bbd-120">text</span></span>|<span data-ttu-id="80bbd-121">文字列</span><span class="sxs-lookup"><span data-stu-id="80bbd-121">string</span></span>|<span data-ttu-id="80bbd-122">グラフのタイトルのテキストを表します。</span><span class="sxs-lookup"><span data-stu-id="80bbd-122">Represents the title text of a chart.</span></span>|
|<span data-ttu-id="80bbd-123">目に見える</span><span class="sxs-lookup"><span data-stu-id="80bbd-123">visible</span></span>|<span data-ttu-id="80bbd-124">ブール値</span><span class="sxs-lookup"><span data-stu-id="80bbd-124">boolean</span></span>|<span data-ttu-id="80bbd-125">ChartTitle オブジェクトを表示または非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="80bbd-125">A boolean value the represents the visibility of a chart title object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="80bbd-126">関係</span><span class="sxs-lookup"><span data-stu-id="80bbd-126">Relationships</span></span>
| <span data-ttu-id="80bbd-127">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="80bbd-127">Relationship</span></span> | <span data-ttu-id="80bbd-128">型</span><span class="sxs-lookup"><span data-stu-id="80bbd-128">Type</span></span>   |<span data-ttu-id="80bbd-129">説明</span><span class="sxs-lookup"><span data-stu-id="80bbd-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="80bbd-130">format</span><span class="sxs-lookup"><span data-stu-id="80bbd-130">format</span></span>|[<span data-ttu-id="80bbd-131">WorkbookChartTitleFormat</span><span class="sxs-lookup"><span data-stu-id="80bbd-131">WorkbookChartTitleFormat</span></span>](charttitleformat.md)|<span data-ttu-id="80bbd-p101">グラフ のタイトルの書式設定を表します。これには塗りつぶしとフォントの書式設定などがあります。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="80bbd-p101">Represents the formatting of a chart title, which includes fill and font formatting. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="80bbd-134">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="80bbd-134">JSON representation</span></span>

<span data-ttu-id="80bbd-135">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="80bbd-135">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookChartTitle"
}-->

```json
{
  "overlay": true,
  "text": "string",
  "visible": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartTitle resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->