# <a name="plannertaskdetails-resource-type"></a><span data-ttu-id="de610-101">plannerTaskDetails リソースの種類</span><span class="sxs-lookup"><span data-stu-id="de610-101">plannerTaskDetails resource type</span></span>

<span data-ttu-id="de610-p101">**plannerTaskDetails** リソースは、タスクに関する追加情報を表します。各 [task](plannertask.md) オブジェクトには詳細オブジェクトがあります。</span><span class="sxs-lookup"><span data-stu-id="de610-p101">The **plannerTaskDetails** resource represents the additional information about a task. Each [task](plannertask.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="de610-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="de610-104">Methods</span></span>

| <span data-ttu-id="de610-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="de610-105">Method</span></span>           | <span data-ttu-id="de610-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="de610-106">Return Type</span></span>    |<span data-ttu-id="de610-107">説明</span><span class="sxs-lookup"><span data-stu-id="de610-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="de610-108">plannerTaskDetails を取得</span><span class="sxs-lookup"><span data-stu-id="de610-108">Get plannerTaskDetails</span></span>](../api/plannertaskdetails_get.md) | [<span data-ttu-id="de610-109">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="de610-109">plannerTaskDetails</span></span>](plannertaskdetails.md) |<span data-ttu-id="de610-110">**plannerTaskDetails** オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="de610-110">Read properties and relationships of **plannerTaskDetails** object.</span></span>|
|[<span data-ttu-id="de610-111">更新</span><span class="sxs-lookup"><span data-stu-id="de610-111">Update</span></span>](../api/plannertaskdetails_update.md) | [<span data-ttu-id="de610-112">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="de610-112">plannerTaskDetails</span></span>](plannertaskdetails.md)    |<span data-ttu-id="de610-113">**plannerTaskDetails** オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="de610-113">Update **plannerTaskDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="de610-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="de610-114">Properties</span></span>
| <span data-ttu-id="de610-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="de610-115">Property</span></span>     | <span data-ttu-id="de610-116">タイプ</span><span class="sxs-lookup"><span data-stu-id="de610-116">Type</span></span>   |<span data-ttu-id="de610-117">説明</span><span class="sxs-lookup"><span data-stu-id="de610-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="de610-118">checklist</span><span class="sxs-lookup"><span data-stu-id="de610-118">checklist</span></span>|[<span data-ttu-id="de610-119">plannerChecklistItems</span><span class="sxs-lookup"><span data-stu-id="de610-119">plannerChecklistItems</span></span>](plannerchecklistitems.md)|<span data-ttu-id="de610-120">タスク上のチェックリスト項目のコレクション。</span><span class="sxs-lookup"><span data-stu-id="de610-120">The collection of checklist items on the task.</span></span>|
|<span data-ttu-id="de610-121">説明</span><span class="sxs-lookup"><span data-stu-id="de610-121">description</span></span>|<span data-ttu-id="de610-122">文字列</span><span class="sxs-lookup"><span data-stu-id="de610-122">String</span></span>|<span data-ttu-id="de610-123">タスクの説明</span><span class="sxs-lookup"><span data-stu-id="de610-123">Description of the task</span></span>|
|<span data-ttu-id="de610-124">id</span><span class="sxs-lookup"><span data-stu-id="de610-124">id</span></span>|<span data-ttu-id="de610-125">文字列</span><span class="sxs-lookup"><span data-stu-id="de610-125">String</span></span>| <span data-ttu-id="de610-126">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="de610-126">Read-only.</span></span> <span data-ttu-id="de610-127">タスクの詳細の ID です。</span><span class="sxs-lookup"><span data-stu-id="de610-127">The ID of the workflow task.</span></span> <span data-ttu-id="de610-128">28 文字で大文字小文字を区別します。</span><span class="sxs-lookup"><span data-stu-id="de610-128">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="de610-129">サービスの[フォーマットの検証](planner_identifiers_disclaimer.md) が行われます。</span><span class="sxs-lookup"><span data-stu-id="de610-129">[Format validation](planner_identifiers_disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="de610-130">previewType</span><span class="sxs-lookup"><span data-stu-id="de610-130">previewType</span></span>|<span data-ttu-id="de610-131">文字列</span><span class="sxs-lookup"><span data-stu-id="de610-131">string</span></span>|<span data-ttu-id="de610-132">タスクに表示されるプレビューの種類を設定します。</span><span class="sxs-lookup"><span data-stu-id="de610-132">This sets the type of preview that shows up on the task. Possible values are: , , , , .</span></span> <span data-ttu-id="de610-133">可能な値は、`automatic`、`noPreview`、`checklist`、`description`、`reference` です。</span><span class="sxs-lookup"><span data-stu-id="de610-133">The possible values are `automatic`, `noPreview`, `checklist`, `description`, `reference`, , , , , , , or .</span></span> <span data-ttu-id="de610-134">`automatic` に設定されている場合、表示されるプレビューは、タスクを表示するアプリによって選択されます。</span><span class="sxs-lookup"><span data-stu-id="de610-134">This sets the type of preview that shows up on the task. Possible values are: , , , , . When set to `automatic` the displayed preview is chosen by the app viewing the task.</span></span>|
|<span data-ttu-id="de610-135">references</span><span class="sxs-lookup"><span data-stu-id="de610-135">references</span></span>|[<span data-ttu-id="de610-136">plannerExternalReferences</span><span class="sxs-lookup"><span data-stu-id="de610-136">plannerExternalReferences</span></span>](plannerexternalreferences.md)|<span data-ttu-id="de610-137">タスク上の参照のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="de610-137">The collection of references on the task.</span></span>|

## <a name="relationships"></a><span data-ttu-id="de610-138">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="de610-138">Relationships</span></span>
<span data-ttu-id="de610-139">なし</span><span class="sxs-lookup"><span data-stu-id="de610-139">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="de610-140">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="de610-140">JSON representation</span></span>
<span data-ttu-id="de610-141">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="de610-141">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.plannerTaskDetails"
}-->

```json
{
  "checklist": {"@odata.type": "microsoft.graph.plannerChecklistItems"},
  "description": "String",
  "id": "String (identifier)",
  "previewType": "string",
  "references": {"@odata.type": "microsoft.graph.plannerExternalReferences"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerTaskDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
