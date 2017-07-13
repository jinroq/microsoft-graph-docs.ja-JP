<span data-ttu-id="c251c-p101">**PlannerCategoryDescriptions** リソースは、計画に定義されているカテゴリを説明するラベルを表します。これは、[計画の詳細](plannerplandetails.md)オブジェクトに含まれています。最大 6 つのカテゴリを定義できます。</span><span class="sxs-lookup"><span data-stu-id="c251c-p101">The **plannerCategoryDescriptions** resource represents the descriptive labels for the categories that have been defined for a plan. It belongs to the [plan details](plannerplandetails.md) object. There can be up to 6 categories defined.</span></span>

**PlannerCategoryDescriptions** リソースは、計画に定義されているカテゴリを説明するラベルを表します。これは、[計画の詳細](plannerplandetails.md)オブジェクトに含まれています。最大 6 つのカテゴリを定義できます。 


## <span data-ttu-id="c251c-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c251c-105">Properties</span></span>
<a id="properties" class="xliff"></a>
| <span data-ttu-id="c251c-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c251c-106">Property</span></span>     | <span data-ttu-id="c251c-107">型</span><span class="sxs-lookup"><span data-stu-id="c251c-107">Type</span></span>   |<span data-ttu-id="c251c-108">説明</span><span class="sxs-lookup"><span data-stu-id="c251c-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c251c-109">category1</span><span class="sxs-lookup"><span data-stu-id="c251c-109">category1</span></span>|<span data-ttu-id="c251c-110">String</span><span class="sxs-lookup"><span data-stu-id="c251c-110">String</span></span>|<span data-ttu-id="c251c-111">Category 1 に関連付けられているラベル</span><span class="sxs-lookup"><span data-stu-id="c251c-111">The label associated with Category 1</span></span>|
|<span data-ttu-id="c251c-112">category2</span><span class="sxs-lookup"><span data-stu-id="c251c-112">category2</span></span>|<span data-ttu-id="c251c-113">String</span><span class="sxs-lookup"><span data-stu-id="c251c-113">String</span></span>|<span data-ttu-id="c251c-114">Category 2 に関連付けられているラベル</span><span class="sxs-lookup"><span data-stu-id="c251c-114">The label associated with Category 2</span></span>|
|<span data-ttu-id="c251c-115">category3</span><span class="sxs-lookup"><span data-stu-id="c251c-115">category3</span></span>|<span data-ttu-id="c251c-116">String</span><span class="sxs-lookup"><span data-stu-id="c251c-116">String</span></span>|<span data-ttu-id="c251c-117">Category 3 に関連付けられているラベル</span><span class="sxs-lookup"><span data-stu-id="c251c-117">The label associated with Category 3</span></span>|
|<span data-ttu-id="c251c-118">category4</span><span class="sxs-lookup"><span data-stu-id="c251c-118">category4</span></span>|<span data-ttu-id="c251c-119">String</span><span class="sxs-lookup"><span data-stu-id="c251c-119">String</span></span>|<span data-ttu-id="c251c-120">Category 4 に関連付けられているラベル</span><span class="sxs-lookup"><span data-stu-id="c251c-120">The label associated with Category 4</span></span>|
|<span data-ttu-id="c251c-121">category5</span><span class="sxs-lookup"><span data-stu-id="c251c-121">category5</span></span>|<span data-ttu-id="c251c-122">String</span><span class="sxs-lookup"><span data-stu-id="c251c-122">String</span></span>|<span data-ttu-id="c251c-123">Category 5 に関連付けられているラベル</span><span class="sxs-lookup"><span data-stu-id="c251c-123">The label associated with Category 5</span></span>|
|<span data-ttu-id="c251c-124">category6</span><span class="sxs-lookup"><span data-stu-id="c251c-124">category6</span></span>|<span data-ttu-id="c251c-125">String</span><span class="sxs-lookup"><span data-stu-id="c251c-125">String</span></span>|<span data-ttu-id="c251c-126">Category 6 に関連付けられているラベル</span><span class="sxs-lookup"><span data-stu-id="c251c-126">The label associated with Category 6</span></span>|

## <span data-ttu-id="c251c-127">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c251c-127">JSON representation</span></span>
<a id="json-representation" class="xliff"></a>
<span data-ttu-id="c251c-128">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c251c-128">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerCategoryDescriptions"
}-->

```json
{
  "category1": "String",
  "category2": "String",
  "category3": "String",
  "category4": "String",
  "category5": "String",
  "category6": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerCategoryDescriptions resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->