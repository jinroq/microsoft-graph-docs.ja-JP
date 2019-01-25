---
title: plannerBucket リソースの種類
description: ) Office 365 のプランでの作業をします。 PlannerPlan に含まれ、plannerTasks のコレクションを持つことができます。
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
ms.openlocfilehash: 85cf30bc13b3236928e662807a144f81614adbd7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524458"
---
# <a name="plannerbucket-resource-type"></a><span data-ttu-id="7e9b3-104">plannerBucket リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7e9b3-104">plannerBucket resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7e9b3-p102">**PlannerBucket** リソースは、Office 365 の計画におけるタスクのバケット (または "カスタム列") を表します。これは [plannerPlan](plannerplan.md) に含まれており、[plannerTasks](plannertask.md) のコレクションを持ちます。</span><span class="sxs-lookup"><span data-stu-id="7e9b3-p102">The **plannerBucket** resource represents a bucket (or "custom column") for tasks in a plan in Office 365. It is contained in a [plannerPlan](plannerplan.md) and can have a collection of [plannerTasks](plannertask.md).</span></span>



## <a name="methods"></a><span data-ttu-id="7e9b3-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="7e9b3-107">Methods</span></span>

| <span data-ttu-id="7e9b3-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="7e9b3-108">Method</span></span>           | <span data-ttu-id="7e9b3-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="7e9b3-109">Return Type</span></span>    |<span data-ttu-id="7e9b3-110">説明</span><span class="sxs-lookup"><span data-stu-id="7e9b3-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7e9b3-111">Get plannerBucket</span><span class="sxs-lookup"><span data-stu-id="7e9b3-111">Get plannerBucket</span></span>](../api/plannerbucket-get.md) | [<span data-ttu-id="7e9b3-112">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="7e9b3-112">plannerBucket</span></span>](plannerbucket.md) |<span data-ttu-id="7e9b3-113">**plannerBucket** オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="7e9b3-113">Read properties and relationships of **plannerBucket** object.</span></span>|
|[<span data-ttu-id="7e9b3-114">List plannerTasks</span><span class="sxs-lookup"><span data-stu-id="7e9b3-114">List plannerTasks</span></span>](../api/plannerbucket-list-tasks.md) |<span data-ttu-id="7e9b3-115">[plannerTask](plannertask.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="7e9b3-115">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="7e9b3-116">**plannerTask** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="7e9b3-116">Get a **plannerTask** object collection.</span></span>|
|[<span data-ttu-id="7e9b3-117">Create</span><span class="sxs-lookup"><span data-stu-id="7e9b3-117">Create</span></span>](../api/planner-post-buckets.md) | [<span data-ttu-id="7e9b3-118">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="7e9b3-118">plannerBucket</span></span>](plannerbucket.md)   | <span data-ttu-id="7e9b3-119">新しい **plannerBucket** オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="7e9b3-119">Create a new **plannerBucket** object.</span></span> |
|[<span data-ttu-id="7e9b3-120">Update</span><span class="sxs-lookup"><span data-stu-id="7e9b3-120">Update</span></span>](../api/plannerbucket-update.md) | [<span data-ttu-id="7e9b3-121">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="7e9b3-121">plannerBucket</span></span>](plannerbucket.md)   |<span data-ttu-id="7e9b3-122">**plannerBucket** オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="7e9b3-122">Update **plannerBucket** object.</span></span> |
|[<span data-ttu-id="7e9b3-123">Delete</span><span class="sxs-lookup"><span data-stu-id="7e9b3-123">Delete</span></span>](../api/plannerbucket-delete.md) | <span data-ttu-id="7e9b3-124">なし</span><span class="sxs-lookup"><span data-stu-id="7e9b3-124">None</span></span> |<span data-ttu-id="7e9b3-125">**plannerBucket** オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="7e9b3-125">Delete **plannerBucket** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="7e9b3-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7e9b3-126">Properties</span></span>
| <span data-ttu-id="7e9b3-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7e9b3-127">Property</span></span>     | <span data-ttu-id="7e9b3-128">型</span><span class="sxs-lookup"><span data-stu-id="7e9b3-128">Type</span></span>   |<span data-ttu-id="7e9b3-129">説明</span><span class="sxs-lookup"><span data-stu-id="7e9b3-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7e9b3-130">id</span><span class="sxs-lookup"><span data-stu-id="7e9b3-130">id</span></span>|<span data-ttu-id="7e9b3-131">String</span><span class="sxs-lookup"><span data-stu-id="7e9b3-131">String</span></span>| <span data-ttu-id="7e9b3-132">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="7e9b3-132">Read-only.</span></span> <span data-ttu-id="7e9b3-133">バケットの ID です。</span><span class="sxs-lookup"><span data-stu-id="7e9b3-133">ID of the bucket.</span></span> <span data-ttu-id="7e9b3-134">28 の文字、大文字小文字を区別することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="7e9b3-134">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="7e9b3-135">サービスの[フォーマットの検証](tasks-identifiers-disclaimer.md)が行われます。</span><span class="sxs-lookup"><span data-stu-id="7e9b3-135">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="7e9b3-136">name</span><span class="sxs-lookup"><span data-stu-id="7e9b3-136">name</span></span>|<span data-ttu-id="7e9b3-137">String</span><span class="sxs-lookup"><span data-stu-id="7e9b3-137">String</span></span>|<span data-ttu-id="7e9b3-138">バケットの名前。</span><span class="sxs-lookup"><span data-stu-id="7e9b3-138">Name of the bucket.</span></span>|
|<span data-ttu-id="7e9b3-139">orderHint</span><span class="sxs-lookup"><span data-stu-id="7e9b3-139">orderHint</span></span>|<span data-ttu-id="7e9b3-140">String</span><span class="sxs-lookup"><span data-stu-id="7e9b3-140">String</span></span>|<span data-ttu-id="7e9b3-p104">リスト ビューでこの種類の項目の順序付けに使用するヒント。形式は[ここ](planner-order-hint-format.md)の説明に従って定義されます。</span><span class="sxs-lookup"><span data-stu-id="7e9b3-p104">Hint used to order items of this type in a list view. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="7e9b3-143">planId</span><span class="sxs-lookup"><span data-stu-id="7e9b3-143">planId</span></span>|<span data-ttu-id="7e9b3-144">String</span><span class="sxs-lookup"><span data-stu-id="7e9b3-144">String</span></span>|<span data-ttu-id="7e9b3-145">バケットが所属する計画の ID。</span><span class="sxs-lookup"><span data-stu-id="7e9b3-145">Plan ID to which the bucket belongs.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7e9b3-146">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7e9b3-146">Relationships</span></span>
| <span data-ttu-id="7e9b3-147">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7e9b3-147">Relationship</span></span> | <span data-ttu-id="7e9b3-148">型</span><span class="sxs-lookup"><span data-stu-id="7e9b3-148">Type</span></span>   |<span data-ttu-id="7e9b3-149">説明</span><span class="sxs-lookup"><span data-stu-id="7e9b3-149">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7e9b3-150">tasks</span><span class="sxs-lookup"><span data-stu-id="7e9b3-150">tasks</span></span>|<span data-ttu-id="7e9b3-151">[plannerTask](plannertask.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="7e9b3-151">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="7e9b3-p105">読み取り専用です。Null 許容型。バケットに含まれるタスクのコレクション。</span><span class="sxs-lookup"><span data-stu-id="7e9b3-p105">Read-only. Nullable. The collection of tasks in the bucket.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7e9b3-155">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7e9b3-155">JSON representation</span></span>
<span data-ttu-id="7e9b3-156">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7e9b3-156">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "plannerBucket resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerbucket.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
