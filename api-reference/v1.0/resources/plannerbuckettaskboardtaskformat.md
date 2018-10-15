# <a name="plannerbuckettaskboardtaskformat-resource-type"></a><span data-ttu-id="d14c4-101">plannerBucketTaskBoardTaskFormat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d14c4-101">plannerBucketTaskBoardTaskFormat resource type</span></span>

<span data-ttu-id="d14c4-p101">**plannerBucketTaskBoardTaskFormat** リソースは、タスク ボードのバケット ビューでタスクを正しく表示するための情報を示します (ビューは割り当てられているバケット内のタスクごとに整理されます)。各 [task](plannertask.md) にはそれぞれ **plannerBucketTaskBoardTaskFormat** オブジェクトが 1 つ関連付けられています。</span><span class="sxs-lookup"><span data-stu-id="d14c4-p101">The **plannerBucketTaskBoardTaskFormat** resource represents the information used to render a task correctly in the Buckets view of the Task Board (a view organized by tasks within the buckets they are assigned to). Each [task](plannertask.md) will have one **plannerBucketTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="d14c4-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="d14c4-104">Methods</span></span>

| <span data-ttu-id="d14c4-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="d14c4-105">Method</span></span>           | <span data-ttu-id="d14c4-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="d14c4-106">Return Type</span></span>    |<span data-ttu-id="d14c4-107">説明</span><span class="sxs-lookup"><span data-stu-id="d14c4-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d14c4-108">plannerBucketTaskBoardTaskFormat の取得</span><span class="sxs-lookup"><span data-stu-id="d14c4-108">Get plannerBucketTaskBoardTaskFormat</span></span>](../api/plannerbuckettaskboardtaskformat_get.md) | [<span data-ttu-id="d14c4-109">plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="d14c4-109">plannerBucketTaskBoardTaskFormat</span></span>](plannerbuckettaskboardtaskformat.md) |<span data-ttu-id="d14c4-110">**plannerBucketTaskBoardTaskFormat** オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="d14c4-110">Read properties and relationships of **plannerBucketTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="d14c4-111">Update</span><span class="sxs-lookup"><span data-stu-id="d14c4-111">Update</span></span>](../api/plannerbuckettaskboardtaskformat_update.md) | [<span data-ttu-id="d14c4-112">plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="d14c4-112">plannerBucketTaskBoardTaskFormat</span></span>](plannerbuckettaskboardtaskformat.md)  |<span data-ttu-id="d14c4-113">**plannerBucketTaskBoardTaskFormat** オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="d14c4-113">Update **plannerBucketTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="d14c4-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d14c4-114">Properties</span></span>
| <span data-ttu-id="d14c4-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d14c4-115">Property</span></span>     | <span data-ttu-id="d14c4-116">タイプ</span><span class="sxs-lookup"><span data-stu-id="d14c4-116">Type</span></span>   |<span data-ttu-id="d14c4-117">説明</span><span class="sxs-lookup"><span data-stu-id="d14c4-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d14c4-118">id</span><span class="sxs-lookup"><span data-stu-id="d14c4-118">id</span></span>|<span data-ttu-id="d14c4-119">文字列</span><span class="sxs-lookup"><span data-stu-id="d14c4-119">String</span></span>| <span data-ttu-id="d14c4-120">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="d14c4-120">Read-only.</span></span> <span data-ttu-id="d14c4-121">リソースの ID。</span><span class="sxs-lookup"><span data-stu-id="d14c4-121">The ID of the resource.</span></span> <span data-ttu-id="d14c4-122">28 文字で大文字小文字を区別します。</span><span class="sxs-lookup"><span data-stu-id="d14c4-122">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="d14c4-123">サービスの[フォーマットの検証](planner_identifiers_disclaimer.md) が行われます。</span><span class="sxs-lookup"><span data-stu-id="d14c4-123">[Format validation](planner_identifiers_disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="d14c4-124">orderHint</span><span class="sxs-lookup"><span data-stu-id="d14c4-124">orderHint</span></span>|<span data-ttu-id="d14c4-125">文字列</span><span class="sxs-lookup"><span data-stu-id="d14c4-125">String</span></span>|<span data-ttu-id="d14c4-p103">タスク ボードのバケット ビューでタスクの順序付けに使用するヒント。形式は[ここ](planner_order_hint_format.md)の説明に従って定義されます。</span><span class="sxs-lookup"><span data-stu-id="d14c4-p103">Hint used to order tasks in the Bucket view of the Task Board. The format is defined as outlined [here](planner_order_hint_format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="d14c4-128">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d14c4-128">Relationships</span></span>
<span data-ttu-id="d14c4-129">なし</span><span class="sxs-lookup"><span data-stu-id="d14c4-129">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="d14c4-130">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d14c4-130">JSON representation</span></span>
<span data-ttu-id="d14c4-131">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d14c4-131">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.plannerBucketTaskBoardTaskFormat"
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
  "description": "plannerBucketTaskBoardTaskFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->