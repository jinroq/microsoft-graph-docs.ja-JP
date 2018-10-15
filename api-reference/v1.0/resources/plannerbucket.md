# <a name="plannerbucket-resource-type"></a><span data-ttu-id="7cf68-101">plannerBucket リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7cf68-101">plannerBucket resource type</span></span>

<span data-ttu-id="7cf68-p101">**PlannerBucket** リソースは、Office 365 の計画におけるタスクのバケット (または "カスタム列") を表します。これは [plannerPlan](plannerPlan.md) に含まれており、[plannerTasks](plannerTask.md) のコレクションを持ちます。</span><span class="sxs-lookup"><span data-stu-id="7cf68-p101">The **plannerBucket** resource represents a bucket (or "custom column") for tasks in a plan in Office 365. It is contained in a [plannerPlan](plannerPlan.md) and can have a collection of [plannerTasks](plannerTask.md).</span></span>



## <a name="methods"></a><span data-ttu-id="7cf68-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="7cf68-104">Methods</span></span>

| <span data-ttu-id="7cf68-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="7cf68-105">Method</span></span>           | <span data-ttu-id="7cf68-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="7cf68-106">Return Type</span></span>    |<span data-ttu-id="7cf68-107">説明</span><span class="sxs-lookup"><span data-stu-id="7cf68-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7cf68-108">plannerBucket の取得</span><span class="sxs-lookup"><span data-stu-id="7cf68-108">Get plannerBucket</span></span>](../api/plannerbucket_get.md) | [<span data-ttu-id="7cf68-109">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="7cf68-109">plannerBucket</span></span>](plannerbucket.md) |<span data-ttu-id="7cf68-110">**plannerBucket** オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="7cf68-110">Read properties and relationships of **plannerBucket** object.</span></span>|
|[<span data-ttu-id="7cf68-111">plannerTasks のリスト</span><span class="sxs-lookup"><span data-stu-id="7cf68-111">List plannerTasks</span></span>](../api/plannerbucket_list_tasks.md) |<span data-ttu-id="7cf68-112">[plannerTask](plannertask.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="7cf68-112">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="7cf68-113">**plannerTask** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="7cf68-113">Get a **plannerTask** object collection.</span></span>|
|[<span data-ttu-id="7cf68-114">作成</span><span class="sxs-lookup"><span data-stu-id="7cf68-114">Create</span></span>](../api/planner_post_buckets.md) | [<span data-ttu-id="7cf68-115">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="7cf68-115">plannerBucket</span></span>](plannerbucket.md)   | <span data-ttu-id="7cf68-116">新しい **plannerBucket** オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="7cf68-116">Create a new **plannerBucket** object.</span></span> |
|[<span data-ttu-id="7cf68-117">更新</span><span class="sxs-lookup"><span data-stu-id="7cf68-117">Update</span></span>](../api/plannerbucket_update.md) | [<span data-ttu-id="7cf68-118">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="7cf68-118">plannerBucket</span></span>](plannerbucket.md)   |<span data-ttu-id="7cf68-119">**plannerBucket** オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="7cf68-119">Update **plannerBucket** object.</span></span> |
|[<span data-ttu-id="7cf68-120">削除</span><span class="sxs-lookup"><span data-stu-id="7cf68-120">Delete</span></span>](../api/plannerbucket_delete.md) | <span data-ttu-id="7cf68-121">なし</span><span class="sxs-lookup"><span data-stu-id="7cf68-121">None</span></span> |<span data-ttu-id="7cf68-122">**plannerBucket** オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="7cf68-122">Delete **plannerBucket** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="7cf68-123">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7cf68-123">Properties</span></span>
| <span data-ttu-id="7cf68-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7cf68-124">Property</span></span>     | <span data-ttu-id="7cf68-125">タイプ</span><span class="sxs-lookup"><span data-stu-id="7cf68-125">Type</span></span>   |<span data-ttu-id="7cf68-126">説明</span><span class="sxs-lookup"><span data-stu-id="7cf68-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7cf68-127">id</span><span class="sxs-lookup"><span data-stu-id="7cf68-127">id</span></span>|<span data-ttu-id="7cf68-128">文字列</span><span class="sxs-lookup"><span data-stu-id="7cf68-128">String</span></span>| <span data-ttu-id="7cf68-129">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="7cf68-129">Read-only.</span></span> <span data-ttu-id="7cf68-130">バケットの ID です。</span><span class="sxs-lookup"><span data-stu-id="7cf68-130">Name of the bucket.</span></span> <span data-ttu-id="7cf68-131">28 文字で大文字小文字を区別します。</span><span class="sxs-lookup"><span data-stu-id="7cf68-131">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="7cf68-132">サービスの[フォーマットの検証](planner_identifiers_disclaimer.md) が行われます。</span><span class="sxs-lookup"><span data-stu-id="7cf68-132">[Format validation](planner_identifiers_disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="7cf68-133">name</span><span class="sxs-lookup"><span data-stu-id="7cf68-133">name</span></span>|<span data-ttu-id="7cf68-134">文字列</span><span class="sxs-lookup"><span data-stu-id="7cf68-134">String</span></span>|<span data-ttu-id="7cf68-135">バケットの名前。</span><span class="sxs-lookup"><span data-stu-id="7cf68-135">Name of the bucket.</span></span>|
|<span data-ttu-id="7cf68-136">orderHint</span><span class="sxs-lookup"><span data-stu-id="7cf68-136">orderHint</span></span>|<span data-ttu-id="7cf68-137">文字列</span><span class="sxs-lookup"><span data-stu-id="7cf68-137">String</span></span>|<span data-ttu-id="7cf68-p103">リスト ビューでこの種類の項目の順序付けに使用するヒント。形式は[ここ](planner_order_hint_format.md)の説明に従って定義されます。</span><span class="sxs-lookup"><span data-stu-id="7cf68-p103">Hint used to order items of this type in a list view. The format is defined as outlined [here](planner_order_hint_format.md).</span></span>|
|<span data-ttu-id="7cf68-140">planId</span><span class="sxs-lookup"><span data-stu-id="7cf68-140">planId</span></span>|<span data-ttu-id="7cf68-141">文字列</span><span class="sxs-lookup"><span data-stu-id="7cf68-141">String</span></span>|<span data-ttu-id="7cf68-142">バケットが所属する計画の ID。</span><span class="sxs-lookup"><span data-stu-id="7cf68-142">Plan ID to which the bucket belongs.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7cf68-143">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7cf68-143">Relationships</span></span>
| <span data-ttu-id="7cf68-144">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7cf68-144">Relationship</span></span> | <span data-ttu-id="7cf68-145">型</span><span class="sxs-lookup"><span data-stu-id="7cf68-145">Type</span></span>   |<span data-ttu-id="7cf68-146">説明</span><span class="sxs-lookup"><span data-stu-id="7cf68-146">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7cf68-147">tasks</span><span class="sxs-lookup"><span data-stu-id="7cf68-147">tasks</span></span>|<span data-ttu-id="7cf68-148">[plannerTask](plannertask.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="7cf68-148">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="7cf68-p104">読み取り専用です。Null 許容型。バケットに含まれるタスクのコレクション。</span><span class="sxs-lookup"><span data-stu-id="7cf68-p104">Read-only. Nullable. The collection of tasks in the bucket.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7cf68-152">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7cf68-152">JSON representation</span></span>
<span data-ttu-id="7cf68-153">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7cf68-153">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerBucket"
}-->

```json
{
  "id": "String (identifier)",
  "name": "String",
  "orderHint": "String",
  "planId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerBucket resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->