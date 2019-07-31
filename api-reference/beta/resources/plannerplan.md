---
title: plannerPlan リソースの種類
description: '**plannerPlan** リソースは、Office 365 での計画を表します。 計画は group によって所有され、plannerTasks のコレクションが含まれています。 plannerBuckets のコレクションを含む場合もあります。 各プランオブジェクトには details オブジェクトがあり、プランに関する詳細情報を含めることができます。 グループ、計画、タスク間のリレーションシップの詳細については、「Planner」を参照してください。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 658bcbbaf8431b65565ecebd03a014776be840e9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965946"
---
# <a name="plannerplan-resource-type"></a><span data-ttu-id="7dce8-107">plannerPlan リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7dce8-107">plannerPlan resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7dce8-108">**plannerPlan** リソースは、Office 365 での計画を表します。</span><span class="sxs-lookup"><span data-stu-id="7dce8-108">The **plannerPlan** resource represents a plan in Office 365.</span></span> <span data-ttu-id="7dce8-109">計画は [group](group.md) によって所有され、[plannerTasks](plannertask.md) のコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="7dce8-109">A plan can be owned by a [group](group.md) and contains a collection of [plannerTasks](plannertask.md).</span></span> <span data-ttu-id="7dce8-110">[plannerBuckets](plannerbucket.md) のコレクションを含む場合もあります。</span><span class="sxs-lookup"><span data-stu-id="7dce8-110">It can also have a collection of [plannerBuckets](plannerbucket.md).</span></span> <span data-ttu-id="7dce8-111">各プランオブジェクトには[details](plannerplandetails.md)オブジェクトがあり、プランに関する詳細情報を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="7dce8-111">Each plan object has a [details](plannerplandetails.md) object which can contain more information about the plan.</span></span> <span data-ttu-id="7dce8-112">グループ、計画、タスク間のリレーションシップの詳細については、「[Planner](planner-overview.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7dce8-112">For more information about the relationships between groups, plans, and tasks, see [Planner](planner-overview.md).</span></span>



## <a name="methods"></a><span data-ttu-id="7dce8-113">メソッド</span><span class="sxs-lookup"><span data-stu-id="7dce8-113">Methods</span></span>

| <span data-ttu-id="7dce8-114">メソッド</span><span class="sxs-lookup"><span data-stu-id="7dce8-114">Method</span></span>           | <span data-ttu-id="7dce8-115">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="7dce8-115">Return Type</span></span>    |<span data-ttu-id="7dce8-116">説明</span><span class="sxs-lookup"><span data-stu-id="7dce8-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7dce8-117">Get plannerPlan</span><span class="sxs-lookup"><span data-stu-id="7dce8-117">Get plannerPlan</span></span>](../api/plannerplan-get.md) | [<span data-ttu-id="7dce8-118">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="7dce8-118">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="7dce8-119">**plannerPlan** オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="7dce8-119">Read properties and relationships of **plannerPlan** object.</span></span>|
|[<span data-ttu-id="7dce8-120">List buckets</span><span class="sxs-lookup"><span data-stu-id="7dce8-120">List buckets</span></span>](../api/plannerplan-list-buckets.md) |<span data-ttu-id="7dce8-121">[plannerBucket](plannerbucket.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="7dce8-121">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="7dce8-122">**plannerBucket** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="7dce8-122">Get a **plannerBucket** object collection.</span></span>|
|[<span data-ttu-id="7dce8-123">List tasks</span><span class="sxs-lookup"><span data-stu-id="7dce8-123">List tasks</span></span>](../api/plannerplan-list-tasks.md) |<span data-ttu-id="7dce8-124">[plannerTask](plannertask.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="7dce8-124">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="7dce8-125">**plannerTask** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="7dce8-125">Get a **plannerTask** object collection.</span></span>|
|[<span data-ttu-id="7dce8-126">Update</span><span class="sxs-lookup"><span data-stu-id="7dce8-126">Update</span></span>](../api/plannerplan-update.md) | [<span data-ttu-id="7dce8-127">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="7dce8-127">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="7dce8-128">**plannerPlan** オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="7dce8-128">Update **plannerPlan** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="7dce8-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7dce8-129">Properties</span></span>
| <span data-ttu-id="7dce8-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7dce8-130">Property</span></span>     | <span data-ttu-id="7dce8-131">型</span><span class="sxs-lookup"><span data-stu-id="7dce8-131">Type</span></span>   |<span data-ttu-id="7dce8-132">説明</span><span class="sxs-lookup"><span data-stu-id="7dce8-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7dce8-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7dce8-133">createdDateTime</span></span>|<span data-ttu-id="7dce8-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7dce8-134">DateTimeOffset</span></span>|<span data-ttu-id="7dce8-p103">読み取り専用。計画の作成日時。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="7dce8-p103">Read-only. Date and time at which the plan is created. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="7dce8-139">id</span><span class="sxs-lookup"><span data-stu-id="7dce8-139">id</span></span>|<span data-ttu-id="7dce8-140">String</span><span class="sxs-lookup"><span data-stu-id="7dce8-140">String</span></span>| <span data-ttu-id="7dce8-141">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="7dce8-141">Read-only.</span></span> <span data-ttu-id="7dce8-142">計画の ID。</span><span class="sxs-lookup"><span data-stu-id="7dce8-142">ID of the plan.</span></span> <span data-ttu-id="7dce8-143">28 文字長で、大文字と小文字の区別があります。</span><span class="sxs-lookup"><span data-stu-id="7dce8-143">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="7dce8-144">[書式検証](tasks-identifiers-disclaimer.md)はサービスによって行われます。</span><span class="sxs-lookup"><span data-stu-id="7dce8-144">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="7dce8-145">owner</span><span class="sxs-lookup"><span data-stu-id="7dce8-145">owner</span></span>|<span data-ttu-id="7dce8-146">String</span><span class="sxs-lookup"><span data-stu-id="7dce8-146">String</span></span>|<span data-ttu-id="7dce8-147">計画を所有している [Group](group.md) の ID。</span><span class="sxs-lookup"><span data-stu-id="7dce8-147">ID of the [Group](group.md) that owns the plan.</span></span> <span data-ttu-id="7dce8-148">このフィールドを設定するためには、有効なグループが存在していなければなりません。</span><span class="sxs-lookup"><span data-stu-id="7dce8-148">A valid group must exist before this field can be set.</span></span> <span data-ttu-id="7dce8-149">設定すると、このプロパティを更新することはできません。</span><span class="sxs-lookup"><span data-stu-id="7dce8-149">After it is set, this property can’t be updated.</span></span>|
|<span data-ttu-id="7dce8-150">title</span><span class="sxs-lookup"><span data-stu-id="7dce8-150">title</span></span>|<span data-ttu-id="7dce8-151">String</span><span class="sxs-lookup"><span data-stu-id="7dce8-151">String</span></span>|<span data-ttu-id="7dce8-152">必須。</span><span class="sxs-lookup"><span data-stu-id="7dce8-152">Required.</span></span> <span data-ttu-id="7dce8-153">計画のタイトル。</span><span class="sxs-lookup"><span data-stu-id="7dce8-153">Title of the plan.</span></span>|
|<span data-ttu-id="7dce8-154">createdBy</span><span class="sxs-lookup"><span data-stu-id="7dce8-154">createdBy</span></span>|[<span data-ttu-id="7dce8-155">identitySet</span><span class="sxs-lookup"><span data-stu-id="7dce8-155">identitySet</span></span>](identityset.md)|<span data-ttu-id="7dce8-156">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="7dce8-156">Read-only.</span></span> <span data-ttu-id="7dce8-157">計画を作成したユーザー。</span><span class="sxs-lookup"><span data-stu-id="7dce8-157">The user who created the plan.</span></span>|
|<span data-ttu-id="7dce8-158">状況</span><span class="sxs-lookup"><span data-stu-id="7dce8-158">contexts</span></span>|[<span data-ttu-id="7dce8-159">plannerPlanContextCollection</span><span class="sxs-lookup"><span data-stu-id="7dce8-159">plannerPlanContextCollection</span></span>](plannerplancontextcollection.md)| <span data-ttu-id="7dce8-160">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="7dce8-160">Read-only.</span></span> <span data-ttu-id="7dce8-161">このプランが使用される追加のユーザーエクスペリエンス。このプランは、[コンテキスト](plannerplancontext.md)エントリをプランとして表現します。</span><span class="sxs-lookup"><span data-stu-id="7dce8-161">Additional user experiences in which this plan is used, represented as [plannerPlanContext](plannerplancontext.md) entries.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7dce8-162">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7dce8-162">Relationships</span></span>
| <span data-ttu-id="7dce8-163">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7dce8-163">Relationship</span></span> | <span data-ttu-id="7dce8-164">型</span><span class="sxs-lookup"><span data-stu-id="7dce8-164">Type</span></span>   |<span data-ttu-id="7dce8-165">説明</span><span class="sxs-lookup"><span data-stu-id="7dce8-165">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7dce8-166">buckets</span><span class="sxs-lookup"><span data-stu-id="7dce8-166">buckets</span></span>|<span data-ttu-id="7dce8-167">[plannerBucket](plannerbucket.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="7dce8-167">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="7dce8-p109">読み取り専用です。Null 許容型。計画に含まれるバケットのコレクション。</span><span class="sxs-lookup"><span data-stu-id="7dce8-p109">Read-only. Nullable. Collection of buckets in the plan.</span></span>|
|<span data-ttu-id="7dce8-171">詳細</span><span class="sxs-lookup"><span data-stu-id="7dce8-171">details</span></span>|[<span data-ttu-id="7dce8-172">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="7dce8-172">plannerPlanDetails</span></span>](plannerplandetails.md)| <span data-ttu-id="7dce8-173">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="7dce8-173">Read-only.</span></span> <span data-ttu-id="7dce8-174">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="7dce8-174">Nullable.</span></span> <span data-ttu-id="7dce8-175">計画に関する追加の詳細。</span><span class="sxs-lookup"><span data-stu-id="7dce8-175">Additional details about the plan.</span></span>|
|<span data-ttu-id="7dce8-176">tasks</span><span class="sxs-lookup"><span data-stu-id="7dce8-176">tasks</span></span>|<span data-ttu-id="7dce8-177">[plannerTask](plannertask.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="7dce8-177">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="7dce8-178">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="7dce8-178">Read-only.</span></span> <span data-ttu-id="7dce8-179">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="7dce8-179">Nullable.</span></span> <span data-ttu-id="7dce8-180">計画に含まれるタスクのコレクション。</span><span class="sxs-lookup"><span data-stu-id="7dce8-180">Collection of tasks in the plan.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7dce8-181">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7dce8-181">JSON representation</span></span>

<span data-ttu-id="7dce8-182">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7dce8-182">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",  
  "@odata.type": "microsoft.graph.plannerPlan"
}-->

```json
{
  "contexts": {
    "48#19%3Ad128c63941b24733951ea7defd81e550%40thread%2Eskype19%3Ad128c63941b24733951ea7defd81e550%40thread%2Eskype": {
        "@odata.type": "#microsoft.graph.plannerPlanContext",
        "associationType": "Board",
        "createdDateTime": "2015-10-14T00:57:28.4698344Z",
        "displayNameSegments": [
            "Finance Team",
            "Budget Plans"
        ],
        "ownerAppId": "5e3ce6c0-2b1f-4285-8d4b-75ee78787346"
    }
  },
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "owner": "String",
  "title": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerPlan resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
