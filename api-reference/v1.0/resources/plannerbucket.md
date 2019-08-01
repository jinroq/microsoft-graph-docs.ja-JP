---
title: Plan/バケットリソースの種類
description: ) Office 365 のプラン内のタスク。 これはプランに含まれており、plan グループのタスクのコレクションを持つことができます。
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: b6810a62ecab5209ca1c17aa7f3ca9e4753a50a9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035324"
---
# <a name="plannerbucket-resource-type"></a><span data-ttu-id="8d15c-104">Plan/バケットリソースの種類</span><span class="sxs-lookup"><span data-stu-id="8d15c-104">plannerBucket resource type</span></span>

<span data-ttu-id="8d15c-105">**Plan**は、Office 365 のプランに含まれるタスクのバケット (または "ユーザー設定列") を表します。</span><span class="sxs-lookup"><span data-stu-id="8d15c-105">The **plannerBucket** resource represents a bucket (or "custom column") for tasks in a plan in Office 365.</span></span> <span data-ttu-id="8d15c-106">これは[プラン](plannerplan.md)に含まれており、plan グループの[タスク](plannertask.md)のコレクションを持つことができます。</span><span class="sxs-lookup"><span data-stu-id="8d15c-106">It is contained in a [plannerPlan](plannerplan.md) and can have a collection of [plannerTasks](plannertask.md).</span></span>



## <a name="methods"></a><span data-ttu-id="8d15c-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="8d15c-107">Methods</span></span>

| <span data-ttu-id="8d15c-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="8d15c-108">Method</span></span>           | <span data-ttu-id="8d15c-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="8d15c-109">Return Type</span></span>    |<span data-ttu-id="8d15c-110">説明</span><span class="sxs-lookup"><span data-stu-id="8d15c-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8d15c-111">Get plannerBucket</span><span class="sxs-lookup"><span data-stu-id="8d15c-111">Get plannerBucket</span></span>](../api/plannerbucket-get.md) | [<span data-ttu-id="8d15c-112">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="8d15c-112">plannerBucket</span></span>](plannerbucket.md) |<span data-ttu-id="8d15c-113">**プラン**オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="8d15c-113">Read properties and relationships of **plannerBucket** object.</span></span>|
|[<span data-ttu-id="8d15c-114">plannerTasks を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="8d15c-114">List plannerTasks</span></span>](../api/plannerbucket-list-tasks.md) |<span data-ttu-id="8d15c-115">[plannerTask](plannertask.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="8d15c-115">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="8d15c-116">**plannerTask** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="8d15c-116">Get a **plannerTask** object collection.</span></span>|
|[<span data-ttu-id="8d15c-117">Create</span><span class="sxs-lookup"><span data-stu-id="8d15c-117">Create</span></span>](../api/planner-post-buckets.md) | [<span data-ttu-id="8d15c-118">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="8d15c-118">plannerBucket</span></span>](plannerbucket.md)   | <span data-ttu-id="8d15c-119">新しい**プラン**のオブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="8d15c-119">Create a new **plannerBucket** object.</span></span> |
|[<span data-ttu-id="8d15c-120">Update</span><span class="sxs-lookup"><span data-stu-id="8d15c-120">Update</span></span>](../api/plannerbucket-update.md) | [<span data-ttu-id="8d15c-121">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="8d15c-121">plannerBucket</span></span>](plannerbucket.md)   |<span data-ttu-id="8d15c-122">**プラン**オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="8d15c-122">Update **plannerBucket** object.</span></span> |
|[<span data-ttu-id="8d15c-123">Delete</span><span class="sxs-lookup"><span data-stu-id="8d15c-123">Delete</span></span>](../api/plannerbucket-delete.md) | <span data-ttu-id="8d15c-124">None</span><span class="sxs-lookup"><span data-stu-id="8d15c-124">None</span></span> |<span data-ttu-id="8d15c-125">**プラン**オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="8d15c-125">Delete **plannerBucket** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="8d15c-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8d15c-126">Properties</span></span>
| <span data-ttu-id="8d15c-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8d15c-127">Property</span></span>     | <span data-ttu-id="8d15c-128">型</span><span class="sxs-lookup"><span data-stu-id="8d15c-128">Type</span></span>   |<span data-ttu-id="8d15c-129">説明</span><span class="sxs-lookup"><span data-stu-id="8d15c-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8d15c-130">id</span><span class="sxs-lookup"><span data-stu-id="8d15c-130">id</span></span>|<span data-ttu-id="8d15c-131">文字列</span><span class="sxs-lookup"><span data-stu-id="8d15c-131">String</span></span>| <span data-ttu-id="8d15c-132">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="8d15c-132">Read-only.</span></span> <span data-ttu-id="8d15c-133">バケットの ID。</span><span class="sxs-lookup"><span data-stu-id="8d15c-133">ID of the bucket.</span></span> <span data-ttu-id="8d15c-134">28 文字長で、大文字と小文字の区別があります。</span><span class="sxs-lookup"><span data-stu-id="8d15c-134">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="8d15c-135">[書式検証](planner-identifiers-disclaimer.md)はサービスによって行われます。</span><span class="sxs-lookup"><span data-stu-id="8d15c-135">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="8d15c-136">name</span><span class="sxs-lookup"><span data-stu-id="8d15c-136">name</span></span>|<span data-ttu-id="8d15c-137">String</span><span class="sxs-lookup"><span data-stu-id="8d15c-137">String</span></span>|<span data-ttu-id="8d15c-138">バケットの名前。</span><span class="sxs-lookup"><span data-stu-id="8d15c-138">Name of the bucket.</span></span>|
|<span data-ttu-id="8d15c-139">orderHint</span><span class="sxs-lookup"><span data-stu-id="8d15c-139">orderHint</span></span>|<span data-ttu-id="8d15c-140">String</span><span class="sxs-lookup"><span data-stu-id="8d15c-140">String</span></span>|<span data-ttu-id="8d15c-p104">リスト ビューでこの種類の項目の順序付けに使用するヒント。形式は[ここ](planner-order-hint-format.md)の説明に従って定義されます。</span><span class="sxs-lookup"><span data-stu-id="8d15c-p104">Hint used to order items of this type in a list view. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="8d15c-143">planId</span><span class="sxs-lookup"><span data-stu-id="8d15c-143">planId</span></span>|<span data-ttu-id="8d15c-144">String</span><span class="sxs-lookup"><span data-stu-id="8d15c-144">String</span></span>|<span data-ttu-id="8d15c-145">バケットが属している計画 ID。</span><span class="sxs-lookup"><span data-stu-id="8d15c-145">Plan ID to which the bucket belongs.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8d15c-146">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8d15c-146">Relationships</span></span>
| <span data-ttu-id="8d15c-147">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8d15c-147">Relationship</span></span> | <span data-ttu-id="8d15c-148">型</span><span class="sxs-lookup"><span data-stu-id="8d15c-148">Type</span></span>   |<span data-ttu-id="8d15c-149">説明</span><span class="sxs-lookup"><span data-stu-id="8d15c-149">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8d15c-150">tasks</span><span class="sxs-lookup"><span data-stu-id="8d15c-150">tasks</span></span>|<span data-ttu-id="8d15c-151">[plannerTask](plannertask.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="8d15c-151">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="8d15c-152">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="8d15c-152">Read-only.</span></span> <span data-ttu-id="8d15c-153">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="8d15c-153">Nullable.</span></span> <span data-ttu-id="8d15c-154">バケット内のタスクのコレクション。</span><span class="sxs-lookup"><span data-stu-id="8d15c-154">The collection of tasks in the bucket.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8d15c-155">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8d15c-155">JSON representation</span></span>
<span data-ttu-id="8d15c-156">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8d15c-156">Here is a JSON representation of the resource.</span></span>

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
