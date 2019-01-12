---
title: plannerPlan リソースの種類
description: '**PlannerPlan**リソースでは、Office 365 のプランを表します。 計画は、グループが所有することができ、plannerTasks のコレクションが含まれています。 PlannerBuckets のコレクションもあります。 各プラン オブジェクトには、計画の詳細を含めることができる詳細オブジェクトがあります。 グループ、計画、およびタスク間の関係の詳細については、プランナーを参照してください。'
localization_priority: Priority
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 9e77f2c0163f9093d931c46098498caa8c43f42c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987896"
---
# <a name="plannerplan-resource-type"></a><span data-ttu-id="a5ba1-107">plannerPlan リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a5ba1-107">plannerPlan resource type</span></span>

<span data-ttu-id="a5ba1-p102">**plannerPlan** リソースは、Office 365 での計画を表します。計画は [group](group.md) によって所有され、[plannerTasks](plannertask.md) のコレクションが含まれています。[plannerBuckets](plannerbucket.md) のコレクションを含む場合もあります。各計画オブジェクトには [details](plannerplandetails.md) オブジェクトがあり、計画に関する詳細情報が含まれていることがあります。グループ、計画、タスク間のリレーションシップの詳細については、「[Planner](planner-overview.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a5ba1-p102">The **plannerPlan** resource represents a plan in Office 365. A plan can be owned by a [group](group.md) and contains a collection of [plannerTasks](plannertask.md). It can also have a collection of [plannerBuckets](plannerbucket.md). Each plan object has a [details](plannerplandetails.md) object that can contain more information about the plan. For more information about the relationships between groups, plans, and tasks, see [Planner](planner-overview.md).</span></span>

## <a name="methods"></a><span data-ttu-id="a5ba1-113">メソッド</span><span class="sxs-lookup"><span data-stu-id="a5ba1-113">Methods</span></span>

| <span data-ttu-id="a5ba1-114">メソッド</span><span class="sxs-lookup"><span data-stu-id="a5ba1-114">Method</span></span>           | <span data-ttu-id="a5ba1-115">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="a5ba1-115">Return Type</span></span>    |<span data-ttu-id="a5ba1-116">説明</span><span class="sxs-lookup"><span data-stu-id="a5ba1-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a5ba1-117">Get plannerPlan</span><span class="sxs-lookup"><span data-stu-id="a5ba1-117">Get plannerPlan</span></span>](../api/plannerplan-get.md) | [<span data-ttu-id="a5ba1-118">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="a5ba1-118">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="a5ba1-119">**plannerPlan** オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="a5ba1-119">Read properties and relationships of **plannerPlan** object.</span></span>|
|[<span data-ttu-id="a5ba1-120">List buckets</span><span class="sxs-lookup"><span data-stu-id="a5ba1-120">List buckets</span></span>](../api/plannerplan-list-buckets.md) |<span data-ttu-id="a5ba1-121">[plannerBucket](plannerbucket.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a5ba1-121">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="a5ba1-122">**plannerBucket** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="a5ba1-122">Get a **plannerBucket** object collection.</span></span>|
|[<span data-ttu-id="a5ba1-123">List tasks</span><span class="sxs-lookup"><span data-stu-id="a5ba1-123">List tasks</span></span>](../api/plannerplan-list-tasks.md) |<span data-ttu-id="a5ba1-124">[plannerTask](plannertask.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a5ba1-124">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="a5ba1-125">**plannerTask** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="a5ba1-125">Get a **plannerTask** object collection.</span></span>|
|[<span data-ttu-id="a5ba1-126">Update</span><span class="sxs-lookup"><span data-stu-id="a5ba1-126">Update</span></span>](../api/plannerplan-update.md) | [<span data-ttu-id="a5ba1-127">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="a5ba1-127">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="a5ba1-128">**plannerPlan** オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="a5ba1-128">Update **plannerPlan** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="a5ba1-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a5ba1-129">Properties</span></span>
| <span data-ttu-id="a5ba1-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a5ba1-130">Property</span></span>     | <span data-ttu-id="a5ba1-131">型</span><span class="sxs-lookup"><span data-stu-id="a5ba1-131">Type</span></span>   |<span data-ttu-id="a5ba1-132">説明</span><span class="sxs-lookup"><span data-stu-id="a5ba1-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a5ba1-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a5ba1-133">createdDateTime</span></span>|<span data-ttu-id="a5ba1-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a5ba1-134">DateTimeOffset</span></span>|<span data-ttu-id="a5ba1-p103">読み取り専用。計画の作成日時。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="a5ba1-p103">Read-only. Date and time at which the plan is created. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="a5ba1-139">id</span><span class="sxs-lookup"><span data-stu-id="a5ba1-139">id</span></span>|<span data-ttu-id="a5ba1-140">String</span><span class="sxs-lookup"><span data-stu-id="a5ba1-140">String</span></span>| <span data-ttu-id="a5ba1-141">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a5ba1-141">Read-only.</span></span> <span data-ttu-id="a5ba1-142">計画の ID です。</span><span class="sxs-lookup"><span data-stu-id="a5ba1-142">ID of the plan.</span></span> <span data-ttu-id="a5ba1-143">28 の文字、大文字小文字を区別することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="a5ba1-143">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="a5ba1-144">サービスの[フォーマットの検証](planner-identifiers-disclaimer.md)が行われます。</span><span class="sxs-lookup"><span data-stu-id="a5ba1-144">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="a5ba1-145">owner</span><span class="sxs-lookup"><span data-stu-id="a5ba1-145">owner</span></span>|<span data-ttu-id="a5ba1-146">String</span><span class="sxs-lookup"><span data-stu-id="a5ba1-146">String</span></span>|<span data-ttu-id="a5ba1-147">計画を所有する[グループ](group.md)の ID です。</span><span class="sxs-lookup"><span data-stu-id="a5ba1-147">ID of the [Group](group.md) that owns the plan.</span></span> <span data-ttu-id="a5ba1-148">このフィールドを設定する前に、有効なグループが存在する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a5ba1-148">A valid group must exist before this field can be set.</span></span> <span data-ttu-id="a5ba1-149">設定すると後、は、このプロパティを更新できません。</span><span class="sxs-lookup"><span data-stu-id="a5ba1-149">After it is set, this property can’t be updated.</span></span>|
|<span data-ttu-id="a5ba1-150">タイトル</span><span class="sxs-lookup"><span data-stu-id="a5ba1-150">title</span></span>|<span data-ttu-id="a5ba1-151">String</span><span class="sxs-lookup"><span data-stu-id="a5ba1-151">String</span></span>|<span data-ttu-id="a5ba1-p106">必須。計画のタイトル。</span><span class="sxs-lookup"><span data-stu-id="a5ba1-p106">Required. Title of the plan.</span></span>|
|<span data-ttu-id="a5ba1-154">createdBy</span><span class="sxs-lookup"><span data-stu-id="a5ba1-154">createdBy</span></span>|[<span data-ttu-id="a5ba1-155">identitySet</span><span class="sxs-lookup"><span data-stu-id="a5ba1-155">identitySet</span></span>](identityset.md)|<span data-ttu-id="a5ba1-p107">読み取り専用です。計画を作成したユーザー。</span><span class="sxs-lookup"><span data-stu-id="a5ba1-p107">Read-only. The user who created the plan.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a5ba1-158">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a5ba1-158">Relationships</span></span>
| <span data-ttu-id="a5ba1-159">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a5ba1-159">Relationship</span></span> | <span data-ttu-id="a5ba1-160">型</span><span class="sxs-lookup"><span data-stu-id="a5ba1-160">Type</span></span>   |<span data-ttu-id="a5ba1-161">説明</span><span class="sxs-lookup"><span data-stu-id="a5ba1-161">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a5ba1-162">buckets</span><span class="sxs-lookup"><span data-stu-id="a5ba1-162">buckets</span></span>|<span data-ttu-id="a5ba1-163">[plannerBucket](plannerbucket.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a5ba1-163">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="a5ba1-p108">読み取り専用です。Null 許容型。計画に含まれるバケットのコレクション。</span><span class="sxs-lookup"><span data-stu-id="a5ba1-p108">Read-only. Nullable. Collection of buckets in the plan.</span></span>|
|<span data-ttu-id="a5ba1-167">詳細</span><span class="sxs-lookup"><span data-stu-id="a5ba1-167">details</span></span>|[<span data-ttu-id="a5ba1-168">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="a5ba1-168">plannerPlanDetails</span></span>](plannerplandetails.md)| <span data-ttu-id="a5ba1-p109">読み取り専用です。Null 許容型。計画に関する追加の詳細。</span><span class="sxs-lookup"><span data-stu-id="a5ba1-p109">Read-only. Nullable. Additional details about the plan.</span></span>|
|<span data-ttu-id="a5ba1-172">tasks</span><span class="sxs-lookup"><span data-stu-id="a5ba1-172">tasks</span></span>|<span data-ttu-id="a5ba1-173">[plannerTask](plannertask.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a5ba1-173">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="a5ba1-p110">読み取り専用です。Null 許容型。計画に含まれるタスクのコレクション。</span><span class="sxs-lookup"><span data-stu-id="a5ba1-p110">Read-only. Nullable. Collection of tasks in the plan.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a5ba1-177">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a5ba1-177">JSON representation</span></span>

<span data-ttu-id="a5ba1-178">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a5ba1-178">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerPlan"
}-->

```json
{
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "owner": "String",
  "title": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerPlan resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
