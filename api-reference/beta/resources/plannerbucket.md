---
title: plannerBucket リソースの種類
description: ) Office 365 のプランでの作業をします。 PlannerPlan に含まれ、plannerTasks のコレクションを持つことができます。
author: TarkanSevilmis
ms.openlocfilehash: e3b09e50c62842d5b3f60206da49e9596648c565
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27311866"
---
# <a name="plannerbucket-resource-type"></a><span data-ttu-id="db666-104">plannerBucket リソースの種類</span><span class="sxs-lookup"><span data-stu-id="db666-104">plannerBucket resource type</span></span>

> <span data-ttu-id="db666-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="db666-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="db666-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="db666-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="db666-p103">**PlannerBucket** リソースは、Office 365 の計画におけるタスクのバケット (または "カスタム列") を表します。これは [plannerPlan](plannerplan.md) に含まれており、[plannerTasks](plannertask.md) のコレクションを持ちます。</span><span class="sxs-lookup"><span data-stu-id="db666-p103">The **plannerBucket** resource represents a bucket (or "custom column") for tasks in a plan in Office 365. It is contained in a [plannerPlan](plannerplan.md) and can have a collection of [plannerTasks](plannertask.md).</span></span>



## <a name="methods"></a><span data-ttu-id="db666-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="db666-109">Methods</span></span>

| <span data-ttu-id="db666-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="db666-110">Method</span></span>           | <span data-ttu-id="db666-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="db666-111">Return Type</span></span>    |<span data-ttu-id="db666-112">説明</span><span class="sxs-lookup"><span data-stu-id="db666-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="db666-113">Get plannerBucket</span><span class="sxs-lookup"><span data-stu-id="db666-113">Get plannerBucket</span></span>](../api/plannerbucket-get.md) | [<span data-ttu-id="db666-114">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="db666-114">plannerBucket</span></span>](plannerbucket.md) |<span data-ttu-id="db666-115">**plannerBucket** オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="db666-115">Read properties and relationships of **plannerBucket** object.</span></span>|
|[<span data-ttu-id="db666-116">List plannerTasks</span><span class="sxs-lookup"><span data-stu-id="db666-116">List plannerTasks</span></span>](../api/plannerbucket-list-tasks.md) |<span data-ttu-id="db666-117">[plannerTask](plannertask.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="db666-117">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="db666-118">**plannerTask** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="db666-118">Get a **plannerTask** object collection.</span></span>|
|[<span data-ttu-id="db666-119">Create</span><span class="sxs-lookup"><span data-stu-id="db666-119">Create</span></span>](../api/planner-post-buckets.md) | [<span data-ttu-id="db666-120">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="db666-120">plannerBucket</span></span>](plannerbucket.md)   | <span data-ttu-id="db666-121">新しい **plannerBucket** オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="db666-121">Create a new **plannerBucket** object.</span></span> |
|[<span data-ttu-id="db666-122">Update</span><span class="sxs-lookup"><span data-stu-id="db666-122">Update</span></span>](../api/plannerbucket-update.md) | [<span data-ttu-id="db666-123">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="db666-123">plannerBucket</span></span>](plannerbucket.md)   |<span data-ttu-id="db666-124">**plannerBucket** オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="db666-124">Update **plannerBucket** object.</span></span> |
|[<span data-ttu-id="db666-125">Delete</span><span class="sxs-lookup"><span data-stu-id="db666-125">Delete</span></span>](../api/plannerbucket-delete.md) | <span data-ttu-id="db666-126">なし</span><span class="sxs-lookup"><span data-stu-id="db666-126">None</span></span> |<span data-ttu-id="db666-127">**plannerBucket** オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="db666-127">Delete **plannerBucket** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="db666-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="db666-128">Properties</span></span>
| <span data-ttu-id="db666-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="db666-129">Property</span></span>     | <span data-ttu-id="db666-130">種類</span><span class="sxs-lookup"><span data-stu-id="db666-130">Type</span></span>   |<span data-ttu-id="db666-131">説明</span><span class="sxs-lookup"><span data-stu-id="db666-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="db666-132">ID</span><span class="sxs-lookup"><span data-stu-id="db666-132">id</span></span>|<span data-ttu-id="db666-133">String</span><span class="sxs-lookup"><span data-stu-id="db666-133">String</span></span>| <span data-ttu-id="db666-134">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="db666-134">Read-only.</span></span> <span data-ttu-id="db666-135">バケットの ID です。</span><span class="sxs-lookup"><span data-stu-id="db666-135">ID of the bucket.</span></span> <span data-ttu-id="db666-136">28 の文字、大文字小文字を区別することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="db666-136">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="db666-137">サービスの[フォーマットの検証](tasks-identifiers-disclaimer.md)が行われます。</span><span class="sxs-lookup"><span data-stu-id="db666-137">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="db666-138">名前</span><span class="sxs-lookup"><span data-stu-id="db666-138">name</span></span>|<span data-ttu-id="db666-139">String</span><span class="sxs-lookup"><span data-stu-id="db666-139">String</span></span>|<span data-ttu-id="db666-140">バケットの名前。</span><span class="sxs-lookup"><span data-stu-id="db666-140">Name of the bucket.</span></span>|
|<span data-ttu-id="db666-141">orderHint</span><span class="sxs-lookup"><span data-stu-id="db666-141">orderHint</span></span>|<span data-ttu-id="db666-142">String</span><span class="sxs-lookup"><span data-stu-id="db666-142">String</span></span>|<span data-ttu-id="db666-p105">リスト ビューでこの種類の項目の順序付けに使用するヒント。形式は[ここ](planner-order-hint-format.md)の説明に従って定義されます。</span><span class="sxs-lookup"><span data-stu-id="db666-p105">Hint used to order items of this type in a list view. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="db666-145">planId</span><span class="sxs-lookup"><span data-stu-id="db666-145">planId</span></span>|<span data-ttu-id="db666-146">String</span><span class="sxs-lookup"><span data-stu-id="db666-146">String</span></span>|<span data-ttu-id="db666-147">バケットが所属する計画の ID。</span><span class="sxs-lookup"><span data-stu-id="db666-147">Plan ID to which the bucket belongs.</span></span>|

## <a name="relationships"></a><span data-ttu-id="db666-148">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="db666-148">Relationships</span></span>
| <span data-ttu-id="db666-149">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="db666-149">Relationship</span></span> | <span data-ttu-id="db666-150">型</span><span class="sxs-lookup"><span data-stu-id="db666-150">Type</span></span>   |<span data-ttu-id="db666-151">説明</span><span class="sxs-lookup"><span data-stu-id="db666-151">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="db666-152">tasks</span><span class="sxs-lookup"><span data-stu-id="db666-152">tasks</span></span>|<span data-ttu-id="db666-153">[plannerTask](plannertask.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="db666-153">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="db666-p106">読み取り専用です。Null 許容型。バケットに含まれるタスクのコレクション。</span><span class="sxs-lookup"><span data-stu-id="db666-p106">Read-only. Nullable. The collection of tasks in the bucket.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="db666-157">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="db666-157">JSON representation</span></span>
<span data-ttu-id="db666-158">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="db666-158">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
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