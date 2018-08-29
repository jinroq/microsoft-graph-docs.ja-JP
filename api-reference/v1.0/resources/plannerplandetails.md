# <a name="plannerplandetails-resource-type"></a><span data-ttu-id="a5035-101">plannerPlanDetails リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a5035-101">plannerPlanDetails resource type</span></span>


<span data-ttu-id="a5035-p101">**plannerPlanDetails** リソースは、計画に関する追加情報を表します。各 [plan](plannerplan.md) オブジェクトには詳細オブジェクトがあります。</span><span class="sxs-lookup"><span data-stu-id="a5035-p101">The **plannerPlanDetails** resource represents the additional information about a plan. Each [plan](plannerplan.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="a5035-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="a5035-104">Methods</span></span>

| <span data-ttu-id="a5035-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="a5035-105">Method</span></span>           | <span data-ttu-id="a5035-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="a5035-106">Return Type</span></span>    |<span data-ttu-id="a5035-107">説明</span><span class="sxs-lookup"><span data-stu-id="a5035-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a5035-108">plannerPlanDetails を取得</span><span class="sxs-lookup"><span data-stu-id="a5035-108">Get plannerPlanDetails</span></span>](../api/plannerplandetails_get.md) | [<span data-ttu-id="a5035-109">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="a5035-109">plannerPlanDetails</span></span>](plannerplandetails.md) |<span data-ttu-id="a5035-110">**plannerPlanDetails** オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="a5035-110">Read properties and relationships of **plannerPlanDetails** object.</span></span>|
|[<span data-ttu-id="a5035-111">更新する</span><span class="sxs-lookup"><span data-stu-id="a5035-111">Update</span></span>](../api/plannerplandetails_update.md) | [<span data-ttu-id="a5035-112">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="a5035-112">plannerPlanDetails</span></span>](plannerplandetails.md)    |<span data-ttu-id="a5035-113">**plannerPlanDetails** オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="a5035-113">Update **plannerPlanDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="a5035-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a5035-114">Properties</span></span>
| <span data-ttu-id="a5035-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a5035-115">Property</span></span>     | <span data-ttu-id="a5035-116">タイプ</span><span class="sxs-lookup"><span data-stu-id="a5035-116">Type</span></span>   |<span data-ttu-id="a5035-117">説明</span><span class="sxs-lookup"><span data-stu-id="a5035-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a5035-118">categoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="a5035-118">categoryDescriptions</span></span>|[<span data-ttu-id="a5035-119">plannerCategoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="a5035-119">plannerCategoryDescriptions</span></span>](plannercategorydescriptions.md)|<span data-ttu-id="a5035-120">計画内のタスクに関連付けられる 6 つのカテゴリの説明を指定するオブジェクト</span><span class="sxs-lookup"><span data-stu-id="a5035-120">An object that specifies the descriptions of the six categories that can be associated with tasks in the plan</span></span>|
|<span data-ttu-id="a5035-121">ID</span><span class="sxs-lookup"><span data-stu-id="a5035-121">id</span></span>|<span data-ttu-id="a5035-122">文字列</span><span class="sxs-lookup"><span data-stu-id="a5035-122">String</span></span>| <span data-ttu-id="a5035-123">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="a5035-123">Read-only.</span></span> <span data-ttu-id="a5035-124">計画の ID です。</span><span class="sxs-lookup"><span data-stu-id="a5035-124">ID of the plan details.</span></span> <span data-ttu-id="a5035-125">28 文字で大文字小文字を区別します。</span><span class="sxs-lookup"><span data-stu-id="a5035-125">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="a5035-126">サービスの[フォーマットの検証](planner_identifiers_disclaimer.md) が行われます。</span><span class="sxs-lookup"><span data-stu-id="a5035-126">[Format validation](planner_identifiers_disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="a5035-127">sharedWith</span><span class="sxs-lookup"><span data-stu-id="a5035-127">sharedWith</span></span>|[<span data-ttu-id="a5035-128">plannerUserIds</span><span class="sxs-lookup"><span data-stu-id="a5035-128">plannerUserIds</span></span>](planneruserids.md)|<span data-ttu-id="a5035-p103">この計画を共有するユーザー ID を設定します。Office 365 グループを活用している場合は、グループの API を使用してグループのメンバーシップを管理し、[グループの](group.md)計画を共有します。グループの既存のメンバーもこのコレクションに追加できますが、このグループが所有する計画へのアクセスは必要とされません。</span><span class="sxs-lookup"><span data-stu-id="a5035-p103">Set of user ids that this plan is shared with. If you are leveraging Office 365 Groups, use the Groups API to manage group membership to share the [group's](group.md) plan. You can also add existing members of the group to this collection though it is not required for them to access the plan owned by the group.</span></span> |

## <a name="relationships"></a><span data-ttu-id="a5035-132">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a5035-132">Relationships</span></span>
<span data-ttu-id="a5035-133">なし</span><span class="sxs-lookup"><span data-stu-id="a5035-133">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="a5035-134">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a5035-134">JSON representation</span></span>
<span data-ttu-id="a5035-135">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a5035-135">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.plannerPlanDetails"
}-->

```json
{
  "categoryDescriptions": {"@odata.type": "microsoft.graph.plannerCategoryDescriptions"},
  "id": "String (identifier)",
  "sharedWith": {"@odata.type": "microsoft.graph.plannerUserIds"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerPlanDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->