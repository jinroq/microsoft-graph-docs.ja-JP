# <a name="chartaxistitle-resource-type"></a><span data-ttu-id="78e11-101">ChartAxisTitle リソースの種類</span><span class="sxs-lookup"><span data-stu-id="78e11-101">ChartAxisTitle resource type</span></span>

<span data-ttu-id="78e11-102">グラフ軸のタイトルを表します。</span><span class="sxs-lookup"><span data-stu-id="78e11-102">Represents the title of a chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="78e11-103">メソッド</span><span class="sxs-lookup"><span data-stu-id="78e11-103">Methods</span></span>

| <span data-ttu-id="78e11-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="78e11-104">Method</span></span>           | <span data-ttu-id="78e11-105">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="78e11-105">Return Type</span></span>    |<span data-ttu-id="78e11-106">説明</span><span class="sxs-lookup"><span data-stu-id="78e11-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="78e11-107">Get ChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="78e11-107">Get ChartAxisTitle</span></span>](../api/chartaxistitle_get.md) | [<span data-ttu-id="78e11-108">WorkbookChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="78e11-108">WorkbookChartAxisTitle</span></span>](chartaxistitle.md) |<span data-ttu-id="78e11-109">chartAxisTitle オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="78e11-109">Read properties and relationships of chartAxisTitle object.</span></span>|
|[<span data-ttu-id="78e11-110">Update</span><span class="sxs-lookup"><span data-stu-id="78e11-110">Update</span></span>](../api/chartaxistitle_update.md) | [<span data-ttu-id="78e11-111">WorkbookChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="78e11-111">WorkbookChartAxisTitle</span></span>](chartaxistitle.md)    |<span data-ttu-id="78e11-112">ChartAxisTitle オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="78e11-112">Update ChartAxisTitle object.</span></span> |

## <a name="properties"></a><span data-ttu-id="78e11-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="78e11-113">Properties</span></span>
| <span data-ttu-id="78e11-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="78e11-114">Property</span></span>     | <span data-ttu-id="78e11-115">タイプ</span><span class="sxs-lookup"><span data-stu-id="78e11-115">Type</span></span>   |<span data-ttu-id="78e11-116">説明</span><span class="sxs-lookup"><span data-stu-id="78e11-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="78e11-117">text</span><span class="sxs-lookup"><span data-stu-id="78e11-117">text</span></span>|<span data-ttu-id="78e11-118">文字列</span><span class="sxs-lookup"><span data-stu-id="78e11-118">string</span></span>|<span data-ttu-id="78e11-119">軸タイトルを表します。</span><span class="sxs-lookup"><span data-stu-id="78e11-119">Represents the axis title.</span></span>|
|<span data-ttu-id="78e11-120">visible</span><span class="sxs-lookup"><span data-stu-id="78e11-120">visible</span></span>|<span data-ttu-id="78e11-121">ブール値</span><span class="sxs-lookup"><span data-stu-id="78e11-121">boolean</span></span>|<span data-ttu-id="78e11-122">軸のタイトルの表示/非表示を指定するブール型の値です。</span><span class="sxs-lookup"><span data-stu-id="78e11-122">A boolean that specifies the visibility of an axis title.</span></span>|

## <a name="relationships"></a><span data-ttu-id="78e11-123">関係</span><span class="sxs-lookup"><span data-stu-id="78e11-123">Relationships</span></span>
| <span data-ttu-id="78e11-124">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="78e11-124">Relationship</span></span> | <span data-ttu-id="78e11-125">型</span><span class="sxs-lookup"><span data-stu-id="78e11-125">Type</span></span>   |<span data-ttu-id="78e11-126">説明</span><span class="sxs-lookup"><span data-stu-id="78e11-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="78e11-127">format</span><span class="sxs-lookup"><span data-stu-id="78e11-127">format</span></span>|[<span data-ttu-id="78e11-128">WorkbookChartAxisTitleFormat</span><span class="sxs-lookup"><span data-stu-id="78e11-128">WorkbookChartAxisTitleFormat</span></span>](chartaxistitleformat.md)|<span data-ttu-id="78e11-p101">グラフ軸のタイトルの書式設定を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="78e11-p101">Represents the formatting of chart axis title. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="78e11-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="78e11-131">JSON representation</span></span>

<span data-ttu-id="78e11-132">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="78e11-132">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.workbookChartAxisTitle"
}-->

```json
{
  "text": "string",
  "visible": true,
  "format": {"@odata.type":"microsoft.graph.workbookChartAxisTitleFormat"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartAxisTitle resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->