# <a name="plannerplan-resource-type"></a><span data-ttu-id="71386-101">plannerPlan リソースの種類</span><span class="sxs-lookup"><span data-stu-id="71386-101">plannerPlan resource type</span></span>

<span data-ttu-id="71386-p101">**plannerPlan** リソースは、Office 365 での計画を表します。計画は [group](group.md) によって所有され、[plannerTasks](plannerTask.md) のコレクションが含まれています。[plannerBuckets](plannerBucket.md) のコレクションを含む場合もあります。各計画オブジェクトには [details](plannerPlanDetails.md) オブジェクトがあり、計画に関する詳細情報が含まれていることがあります。グループ、計画、タスク間のリレーションシップの詳細については、「[Planner](planner_overview.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="71386-p101">The **plannerPlan** resource represents a plan in Office 365. A plan can be owned by a [group](group.md) and contains a collection of [plannerTasks](plannerTask.md). It can also have a collection of [plannerBuckets](plannerBucket.md). Each plan object has a [details](plannerPlanDetails.md) object that can contain more information about the plan. For more information about the relationships between groups, plans, and tasks, see [Planner](planner_overview.md).</span></span>

## <a name="methods"></a><span data-ttu-id="71386-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="71386-107">Methods</span></span>

| <span data-ttu-id="71386-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="71386-108">Method</span></span>           | <span data-ttu-id="71386-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="71386-109">Return Type</span></span>    |<span data-ttu-id="71386-110">説明</span><span class="sxs-lookup"><span data-stu-id="71386-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="71386-111">Get plannerPlan</span><span class="sxs-lookup"><span data-stu-id="71386-111">Get plannerPlan</span></span>](../api/plannerplan_get.md) | [<span data-ttu-id="71386-112">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="71386-112">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="71386-113">**plannerPlan** オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="71386-113">Read properties and relationships of **plannerPlan** object.</span></span>|
|[<span data-ttu-id="71386-114">List buckets</span><span class="sxs-lookup"><span data-stu-id="71386-114">List buckets</span></span>](../api/plannerplan_list_buckets.md) |<span data-ttu-id="71386-115">[plannerBucket](plannerbucket.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="71386-115">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="71386-116">**plannerBucket** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="71386-116">Get a **plannerBucket** object collection.</span></span>|
|[<span data-ttu-id="71386-117">List tasks</span><span class="sxs-lookup"><span data-stu-id="71386-117">List tasks</span></span>](../api/plannerplan_list_tasks.md) |<span data-ttu-id="71386-118">[plannerTask](plannertask.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="71386-118">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="71386-119">**plannerTask** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="71386-119">Get a **plannerTask** object collection.</span></span>|
|[<span data-ttu-id="71386-120">Update</span><span class="sxs-lookup"><span data-stu-id="71386-120">Update</span></span>](../api/plannerplan_update.md) | [<span data-ttu-id="71386-121">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="71386-121">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="71386-122">**plannerPlan** オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="71386-122">Update **plannerPlan** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="71386-123">プロパティ</span><span class="sxs-lookup"><span data-stu-id="71386-123">Properties</span></span>
| <span data-ttu-id="71386-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="71386-124">Property</span></span>     | <span data-ttu-id="71386-125">型</span><span class="sxs-lookup"><span data-stu-id="71386-125">Type</span></span>   |<span data-ttu-id="71386-126">説明</span><span class="sxs-lookup"><span data-stu-id="71386-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="71386-127">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="71386-127">createdDateTime</span></span>|<span data-ttu-id="71386-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71386-128">DateTimeOffset</span></span>|<span data-ttu-id="71386-p102">読み取り専用。計画の作成日時。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="71386-p102">Read-only. Date and time at which the plan is created. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="71386-133">id</span><span class="sxs-lookup"><span data-stu-id="71386-133">id</span></span>|<span data-ttu-id="71386-134">文字列</span><span class="sxs-lookup"><span data-stu-id="71386-134">String</span></span>| <span data-ttu-id="71386-135">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="71386-135">Read-only.</span></span> <span data-ttu-id="71386-136">計画の ID です。</span><span class="sxs-lookup"><span data-stu-id="71386-136">ID of the plan.</span></span> <span data-ttu-id="71386-137">28 の文字、大文字小文字を区別することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="71386-137">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="71386-138">サービスの[フォーマットの検証](planner_identifiers_disclaimer.md)が行われます。</span><span class="sxs-lookup"><span data-stu-id="71386-138">[Format validation](planner_identifiers_disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="71386-139">owner</span><span class="sxs-lookup"><span data-stu-id="71386-139">owner</span></span>|<span data-ttu-id="71386-140">String</span><span class="sxs-lookup"><span data-stu-id="71386-140">String</span></span>|<span data-ttu-id="71386-141">計画を所有する[グループ](group.md)の ID です。</span><span class="sxs-lookup"><span data-stu-id="71386-141">ID of the [Group](group.md) that owns the plan.</span></span> <span data-ttu-id="71386-142">このフィールドを設定する前に、有効なグループが存在する必要があります。</span><span class="sxs-lookup"><span data-stu-id="71386-142">A valid group must exist before this field can be set.</span></span> <span data-ttu-id="71386-143">設定すると後、は、このプロパティを更新できません。</span><span class="sxs-lookup"><span data-stu-id="71386-143">After it is set, this property can’t be updated.</span></span>|
|<span data-ttu-id="71386-144">タイトル</span><span class="sxs-lookup"><span data-stu-id="71386-144">title</span></span>|<span data-ttu-id="71386-145">String</span><span class="sxs-lookup"><span data-stu-id="71386-145">String</span></span>|<span data-ttu-id="71386-p105">必須。計画のタイトル。</span><span class="sxs-lookup"><span data-stu-id="71386-p105">Required. Title of the plan.</span></span>|
|<span data-ttu-id="71386-148">createdBy</span><span class="sxs-lookup"><span data-stu-id="71386-148">createdBy</span></span>|[<span data-ttu-id="71386-149">identitySet</span><span class="sxs-lookup"><span data-stu-id="71386-149">identitySet</span></span>](identityset.md)|<span data-ttu-id="71386-p106">読み取り専用です。計画を作成したユーザー。</span><span class="sxs-lookup"><span data-stu-id="71386-p106">Read-only. The user who created the plan.</span></span>|

## <a name="relationships"></a><span data-ttu-id="71386-152">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="71386-152">Relationships</span></span>
| <span data-ttu-id="71386-153">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="71386-153">Relationship</span></span> | <span data-ttu-id="71386-154">型</span><span class="sxs-lookup"><span data-stu-id="71386-154">Type</span></span>   |<span data-ttu-id="71386-155">説明</span><span class="sxs-lookup"><span data-stu-id="71386-155">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="71386-156">buckets</span><span class="sxs-lookup"><span data-stu-id="71386-156">buckets</span></span>|<span data-ttu-id="71386-157">[plannerBucket](plannerbucket.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="71386-157">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="71386-p107">読み取り専用です。Null 許容型。計画に含まれるバケットのコレクション。</span><span class="sxs-lookup"><span data-stu-id="71386-p107">Read-only. Nullable. Collection of buckets in the plan.</span></span>|
|<span data-ttu-id="71386-161">詳細</span><span class="sxs-lookup"><span data-stu-id="71386-161">details</span></span>|[<span data-ttu-id="71386-162">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="71386-162">plannerPlanDetails</span></span>](plannerplandetails.md)| <span data-ttu-id="71386-p108">読み取り専用です。Null 許容型。計画に関する追加の詳細。</span><span class="sxs-lookup"><span data-stu-id="71386-p108">Read-only. Nullable. Additional details about the plan.</span></span>|
|<span data-ttu-id="71386-166">tasks</span><span class="sxs-lookup"><span data-stu-id="71386-166">tasks</span></span>|<span data-ttu-id="71386-167">[plannerTask](plannertask.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="71386-167">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="71386-p109">読み取り専用です。Null 許容型。計画に含まれるタスクのコレクション。</span><span class="sxs-lookup"><span data-stu-id="71386-p109">Read-only. Nullable. Collection of tasks in the plan.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="71386-171">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="71386-171">JSON representation</span></span>

<span data-ttu-id="71386-172">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="71386-172">Here is a JSON representation of the resource.</span></span>

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