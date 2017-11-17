# <a name="onenoteoperation-resource-type"></a><span data-ttu-id="21845-101">onenoteOperation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="21845-101">onenoteOperation resource type</span></span>

<span data-ttu-id="21845-102">OneNote の特定の長時間操作の状態。</span><span class="sxs-lookup"><span data-stu-id="21845-102">The status of certain long-running OneNote operations.</span></span>

## <a name="json-representation"></a><span data-ttu-id="21845-103">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="21845-103">JSON representation</span></span>

<span data-ttu-id="21845-104">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="21845-104">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteOperation"
}-->

```json
{
  "createdDateTime": "String (timestamp)",
  "error": {"@odata.type": "microsoft.graph.onenoteOperationError"},
  "id": "string (identifier)",
  "lastActionDateTime": "String (timestamp)",
  "resourceId": "string",
  "resourceLocation": "string",
  "status": "string",
  "percentComplete": "string"
}

```
## <a name="properties"></a><span data-ttu-id="21845-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="21845-105">Properties</span></span>
| <span data-ttu-id="21845-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="21845-106">Property</span></span>     | <span data-ttu-id="21845-107">型</span><span class="sxs-lookup"><span data-stu-id="21845-107">Type</span></span>   |<span data-ttu-id="21845-108">説明</span><span class="sxs-lookup"><span data-stu-id="21845-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="21845-109">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="21845-109">createdDateTime</span></span>| <span data-ttu-id="21845-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="21845-110">DateTimeOffset</span></span> |<span data-ttu-id="21845-111">操作の開始時刻です。</span><span class="sxs-lookup"><span data-stu-id="21845-111">The start time of the operation.</span></span>|
|<span data-ttu-id="21845-112">error</span><span class="sxs-lookup"><span data-stu-id="21845-112">error</span></span>|[<span data-ttu-id="21845-113">onenoteOperationError</span><span class="sxs-lookup"><span data-stu-id="21845-113">onenoteOperationError</span></span>](onenoteoperationerror.md)|<span data-ttu-id="21845-114">操作によって返されるエラーです。</span><span class="sxs-lookup"><span data-stu-id="21845-114">The error returned by the operation.</span></span>|
|<span data-ttu-id="21845-115">id</span><span class="sxs-lookup"><span data-stu-id="21845-115">id</span></span>|<span data-ttu-id="21845-116">string</span><span class="sxs-lookup"><span data-stu-id="21845-116">string</span></span>|<span data-ttu-id="21845-117">操作 ID です。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="21845-117">The operation id. Read-only.</span></span>|
|<span data-ttu-id="21845-118">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="21845-118">lastActionDateTime</span></span>| <span data-ttu-id="21845-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="21845-119">DateTimeOffset</span></span> |<span data-ttu-id="21845-120">操作の最後の操作の時間です。</span><span class="sxs-lookup"><span data-stu-id="21845-120">The time of the last action of the operation.</span></span>|
|<span data-ttu-id="21845-121">resourceId</span><span class="sxs-lookup"><span data-stu-id="21845-121">resourceId</span></span>|<span data-ttu-id="21845-122">string</span><span class="sxs-lookup"><span data-stu-id="21845-122">string</span></span>|<span data-ttu-id="21845-123">リソース ID。</span><span class="sxs-lookup"><span data-stu-id="21845-123">The resource id.</span></span>|
|<span data-ttu-id="21845-124">resourceLocation</span><span class="sxs-lookup"><span data-stu-id="21845-124">resourceLocation</span></span>|<span data-ttu-id="21845-125">string</span><span class="sxs-lookup"><span data-stu-id="21845-125">string</span></span>|<span data-ttu-id="21845-p101">オブジェクトのリソース URI。たとえば、コピーしたページまたはセクションのリソース URI。</span><span class="sxs-lookup"><span data-stu-id="21845-p101">The resource URI for the object. For example, the resource URI for a copied page or section.</span></span> |
|<span data-ttu-id="21845-128">status</span><span class="sxs-lookup"><span data-stu-id="21845-128">status</span></span>|<span data-ttu-id="21845-129">string</span><span class="sxs-lookup"><span data-stu-id="21845-129">string</span></span>|<span data-ttu-id="21845-130">操作の現在の状態: `notstarted`、`running`、`completed`、`failed`</span><span class="sxs-lookup"><span data-stu-id="21845-130">The current status of the operation: `notstarted`, `running`, `completed`, `failed`</span></span> |
|<span data-ttu-id="21845-131">percentComplete</span><span class="sxs-lookup"><span data-stu-id="21845-131">percentComplete</span></span>|<span data-ttu-id="21845-132">string</span><span class="sxs-lookup"><span data-stu-id="21845-132">string</span></span>|<span data-ttu-id="21845-133">操作がまだ `running` の状態の場合の操作達成率。</span><span class="sxs-lookup"><span data-stu-id="21845-133">The operation percent complete if the operation is still in `running` status</span></span>

## <a name="relationships"></a><span data-ttu-id="21845-134">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="21845-134">Relationships</span></span>
<span data-ttu-id="21845-135">なし</span><span class="sxs-lookup"><span data-stu-id="21845-135">None</span></span>


## <a name="methods"></a><span data-ttu-id="21845-136">メソッド</span><span class="sxs-lookup"><span data-stu-id="21845-136">Methods</span></span>

| <span data-ttu-id="21845-137">メソッド</span><span class="sxs-lookup"><span data-stu-id="21845-137">Method</span></span>           | <span data-ttu-id="21845-138">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="21845-138">Return Type</span></span>    |<span data-ttu-id="21845-139">説明</span><span class="sxs-lookup"><span data-stu-id="21845-139">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="21845-140">操作の取得</span><span class="sxs-lookup"><span data-stu-id="21845-140">Get operation</span></span>](../api/onenoteoperation_get.md) | [<span data-ttu-id="21845-141">onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="21845-141">onenoteOperation</span></span>](onenoteoperation.md) |<span data-ttu-id="21845-142">操作の現在の状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="21845-142">Get the status of the operation.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
