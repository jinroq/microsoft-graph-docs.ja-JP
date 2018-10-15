# <a name="planner-resource-type"></a><span data-ttu-id="65b96-101">planner リソースの種類</span><span class="sxs-lookup"><span data-stu-id="65b96-101">planner resource type</span></span>

<span data-ttu-id="65b96-p101">**planner** リソースは Planner オブジェクト モデルのエントリ ポイントです。単一の **planner** リソースを返します。使用可能なプロパティは含まれていません。</span><span class="sxs-lookup"><span data-stu-id="65b96-p101">The **planner** resource is the entry point for the Planner object model. It returns a singleton **planner** resource.  It doesn't contain any usable properties.</span></span>


## <a name="methods"></a><span data-ttu-id="65b96-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="65b96-105">Methods</span></span>

| <span data-ttu-id="65b96-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="65b96-106">Method</span></span>           | <span data-ttu-id="65b96-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="65b96-107">Return Type</span></span>    |<span data-ttu-id="65b96-108">説明</span><span class="sxs-lookup"><span data-stu-id="65b96-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="65b96-109">Create plannerBucket</span><span class="sxs-lookup"><span data-stu-id="65b96-109">Create plannerBucket</span></span>](../api/planner_post_buckets.md) |[<span data-ttu-id="65b96-110">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="65b96-110">plannerBucket</span></span>](plannerbucket.md)| <span data-ttu-id="65b96-111">バケット コレクションの投稿によって新しい **plannerBucket** を作成します。</span><span class="sxs-lookup"><span data-stu-id="65b96-111">Create a new **plannerBucket** by posting to the buckets collection.</span></span>|
|[<span data-ttu-id="65b96-112">Create plannerPlan</span><span class="sxs-lookup"><span data-stu-id="65b96-112">Create plannerPlan</span></span>](../api/planner_post_plans.md) |[<span data-ttu-id="65b96-113">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="65b96-113">plannerPlan</span></span>](plannerplan.md)| <span data-ttu-id="65b96-114">計画コレクションの投稿によって新しい **plannerPlan** を作成します。</span><span class="sxs-lookup"><span data-stu-id="65b96-114">Create a new **plannerPlan** by posting to the plans collection.</span></span>|
|[<span data-ttu-id="65b96-115">Create plannerTask</span><span class="sxs-lookup"><span data-stu-id="65b96-115">Create plannerTask</span></span>](../api/planner_post_tasks.md) |[<span data-ttu-id="65b96-116">plannerTask</span><span class="sxs-lookup"><span data-stu-id="65b96-116">plannerTask</span></span>](plannertask.md)| <span data-ttu-id="65b96-117">タスク コレクションの投稿によって新しい **plannerTask** を作成します。</span><span class="sxs-lookup"><span data-stu-id="65b96-117">Create a new **plannerTask** by posting to the tasks collection.</span></span>|

## <a name="relationships"></a><span data-ttu-id="65b96-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="65b96-118">Relationships</span></span>
| <span data-ttu-id="65b96-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="65b96-119">Relationship</span></span> | <span data-ttu-id="65b96-120">型</span><span class="sxs-lookup"><span data-stu-id="65b96-120">Type</span></span>   |<span data-ttu-id="65b96-121">説明</span><span class="sxs-lookup"><span data-stu-id="65b96-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="65b96-122">バケット</span><span class="sxs-lookup"><span data-stu-id="65b96-122">buckets</span></span>|<span data-ttu-id="65b96-123">[plannerBucket](plannerbucket.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="65b96-123">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="65b96-p102">読み取り専用です。Null 許容型。指定されたバケットのコレクションを返します</span><span class="sxs-lookup"><span data-stu-id="65b96-p102">Read-only. Nullable. Returns a collection of the specified buckets</span></span>|
|<span data-ttu-id="65b96-127">plans</span><span class="sxs-lookup"><span data-stu-id="65b96-127">plans</span></span>|<span data-ttu-id="65b96-128">[plannerPlan](plannerplan.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="65b96-128">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="65b96-p103">読み取り専用です。Null 許容型。指定された計画のコレクションを返します</span><span class="sxs-lookup"><span data-stu-id="65b96-p103">Read-only. Nullable. Returns a collection of the specified plans</span></span>|
|<span data-ttu-id="65b96-132">tasks</span><span class="sxs-lookup"><span data-stu-id="65b96-132">tasks</span></span>|<span data-ttu-id="65b96-133">[plannerTask](plannertask.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="65b96-133">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="65b96-p104">読み取り専用です。Null 許容型。指定されたタスクのコレクションを返します</span><span class="sxs-lookup"><span data-stu-id="65b96-p104">Read-only. Nullable. Returns a collection of the specified tasks</span></span>|

## <a name="json-representation"></a><span data-ttu-id="65b96-137">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="65b96-137">JSON representation</span></span>
<span data-ttu-id="65b96-138">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="65b96-138">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.planner"
}-->

```json
{
}
```

## <a name="example"></a><span data-ttu-id="65b96-139">例</span><span class="sxs-lookup"><span data-stu-id="65b96-139">Example</span></span>

<span data-ttu-id="65b96-140"> *\*プランナー** のリソースは、グラフのルートに使用できます。</span><span class="sxs-lookup"><span data-stu-id="65b96-140">The **planner** resource is available at the root of the graph.</span></span>

<!--{
  "blockType": "request"
}-->
```http
GET https://graph.microsoft.com/v1.0/planner
```

<!--{
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.planner"
}-->
```json
HTTP/1.1 200 OK
Content-type: application/json

{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "planner resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->