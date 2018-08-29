# <a name="plannergroup-resource-type"></a><span data-ttu-id="ed2eb-101">plannerGroup リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ed2eb-101">plannerGroup resource type</span></span>

<span data-ttu-id="ed2eb-p101">**plannerGroup** リソースは、[group](group.md) の Planner リソースへのアクセスを提供します。使用可能なプロパティは含まれていません。</span><span class="sxs-lookup"><span data-stu-id="ed2eb-p101">The **plannerGroup** resource provides access to Planner resources for a [group](group.md). It doesn't contain any usable properties.</span></span>

## <a name="methods"></a><span data-ttu-id="ed2eb-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="ed2eb-104">Methods</span></span>

| <span data-ttu-id="ed2eb-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="ed2eb-105">Method</span></span>           | <span data-ttu-id="ed2eb-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ed2eb-106">Return Type</span></span>    |<span data-ttu-id="ed2eb-107">説明</span><span class="sxs-lookup"><span data-stu-id="ed2eb-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ed2eb-108">plans を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="ed2eb-108">List plans</span></span>](../api/plannergroup_list_plans.md) |<span data-ttu-id="ed2eb-109">[plannerPlan](plannerplan.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ed2eb-109">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="ed2eb-110">**plannerPlan** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="ed2eb-110">Get a **plannerPlan** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="ed2eb-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ed2eb-111">Properties</span></span>
| <span data-ttu-id="ed2eb-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ed2eb-112">Property</span></span>     | <span data-ttu-id="ed2eb-113">タイプ</span><span class="sxs-lookup"><span data-stu-id="ed2eb-113">Type</span></span>   |<span data-ttu-id="ed2eb-114">説明</span><span class="sxs-lookup"><span data-stu-id="ed2eb-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ed2eb-115">id</span><span class="sxs-lookup"><span data-stu-id="ed2eb-115">id</span></span>|<span data-ttu-id="ed2eb-116">文字列</span><span class="sxs-lookup"><span data-stu-id="ed2eb-116">String</span></span>| <span data-ttu-id="ed2eb-p102">読み取り専用です。**plannerGroup** の識別子</span><span class="sxs-lookup"><span data-stu-id="ed2eb-p102">Read-only. Identifier of the **plannerGroup**</span></span>|

## <a name="relationships"></a><span data-ttu-id="ed2eb-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ed2eb-119">Relationships</span></span>
| <span data-ttu-id="ed2eb-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ed2eb-120">Relationship</span></span> | <span data-ttu-id="ed2eb-121">型</span><span class="sxs-lookup"><span data-stu-id="ed2eb-121">Type</span></span>   |<span data-ttu-id="ed2eb-122">説明</span><span class="sxs-lookup"><span data-stu-id="ed2eb-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ed2eb-123">plans</span><span class="sxs-lookup"><span data-stu-id="ed2eb-123">plans</span></span>|<span data-ttu-id="ed2eb-124">[plannerPlan](plannerplan.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ed2eb-124">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="ed2eb-p103">読み取り専用です。Null 許容型。グループが所有する [plannerPlans](plannerplan.md) を返します。</span><span class="sxs-lookup"><span data-stu-id="ed2eb-p103">Read-only. Nullable. Returns the [plannerPlans](plannerplan.md) owned by the group.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ed2eb-128">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ed2eb-128">JSON representation</span></span>
<span data-ttu-id="ed2eb-129">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ed2eb-129">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerGroup"
}-->

```json
{
  "id": "String (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->