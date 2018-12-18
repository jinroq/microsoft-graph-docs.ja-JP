---
title: plannerBucket リソースの種類
description: ) Office 365 のプランでの作業をします。 PlannerPlan に含まれ、plannerTasks のコレクションを持つことができます。
author: TarkanSevilmis
ms.openlocfilehash: 09c9fab569a819f0545e5c851da12be98b45b150
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27331445"
---
# <a name="plannerbucket-resource-type"></a><span data-ttu-id="93fea-104">plannerBucket リソースの種類</span><span class="sxs-lookup"><span data-stu-id="93fea-104">plannerBucket resource type</span></span>

<span data-ttu-id="93fea-p102">**PlannerBucket** リソースは、Office 365 の計画におけるタスクのバケット (または "カスタム列") を表します。これは [plannerPlan](plannerplan.md) に含まれており、[plannerTasks](plannertask.md) のコレクションを持ちます。</span><span class="sxs-lookup"><span data-stu-id="93fea-p102">The **plannerBucket** resource represents a bucket (or "custom column") for tasks in a plan in Office 365. It is contained in a [plannerPlan](plannerplan.md) and can have a collection of [plannerTasks](plannertask.md).</span></span>



## <a name="methods"></a><span data-ttu-id="93fea-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="93fea-107">Methods</span></span>

| <span data-ttu-id="93fea-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="93fea-108">Method</span></span>           | <span data-ttu-id="93fea-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="93fea-109">Return Type</span></span>    |<span data-ttu-id="93fea-110">説明</span><span class="sxs-lookup"><span data-stu-id="93fea-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="93fea-111">Get plannerBucket</span><span class="sxs-lookup"><span data-stu-id="93fea-111">Get plannerBucket</span></span>](../api/plannerbucket-get.md) | [<span data-ttu-id="93fea-112">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="93fea-112">plannerBucket</span></span>](plannerbucket.md) |<span data-ttu-id="93fea-113">**plannerBucket** オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="93fea-113">Read properties and relationships of **plannerBucket** object.</span></span>|
|[<span data-ttu-id="93fea-114">List plannerTasks</span><span class="sxs-lookup"><span data-stu-id="93fea-114">List plannerTasks</span></span>](../api/plannerbucket-list-tasks.md) |<span data-ttu-id="93fea-115">[plannerTask](plannertask.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="93fea-115">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="93fea-116">**plannerTask** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="93fea-116">Get a **plannerTask** object collection.</span></span>|
|[<span data-ttu-id="93fea-117">Create</span><span class="sxs-lookup"><span data-stu-id="93fea-117">Create</span></span>](../api/planner-post-buckets.md) | [<span data-ttu-id="93fea-118">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="93fea-118">plannerBucket</span></span>](plannerbucket.md)   | <span data-ttu-id="93fea-119">新しい **plannerBucket** オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="93fea-119">Create a new **plannerBucket** object.</span></span> |
|[<span data-ttu-id="93fea-120">Update</span><span class="sxs-lookup"><span data-stu-id="93fea-120">Update</span></span>](../api/plannerbucket-update.md) | [<span data-ttu-id="93fea-121">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="93fea-121">plannerBucket</span></span>](plannerbucket.md)   |<span data-ttu-id="93fea-122">**plannerBucket** オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="93fea-122">Update **plannerBucket** object.</span></span> |
|[<span data-ttu-id="93fea-123">Delete</span><span class="sxs-lookup"><span data-stu-id="93fea-123">Delete</span></span>](../api/plannerbucket-delete.md) | <span data-ttu-id="93fea-124">なし</span><span class="sxs-lookup"><span data-stu-id="93fea-124">None</span></span> |<span data-ttu-id="93fea-125">**plannerBucket** オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="93fea-125">Delete **plannerBucket** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="93fea-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="93fea-126">Properties</span></span>
| <span data-ttu-id="93fea-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="93fea-127">Property</span></span>     | <span data-ttu-id="93fea-128">種類</span><span class="sxs-lookup"><span data-stu-id="93fea-128">Type</span></span>   |<span data-ttu-id="93fea-129">説明</span><span class="sxs-lookup"><span data-stu-id="93fea-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="93fea-130">ID</span><span class="sxs-lookup"><span data-stu-id="93fea-130">id</span></span>|<span data-ttu-id="93fea-131">String</span><span class="sxs-lookup"><span data-stu-id="93fea-131">String</span></span>| <span data-ttu-id="93fea-132">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="93fea-132">Read-only.</span></span> <span data-ttu-id="93fea-133">バケットの ID です。</span><span class="sxs-lookup"><span data-stu-id="93fea-133">ID of the bucket.</span></span> <span data-ttu-id="93fea-134">28 の文字、大文字小文字を区別することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="93fea-134">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="93fea-135">サービスの[フォーマットの検証](planner-identifiers-disclaimer.md)が行われます。</span><span class="sxs-lookup"><span data-stu-id="93fea-135">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="93fea-136">名前</span><span class="sxs-lookup"><span data-stu-id="93fea-136">name</span></span>|<span data-ttu-id="93fea-137">String</span><span class="sxs-lookup"><span data-stu-id="93fea-137">String</span></span>|<span data-ttu-id="93fea-138">バケットの名前。</span><span class="sxs-lookup"><span data-stu-id="93fea-138">Name of the bucket.</span></span>|
|<span data-ttu-id="93fea-139">orderHint</span><span class="sxs-lookup"><span data-stu-id="93fea-139">orderHint</span></span>|<span data-ttu-id="93fea-140">String</span><span class="sxs-lookup"><span data-stu-id="93fea-140">String</span></span>|<span data-ttu-id="93fea-p104">リスト ビューでこの種類の項目の順序付けに使用するヒント。形式は[ここ](planner-order-hint-format.md)の説明に従って定義されます。</span><span class="sxs-lookup"><span data-stu-id="93fea-p104">Hint used to order items of this type in a list view. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="93fea-143">planId</span><span class="sxs-lookup"><span data-stu-id="93fea-143">planId</span></span>|<span data-ttu-id="93fea-144">String</span><span class="sxs-lookup"><span data-stu-id="93fea-144">String</span></span>|<span data-ttu-id="93fea-145">バケットが所属する計画の ID。</span><span class="sxs-lookup"><span data-stu-id="93fea-145">Plan ID to which the bucket belongs.</span></span>|

## <a name="relationships"></a><span data-ttu-id="93fea-146">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="93fea-146">Relationships</span></span>
| <span data-ttu-id="93fea-147">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="93fea-147">Relationship</span></span> | <span data-ttu-id="93fea-148">型</span><span class="sxs-lookup"><span data-stu-id="93fea-148">Type</span></span>   |<span data-ttu-id="93fea-149">説明</span><span class="sxs-lookup"><span data-stu-id="93fea-149">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="93fea-150">tasks</span><span class="sxs-lookup"><span data-stu-id="93fea-150">tasks</span></span>|<span data-ttu-id="93fea-151">[plannerTask](plannertask.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="93fea-151">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="93fea-p105">読み取り専用です。Null 許容型。バケットに含まれるタスクのコレクション。</span><span class="sxs-lookup"><span data-stu-id="93fea-p105">Read-only. Nullable. The collection of tasks in the bucket.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="93fea-155">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="93fea-155">JSON representation</span></span>
<span data-ttu-id="93fea-156">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="93fea-156">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerBucket"
}-->

```json
{
  "id": "String (identifier)",
  "name": "String",
  "orderHint": "String",
  "planId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerBucket resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->