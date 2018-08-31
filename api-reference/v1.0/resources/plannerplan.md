# <a name="plannerplan-resource-type"></a><span data-ttu-id="a1ee4-101">plannerPlan リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a1ee4-101">plannerPlan resource type</span></span>

<span data-ttu-id="a1ee4-p101">**plannerPlan** リソースは、Office 365 での計画を表します。計画は [group](group.md) によって所有され、[plannerTasks](plannerTask.md) のコレクションが含まれています。[plannerBuckets](plannerBucket.md) のコレクションを含む場合もあります。各計画オブジェクトには [details](plannerPlanDetails.md) オブジェクトがあり、計画に関する詳細情報が含まれていることがあります。グループ、計画、タスク間のリレーションシップの詳細については、「[Planner](planner_overview.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a1ee4-p101">The **plannerPlan** resource represents a plan in Office 365. A plan can be owned by a [group](group.md) and contains a collection of [plannerTasks](plannerTask.md). It can also have a collection of [plannerBuckets](plannerBucket.md). Each plan object has a [details](plannerPlanDetails.md) object that can contain more information about the plan. For more information about the relationships between groups, plans, and tasks, see [Planner](planner_overview.md).</span></span>

## <a name="methods"></a><span data-ttu-id="a1ee4-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="a1ee4-107">Methods</span></span>

| <span data-ttu-id="a1ee4-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="a1ee4-108">Method</span></span>           | <span data-ttu-id="a1ee4-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="a1ee4-109">Return Type</span></span>    |<span data-ttu-id="a1ee4-110">説明</span><span class="sxs-lookup"><span data-stu-id="a1ee4-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a1ee4-111">Get plannerPlan</span><span class="sxs-lookup"><span data-stu-id="a1ee4-111">Get plannerPlan</span></span>](../api/plannerplan_get.md) | [<span data-ttu-id="a1ee4-112">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="a1ee4-112">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="a1ee4-113">**plannerPlan** オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="a1ee4-113">Read properties and relationships of **plannerPlan** object.</span></span>|
|[<span data-ttu-id="a1ee4-114">List buckets</span><span class="sxs-lookup"><span data-stu-id="a1ee4-114">List buckets</span></span>](../api/plannerplan_list_buckets.md) |<span data-ttu-id="a1ee4-115">[plannerBucket](plannerbucket.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a1ee4-115">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="a1ee4-116">**plannerBucket** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="a1ee4-116">Get a **plannerBucket** object collection.</span></span>|
|[<span data-ttu-id="a1ee4-117">Tasks を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="a1ee4-117">List tasks</span></span>](../api/plannerplan_list_tasks.md) |<span data-ttu-id="a1ee4-118">[plannerTask](plannertask.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a1ee4-118">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="a1ee4-119">**plannerTask** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="a1ee4-119">Get a **plannerTask** object collection.</span></span>|
|[<span data-ttu-id="a1ee4-120">更新する</span><span class="sxs-lookup"><span data-stu-id="a1ee4-120">Update</span></span>](../api/plannerplan_update.md) | [<span data-ttu-id="a1ee4-121">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="a1ee4-121">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="a1ee4-122">**plannerPlan** オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="a1ee4-122">Update **plannerPlan** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="a1ee4-123">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a1ee4-123">Properties</span></span>
| <span data-ttu-id="a1ee4-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a1ee4-124">Property</span></span>     | <span data-ttu-id="a1ee4-125">タイプ</span><span class="sxs-lookup"><span data-stu-id="a1ee4-125">Type</span></span>   |<span data-ttu-id="a1ee4-126">説明</span><span class="sxs-lookup"><span data-stu-id="a1ee4-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a1ee4-127">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a1ee4-127">createdDateTime</span></span>|<span data-ttu-id="a1ee4-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1ee4-128">DateTimeOffset</span></span>|<span data-ttu-id="a1ee4-p102">読み取り専用。計画の作成日時。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。 `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="a1ee4-p102">Read-only. Date and time at which the plan is created. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="a1ee4-133">ID</span><span class="sxs-lookup"><span data-stu-id="a1ee4-133">id</span></span>|<span data-ttu-id="a1ee4-134">文字列</span><span class="sxs-lookup"><span data-stu-id="a1ee4-134">String</span></span>| <span data-ttu-id="a1ee4-135">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="a1ee4-135">Read-only.</span></span> <span data-ttu-id="a1ee4-136">計画の ID です。</span><span class="sxs-lookup"><span data-stu-id="a1ee4-136">Title of the plan.</span></span> <span data-ttu-id="a1ee4-137">28 文字で大文字小文字を区別します。</span><span class="sxs-lookup"><span data-stu-id="a1ee4-137">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="a1ee4-138">サービスの[フォーマットの検証](planner_identifiers_disclaimer.md) が行われます。</span><span class="sxs-lookup"><span data-stu-id="a1ee4-138">[Format validation](planner_identifiers_disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="a1ee4-139">所有者</span><span class="sxs-lookup"><span data-stu-id="a1ee4-139">owner</span></span>|<span data-ttu-id="a1ee4-140">文字列</span><span class="sxs-lookup"><span data-stu-id="a1ee4-140">String</span></span>|<span data-ttu-id="a1ee4-p104">計画を所有している [Group](group.md) の ID。このフィールドを設定するためには、有効なグループが存在していなければなりません。一度設定したら、所有者のみが更新できます。</span><span class="sxs-lookup"><span data-stu-id="a1ee4-p104">ID of the [Group](group.md) that owns the plan. A valid group must exist before this field can be set. Once set, this can only be updated by the owner.</span></span>|
|<span data-ttu-id="a1ee4-144">タイトル</span><span class="sxs-lookup"><span data-stu-id="a1ee4-144">title</span></span>|<span data-ttu-id="a1ee4-145">文字列</span><span class="sxs-lookup"><span data-stu-id="a1ee4-145">String</span></span>|<span data-ttu-id="a1ee4-p105">必須。計画のタイトル。</span><span class="sxs-lookup"><span data-stu-id="a1ee4-p105">Required. Title of the plan.</span></span>|
|<span data-ttu-id="a1ee4-148">createdBy</span><span class="sxs-lookup"><span data-stu-id="a1ee4-148">createdBy</span></span>|[<span data-ttu-id="a1ee4-149">identitySet</span><span class="sxs-lookup"><span data-stu-id="a1ee4-149">identitySet</span></span>](identityset.md)|<span data-ttu-id="a1ee4-p106">読み取り専用です。計画を作成したユーザー。</span><span class="sxs-lookup"><span data-stu-id="a1ee4-p106">Read-only. The user who created the plan.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a1ee4-152">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a1ee4-152">Relationships</span></span>
| <span data-ttu-id="a1ee4-153">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a1ee4-153">Relationship</span></span> | <span data-ttu-id="a1ee4-154">型</span><span class="sxs-lookup"><span data-stu-id="a1ee4-154">Type</span></span>   |<span data-ttu-id="a1ee4-155">説明</span><span class="sxs-lookup"><span data-stu-id="a1ee4-155">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a1ee4-156">バケット</span><span class="sxs-lookup"><span data-stu-id="a1ee4-156">buckets</span></span>|<span data-ttu-id="a1ee4-157">[plannerBucket](plannerbucket.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a1ee4-157">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="a1ee4-p107">読み取り専用です。Null 許容型。計画に含まれるバケットのコレクション。</span><span class="sxs-lookup"><span data-stu-id="a1ee4-p107">Read-only. Nullable. Collection of buckets in the plan.</span></span>|
|<span data-ttu-id="a1ee4-161">詳細</span><span class="sxs-lookup"><span data-stu-id="a1ee4-161">details</span></span>|[<span data-ttu-id="a1ee4-162">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="a1ee4-162">plannerPlanDetails</span></span>](plannerplandetails.md)| <span data-ttu-id="a1ee4-p108">読み取り専用です。Null 許容型。計画に関する追加の詳細。</span><span class="sxs-lookup"><span data-stu-id="a1ee4-p108">Read-only. Nullable. Additional details about the plan.</span></span>|
|<span data-ttu-id="a1ee4-166">タスク</span><span class="sxs-lookup"><span data-stu-id="a1ee4-166">tasks</span></span>|<span data-ttu-id="a1ee4-167">[plannerTask](plannertask.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a1ee4-167">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="a1ee4-p109">読み取り専用です。Null 許容型。計画に含まれるタスクのコレクション。</span><span class="sxs-lookup"><span data-stu-id="a1ee4-p109">Read-only. Nullable. Collection of tasks in the plan.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a1ee4-171">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a1ee4-171">JSON representation</span></span>

<span data-ttu-id="a1ee4-172">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a1ee4-172">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerPlan"
}-->

```json
{
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "owner": "String",
  "title": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerPlan resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->