# <a name="plannerprogresstaskboardtaskformat-resource-type"></a><span data-ttu-id="92584-101">plannerProgressTaskBoardTaskFormat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="92584-101">plannerProgressTaskBoardTaskFormat resource type</span></span>

<span data-ttu-id="92584-p101">**plannerProgressTaskBoardTaskFormat** リソースは、タスク ボードの進行状況ビューにタスクを正しく表示するための情報を示します (ビューはタスク オブジェクトの [未開始]、[処理中]、[完了] の列に示す PercentComplete フィールドの状態で整理されます)。各 [task](plannertask.md) にはそれぞれ **plannerProgressTaskBoardTaskFormat** オブジェクトが 1 つ関連付けられています。</span><span class="sxs-lookup"><span data-stu-id="92584-p101">The **plannerProgressTaskBoardTaskFormat** resource represents the information used to render a task correctly in the Progress view of the Task Board (a view organized by the state of the PercentComplete field on the task object, with columns for Not Started, In Progress and Complete). Each [task](plannertask.md) will have one **plannerProgressTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="92584-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="92584-104">Methods</span></span>

| <span data-ttu-id="92584-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="92584-105">Method</span></span>           | <span data-ttu-id="92584-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="92584-106">Return Type</span></span>    |<span data-ttu-id="92584-107">説明</span><span class="sxs-lookup"><span data-stu-id="92584-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="92584-108">plannerProgressTaskBoardTaskFormat の取得</span><span class="sxs-lookup"><span data-stu-id="92584-108">Get plannerProgressTaskBoardTaskFormat</span></span>](../api/plannerprogresstaskboardtaskformat_get.md) | [<span data-ttu-id="92584-109">plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="92584-109">plannerProgressTaskBoardTaskFormat</span></span>](plannerprogresstaskboardtaskformat.md) |<span data-ttu-id="92584-110">**plannerProgressTaskBoardTaskFormat** オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="92584-110">Read properties and relationships of **plannerProgressTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="92584-111">更新</span><span class="sxs-lookup"><span data-stu-id="92584-111">Update</span></span>](../api/plannerprogresstaskboardtaskformat_update.md) | [<span data-ttu-id="92584-112">plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="92584-112">plannerProgressTaskBoardTaskFormat</span></span>](plannerprogresstaskboardtaskformat.md)    |<span data-ttu-id="92584-113">**plannerProgressTaskBoardTaskFormat** オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="92584-113">Update **plannerProgressTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="92584-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="92584-114">Properties</span></span>
| <span data-ttu-id="92584-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="92584-115">Property</span></span>     | <span data-ttu-id="92584-116">タイプ</span><span class="sxs-lookup"><span data-stu-id="92584-116">Type</span></span>   |<span data-ttu-id="92584-117">説明</span><span class="sxs-lookup"><span data-stu-id="92584-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="92584-118">ID</span><span class="sxs-lookup"><span data-stu-id="92584-118">id</span></span>|<span data-ttu-id="92584-119">文字列</span><span class="sxs-lookup"><span data-stu-id="92584-119">String</span></span>| <span data-ttu-id="92584-120">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="92584-120">Read-only.</span></span> <span data-ttu-id="92584-121">リソースの ID。</span><span class="sxs-lookup"><span data-stu-id="92584-121">The ID of the resource.</span></span> <span data-ttu-id="92584-122">28 文字で大文字小文字を区別します。</span><span class="sxs-lookup"><span data-stu-id="92584-122">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="92584-123">サービスの[フォーマットの検証](planner_identifiers_disclaimer.md) が行われます。</span><span class="sxs-lookup"><span data-stu-id="92584-123">[Format validation](planner_identifiers_disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="92584-124">orderHint</span><span class="sxs-lookup"><span data-stu-id="92584-124">orderHint</span></span>|<span data-ttu-id="92584-125">文字列</span><span class="sxs-lookup"><span data-stu-id="92584-125">String</span></span>|<span data-ttu-id="92584-p103">タスク ボードの進行状況ビューでタスクの順序付けに使用するヒントの値。形式は[ここ](planner_order_hint_format.md)の説明に従って定義されます。</span><span class="sxs-lookup"><span data-stu-id="92584-p103">Hint value used to order the task on the Progress view of the Task Board. The format is defined as outlined [here](planner_order_hint_format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="92584-128">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="92584-128">Relationships</span></span>
<span data-ttu-id="92584-129">なし</span><span class="sxs-lookup"><span data-stu-id="92584-129">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="92584-130">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="92584-130">JSON representation</span></span>
<span data-ttu-id="92584-131">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="92584-131">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.plannerProgressTaskBoardTaskFormat"
}-->

```json
{
  "id": "String (identifier)",
  "orderHint": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerProgressTaskBoardTaskFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->