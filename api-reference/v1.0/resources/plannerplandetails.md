# <a name="plannerplandetails-resource-type"></a><span data-ttu-id="b8430-101">plannerPlanDetails リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b8430-101">plannerPlanDetails resource type</span></span>


<span data-ttu-id="b8430-p101">**plannerPlanDetails** リソースは、計画に関する追加情報を表します。各 [plan](plannerplan.md) オブジェクトには詳細オブジェクトがあります。</span><span class="sxs-lookup"><span data-stu-id="b8430-p101">The **plannerPlanDetails** resource represents the additional information about a plan. Each [plan](plannerplan.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="b8430-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="b8430-104">Methods</span></span>

| <span data-ttu-id="b8430-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="b8430-105">Method</span></span>           | <span data-ttu-id="b8430-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="b8430-106">Return Type</span></span>    |<span data-ttu-id="b8430-107">説明</span><span class="sxs-lookup"><span data-stu-id="b8430-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b8430-108">Get plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="b8430-108">Get plannerPlanDetails</span></span>](../api/plannerplandetails_get.md) | [<span data-ttu-id="b8430-109">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="b8430-109">plannerPlanDetails</span></span>](plannerplandetails.md) |<span data-ttu-id="b8430-110">**plannerPlanDetails** オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="b8430-110">Read properties and relationships of **plannerPlanDetails** object.</span></span>|
|[<span data-ttu-id="b8430-111">Update</span><span class="sxs-lookup"><span data-stu-id="b8430-111">Update</span></span>](../api/plannerplandetails_update.md) | [<span data-ttu-id="b8430-112">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="b8430-112">plannerPlanDetails</span></span>](plannerplandetails.md)    |<span data-ttu-id="b8430-113">**plannerPlanDetails** オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="b8430-113">Update **plannerPlanDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="b8430-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b8430-114">Properties</span></span>
| <span data-ttu-id="b8430-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b8430-115">Property</span></span>     | <span data-ttu-id="b8430-116">型</span><span class="sxs-lookup"><span data-stu-id="b8430-116">Type</span></span>   |<span data-ttu-id="b8430-117">説明</span><span class="sxs-lookup"><span data-stu-id="b8430-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b8430-118">categoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="b8430-118">categoryDescriptions</span></span>|[<span data-ttu-id="b8430-119">plannerCategoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="b8430-119">plannerCategoryDescriptions</span></span>](plannercategorydescriptions.md)|<span data-ttu-id="b8430-120">計画内のタスクに関連付けられる 6 つのカテゴリの説明を指定するオブジェクト</span><span class="sxs-lookup"><span data-stu-id="b8430-120">An object that specifies the descriptions of the six categories that can be associated with tasks in the plan</span></span>|
|<span data-ttu-id="b8430-121">id</span><span class="sxs-lookup"><span data-stu-id="b8430-121">id</span></span>|<span data-ttu-id="b8430-122">String</span><span class="sxs-lookup"><span data-stu-id="b8430-122">String</span></span>| <span data-ttu-id="b8430-p102">読み取り専用です。計画の詳細の ID。28 文字長で、大文字と小文字の区別があります。[書式検証](planner_identifiers_disclaimer.md)はサービスによって行われます。</span><span class="sxs-lookup"><span data-stu-id="b8430-p102">Read-only. ID of the plan details. It is 28 characters long and case sensitive. [Format validation](planner_identifiers_disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="b8430-127">sharedWith</span><span class="sxs-lookup"><span data-stu-id="b8430-127">sharedWith</span></span>|[<span data-ttu-id="b8430-128">plannerUserIds</span><span class="sxs-lookup"><span data-stu-id="b8430-128">plannerUserIds</span></span>](planneruserids.md)|<span data-ttu-id="b8430-p103">この計画を共有するユーザー ID を設定します。Office 365 グループを活用している場合は、グループの API を使用してグループのメンバーシップを管理し、[グループの](group.md)計画を共有します。グループの既存のメンバーもこのコレクションに追加できますが、このグループが所有する計画へのアクセスは必要とされません。</span><span class="sxs-lookup"><span data-stu-id="b8430-p103">Set of user ids that this plan is shared with. If you are leveraging Office 365 Groups, use the Groups API to manage group membership to share the [group's](group.md) plan. You can also add existing members of the group to this collection though it is not required for them to access the plan owned by the group.</span></span> |

## <a name="relationships"></a><span data-ttu-id="b8430-132">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b8430-132">Relationships</span></span>
<span data-ttu-id="b8430-133">なし</span><span class="sxs-lookup"><span data-stu-id="b8430-133">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="b8430-134">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b8430-134">JSON representation</span></span>
<span data-ttu-id="b8430-135">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b8430-135">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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