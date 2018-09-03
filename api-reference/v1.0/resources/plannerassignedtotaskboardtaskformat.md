# <a name="plannerassignedtotaskboardtaskformat-resource-type"></a><span data-ttu-id="827fd-101">plannerAssignedToTaskBoardTaskFormat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="827fd-101">plannerAssignedToTaskBoardTaskFormat resource type</span></span>

<span data-ttu-id="827fd-p101">**PlannerAssignedToTaskBoardTaskFormat** リソースは、タスク ボードの AssignedTo ビューを正しく表示するための情報を示します (ビューはタスクが割り当てられているユーザーごとに整理されます)。各 [task](plannertask.md) にはそれぞれ **plannerAssignedToTaskBoardTaskFormat** オブジェクトが 1 つ関連付けられています。</span><span class="sxs-lookup"><span data-stu-id="827fd-p101">The **plannerAssignedToTaskBoardTaskFormat** resource represents the information used to render a task correctly in the AssignedTo view of the Task Board (a view organized by users to whom tasks are assigned to). Each [task](plannertask.md) will have one **plannerAssignedToTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="827fd-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="827fd-104">Methods</span></span>

| <span data-ttu-id="827fd-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="827fd-105">Method</span></span>           | <span data-ttu-id="827fd-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="827fd-106">Return Type</span></span>    |<span data-ttu-id="827fd-107">説明</span><span class="sxs-lookup"><span data-stu-id="827fd-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="827fd-108">plannerAssignedToTaskBoardTaskFormat の取得</span><span class="sxs-lookup"><span data-stu-id="827fd-108">Get plannerAssignedToTaskBoardTaskFormat</span></span>](../api/plannerassignedtotaskboardtaskformat_get.md) | [<span data-ttu-id="827fd-109">plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="827fd-109">plannerAssignedToTaskBoardTaskFormat</span></span>](plannerassignedtotaskboardtaskformat.md) |<span data-ttu-id="827fd-110">**plannerAssignedToTaskBoardTaskFormat** オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="827fd-110">Read properties and relationships of **plannerAssignedToTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="827fd-111">更新する</span><span class="sxs-lookup"><span data-stu-id="827fd-111">Update</span></span>](../api/plannerassignedtotaskboardtaskformat_update.md) | [<span data-ttu-id="827fd-112">plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="827fd-112">plannerAssignedToTaskBoardTaskFormat</span></span>](plannerassignedtotaskboardtaskformat.md)  |<span data-ttu-id="827fd-113">**plannerAssignedToTaskBoardTaskFormat** オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="827fd-113">Update **plannerAssignedToTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="827fd-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="827fd-114">Properties</span></span>
| <span data-ttu-id="827fd-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="827fd-115">Property</span></span>     | <span data-ttu-id="827fd-116">タイプ</span><span class="sxs-lookup"><span data-stu-id="827fd-116">Type</span></span>   |<span data-ttu-id="827fd-117">説明</span><span class="sxs-lookup"><span data-stu-id="827fd-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="827fd-118">ID</span><span class="sxs-lookup"><span data-stu-id="827fd-118">id</span></span>|<span data-ttu-id="827fd-119">文字列</span><span class="sxs-lookup"><span data-stu-id="827fd-119">String</span></span>| <span data-ttu-id="827fd-120">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="827fd-120">Read-only.</span></span> <span data-ttu-id="827fd-121">リソースの ID。</span><span class="sxs-lookup"><span data-stu-id="827fd-121">The ID of the resource.</span></span> <span data-ttu-id="827fd-122">28 文字で大文字小文字を区別します。</span><span class="sxs-lookup"><span data-stu-id="827fd-122">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="827fd-123">サービスの[フォーマットの検証](planner_identifiers_disclaimer.md) が行われます。</span><span class="sxs-lookup"><span data-stu-id="827fd-123">[Format validation](planner_identifiers_disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="827fd-124">orderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="827fd-124">orderHintsByAssignee</span></span>|[<span data-ttu-id="827fd-125">plannerOrderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="827fd-125">plannerOrderHintsByAssignee</span></span>](plannerorderhintsbyassignee.md)|<span data-ttu-id="827fd-p103">タスク ボードの AssignedTo ビューでのタスクの順序付けに使用するヒントのディクショナリ。各エントリのキーは、タスクが割り当てられているユーザーのいずれかであり、値は順序のヒントです。それぞれの値の形式は[ここ](planner_order_hint_format.md)で説明するとおり定義されます。</span><span class="sxs-lookup"><span data-stu-id="827fd-p103">Dictionary of hints used to order tasks on the AssignedTo view of the Task Board. The key of each entry is one of the users the task is assigned to and the value is the order hint. The format of each value is defined as outlined [here](planner_order_hint_format.md).</span></span>|
|<span data-ttu-id="827fd-129">unassignedOrderHint</span><span class="sxs-lookup"><span data-stu-id="827fd-129">unassignedOrderHint</span></span>|<span data-ttu-id="827fd-130">文字列</span><span class="sxs-lookup"><span data-stu-id="827fd-130">String</span></span>|<span data-ttu-id="827fd-p104">タスクが誰にも割り当てられていない場合、または orderHintsByAssignee ディクショナリに、タスクが割り当てられているユーザーのヒントの順序が指定されない場合に、タスク ボードの AssignedTo ビューでのタスクの順序付けに使用するヒントの値。形式は[ここ](planner_order_hint_format.md)の説明に従って定義されます。</span><span class="sxs-lookup"><span data-stu-id="827fd-p104">Hint value used to order the task on the AssignedTo view of the Task Board when the task is not assigned to anyone, or if the orderHintsByAssignee dictionary does not provide an order hint for the user the task is assigned to. The format is defined as outlined [here](planner_order_hint_format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="827fd-133">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="827fd-133">Relationships</span></span>
<span data-ttu-id="827fd-134">なし</span><span class="sxs-lookup"><span data-stu-id="827fd-134">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="827fd-135">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="827fd-135">JSON representation</span></span>
<span data-ttu-id="827fd-136">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="827fd-136">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.plannerAssignedToTaskBoardTaskFormat"
}-->

```json
{
  "id": "String (identifier)",
  "orderHintsByAssignee": {"@odata.type": "microsoft.graph.plannerOrderHintsByAssignee"},
  "unassignedOrderHint": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerAssignedToTaskBoardTaskFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->