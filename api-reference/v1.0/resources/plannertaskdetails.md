# <a name="plannertaskdetails-resource-type"></a><span data-ttu-id="c41c3-101">plannerTaskDetails リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c41c3-101">plannerTaskDetails resource type</span></span>

<span data-ttu-id="c41c3-p101">**plannerTaskDetails** リソースは、タスクに関する追加情報を表します。各 [task](plannertask.md) オブジェクトには詳細オブジェクトがあります。</span><span class="sxs-lookup"><span data-stu-id="c41c3-p101">The **plannerTaskDetails** resource represents the additional information about a task. Each [task](plannertask.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="c41c3-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="c41c3-104">Methods</span></span>

| <span data-ttu-id="c41c3-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="c41c3-105">Method</span></span>           | <span data-ttu-id="c41c3-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="c41c3-106">Return Type</span></span>    |<span data-ttu-id="c41c3-107">説明</span><span class="sxs-lookup"><span data-stu-id="c41c3-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c41c3-108">Get plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="c41c3-108">Get plannerTaskDetails</span></span>](../api/plannertaskdetails_get.md) | [<span data-ttu-id="c41c3-109">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="c41c3-109">plannerTaskDetails</span></span>](plannertaskdetails.md) |<span data-ttu-id="c41c3-110">**plannerTaskDetails** オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="c41c3-110">Read properties and relationships of **plannerTaskDetails** object.</span></span>|
|[<span data-ttu-id="c41c3-111">Update</span><span class="sxs-lookup"><span data-stu-id="c41c3-111">Update</span></span>](../api/plannertaskdetails_update.md) | [<span data-ttu-id="c41c3-112">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="c41c3-112">plannerTaskDetails</span></span>](plannertaskdetails.md)    |<span data-ttu-id="c41c3-113">**plannerTaskDetails** オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="c41c3-113">Update **plannerTaskDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="c41c3-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c41c3-114">Properties</span></span>
| <span data-ttu-id="c41c3-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c41c3-115">Property</span></span>     | <span data-ttu-id="c41c3-116">型</span><span class="sxs-lookup"><span data-stu-id="c41c3-116">Type</span></span>   |<span data-ttu-id="c41c3-117">説明</span><span class="sxs-lookup"><span data-stu-id="c41c3-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c41c3-118">checklist</span><span class="sxs-lookup"><span data-stu-id="c41c3-118">checklist</span></span>|[<span data-ttu-id="c41c3-119">plannerChecklistItems</span><span class="sxs-lookup"><span data-stu-id="c41c3-119">plannerChecklistItems</span></span>](plannerchecklistitems.md)|<span data-ttu-id="c41c3-120">タスク上のチェックリスト項目のコレクション。</span><span class="sxs-lookup"><span data-stu-id="c41c3-120">The collection of checklist items on the task.</span></span>|
|<span data-ttu-id="c41c3-121">description</span><span class="sxs-lookup"><span data-stu-id="c41c3-121">description</span></span>|<span data-ttu-id="c41c3-122">String</span><span class="sxs-lookup"><span data-stu-id="c41c3-122">String</span></span>|<span data-ttu-id="c41c3-123">タスクの説明</span><span class="sxs-lookup"><span data-stu-id="c41c3-123">Description of the task</span></span>|
|<span data-ttu-id="c41c3-124">id</span><span class="sxs-lookup"><span data-stu-id="c41c3-124">id</span></span>|<span data-ttu-id="c41c3-125">String</span><span class="sxs-lookup"><span data-stu-id="c41c3-125">String</span></span>| <span data-ttu-id="c41c3-p102">読み取り専用です。タスクの詳細の ID。28 文字長で、大文字と小文字の区別があります。[書式検証](planner_identifiers_disclaimer.md)はサービスによって行われます。</span><span class="sxs-lookup"><span data-stu-id="c41c3-p102">Read-only. ID of the task details. It is 28 characters long and case sensitive. [Format validation](planner_identifiers_disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="c41c3-130">previewType</span><span class="sxs-lookup"><span data-stu-id="c41c3-130">previewType</span></span>|<span data-ttu-id="c41c3-131">string</span><span class="sxs-lookup"><span data-stu-id="c41c3-131">string</span></span>|<span data-ttu-id="c41c3-p103">タスクに表示されるプレビューの種類を設定します。使用可能な値: `automatic`、`noPreview`、`checklist`、`description`、`reference`。`automatic` に設定すると、タスクを表示しているアプリによって表示するプレビューが選択されます。</span><span class="sxs-lookup"><span data-stu-id="c41c3-p103">This sets the type of preview that shows up on the task. Possible values are: `automatic`, `noPreview`, `checklist`, `description`, `reference`. When set to `automatic` the displayed preview is chosen by the app viewing the task.</span></span>|
|<span data-ttu-id="c41c3-135">references</span><span class="sxs-lookup"><span data-stu-id="c41c3-135">references</span></span>|[<span data-ttu-id="c41c3-136">plannerExternalReferences</span><span class="sxs-lookup"><span data-stu-id="c41c3-136">plannerExternalReferences</span></span>](plannerexternalreferences.md)|<span data-ttu-id="c41c3-137">タスク上の参照のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="c41c3-137">The collection of references on the task.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c41c3-138">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c41c3-138">Relationships</span></span>
<span data-ttu-id="c41c3-139">なし</span><span class="sxs-lookup"><span data-stu-id="c41c3-139">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="c41c3-140">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c41c3-140">JSON representation</span></span>
<span data-ttu-id="c41c3-141">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c41c3-141">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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