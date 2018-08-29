# <a name="planneruser-resource-type"></a><span data-ttu-id="2e35a-101">plannerUser リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2e35a-101">plannerUser resource type</span></span>

<span data-ttu-id="2e35a-p101">**plannerUser** リソースは、[user](user.md) のプランナー リソースへのアクセスを提供します。使用可能なプロパティは含まれていません。</span><span class="sxs-lookup"><span data-stu-id="2e35a-p101">The **plannerUser** resource provide access to Planner resources for a [user](user.md). It doesn't contain any usable properties.</span></span>


## <a name="methods"></a><span data-ttu-id="2e35a-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="2e35a-104">Methods</span></span>

| <span data-ttu-id="2e35a-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="2e35a-105">Method</span></span>           | <span data-ttu-id="2e35a-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="2e35a-106">Return Type</span></span>    |<span data-ttu-id="2e35a-107">説明</span><span class="sxs-lookup"><span data-stu-id="2e35a-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2e35a-108">plans を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="2e35a-108">List plans</span></span>](../api/planneruser_list_plans.md) |<span data-ttu-id="2e35a-109">[plannerPlan](plannerplan.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="2e35a-109">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="2e35a-110">**plannerPlan** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="2e35a-110">Get a **plannerPlan** object collection.</span></span>|
|[<span data-ttu-id="2e35a-111">Tasks を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="2e35a-111">List tasks</span></span>](../api/planneruser_list_tasks.md) |<span data-ttu-id="2e35a-112">[plannerTask](plannertask.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="2e35a-112">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="2e35a-113">**plannerTask** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="2e35a-113">Get a **plannerTask** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="2e35a-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2e35a-114">Properties</span></span>
| <span data-ttu-id="2e35a-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2e35a-115">Property</span></span>     | <span data-ttu-id="2e35a-116">タイプ</span><span class="sxs-lookup"><span data-stu-id="2e35a-116">Type</span></span>   |<span data-ttu-id="2e35a-117">説明</span><span class="sxs-lookup"><span data-stu-id="2e35a-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2e35a-118">id</span><span class="sxs-lookup"><span data-stu-id="2e35a-118">id</span></span>|<span data-ttu-id="2e35a-119">文字列</span><span class="sxs-lookup"><span data-stu-id="2e35a-119">String</span></span>| <span data-ttu-id="2e35a-p102">読み取り専用です。planenrUser の識別子</span><span class="sxs-lookup"><span data-stu-id="2e35a-p102">Read-only. Identifier of the planenrUser</span></span>|

## <a name="relationships"></a><span data-ttu-id="2e35a-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2e35a-122">Relationships</span></span>
| <span data-ttu-id="2e35a-123">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2e35a-123">Relationship</span></span> | <span data-ttu-id="2e35a-124">型</span><span class="sxs-lookup"><span data-stu-id="2e35a-124">Type</span></span>   |<span data-ttu-id="2e35a-125">説明</span><span class="sxs-lookup"><span data-stu-id="2e35a-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2e35a-126">plans</span><span class="sxs-lookup"><span data-stu-id="2e35a-126">plans</span></span>|<span data-ttu-id="2e35a-127">[plannerPlan](plannerplan.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="2e35a-127">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="2e35a-p103">読み取り専用です。Null 許容型。ユーザーに割り当てられている [plannerTasks](plannertask.md) を返します。</span><span class="sxs-lookup"><span data-stu-id="2e35a-p103">Read-only. Nullable. Returns the [plannerTasks](plannertask.md) assigned to the user.</span></span>|
|<span data-ttu-id="2e35a-131">tasks</span><span class="sxs-lookup"><span data-stu-id="2e35a-131">tasks</span></span>|<span data-ttu-id="2e35a-132">[plannerTask](plannertask.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="2e35a-132">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="2e35a-p104">読み取り専用です。Null 許容型。ユーザーと共有している [plannerPlans](plannerplan.md) を返します。</span><span class="sxs-lookup"><span data-stu-id="2e35a-p104">Read-only. Nullable. Returns the [plannerPlans](plannerplan.md) shared with the user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2e35a-136">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2e35a-136">JSON representation</span></span>
<span data-ttu-id="2e35a-137">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2e35a-137">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerUser"
}-->

```json
{
  "id": "String (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->