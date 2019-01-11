---
title: plannerPlan リソースの種類
description: '**PlannerPlan**リソースでは、Office 365 のプランを表します。 計画は、グループが所有することができ、plannerTasks のコレクションが含まれています。 PlannerBuckets のコレクションもあります。 各プラン オブジェクトには、計画の詳細を含めることができる詳細オブジェクトがあります。 グループ、計画、およびタスク間の関係の詳細については、プランナーを参照してください。'
localization_priority: Normal
ms.openlocfilehash: 4890daa6ad221a36cf0029b49ce39560fc80afcd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888103"
---
# <a name="plannerplan-resource-type"></a><span data-ttu-id="5a467-107">plannerPlan リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5a467-107">plannerPlan resource type</span></span>

> <span data-ttu-id="5a467-108">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5a467-108">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5a467-109">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5a467-109">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5a467-110">**PlannerPlan**リソースでは、Office 365 のプランを表します。</span><span class="sxs-lookup"><span data-stu-id="5a467-110">The **plannerPlan** resource represents a plan in Office 365.</span></span> <span data-ttu-id="5a467-111">計画は、[グループ](group.md)が所有することができ、 [plannerTasks](plannertask.md)のコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="5a467-111">A plan can be owned by a [group](group.md) and contains a collection of [plannerTasks](plannertask.md).</span></span> <span data-ttu-id="5a467-112">[PlannerBuckets](plannerbucket.md)のコレクションもあります。</span><span class="sxs-lookup"><span data-stu-id="5a467-112">It can also have a collection of [plannerBuckets](plannerbucket.md).</span></span> <span data-ttu-id="5a467-113">各プラン オブジェクトには、計画の詳細を含めることができる[詳細](plannerplandetails.md)オブジェクトがあります。</span><span class="sxs-lookup"><span data-stu-id="5a467-113">Each plan object has a [details](plannerplandetails.md) object which can contain more information about the plan.</span></span> <span data-ttu-id="5a467-114">グループ、計画、およびタスク間の関係の詳細については、[プランナー](planner-overview.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5a467-114">For more information about the relationships between groups, plans, and tasks, see [Planner](planner-overview.md).</span></span>



## <a name="methods"></a><span data-ttu-id="5a467-115">メソッド</span><span class="sxs-lookup"><span data-stu-id="5a467-115">Methods</span></span>

| <span data-ttu-id="5a467-116">メソッド</span><span class="sxs-lookup"><span data-stu-id="5a467-116">Method</span></span>           | <span data-ttu-id="5a467-117">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="5a467-117">Return Type</span></span>    |<span data-ttu-id="5a467-118">説明</span><span class="sxs-lookup"><span data-stu-id="5a467-118">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5a467-119">Get plannerPlan</span><span class="sxs-lookup"><span data-stu-id="5a467-119">Get plannerPlan</span></span>](../api/plannerplan-get.md) | [<span data-ttu-id="5a467-120">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="5a467-120">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="5a467-121">**plannerPlan** オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="5a467-121">Read properties and relationships of **plannerPlan** object.</span></span>|
|[<span data-ttu-id="5a467-122">List buckets</span><span class="sxs-lookup"><span data-stu-id="5a467-122">List buckets</span></span>](../api/plannerplan-list-buckets.md) |<span data-ttu-id="5a467-123">[plannerBucket](plannerbucket.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="5a467-123">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="5a467-124">**plannerBucket** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="5a467-124">Get a **plannerBucket** object collection.</span></span>|
|[<span data-ttu-id="5a467-125">List tasks</span><span class="sxs-lookup"><span data-stu-id="5a467-125">List tasks</span></span>](../api/plannerplan-list-tasks.md) |<span data-ttu-id="5a467-126">[plannerTask](plannertask.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="5a467-126">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="5a467-127">**plannerTask** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="5a467-127">Get a **plannerTask** object collection.</span></span>|
|[<span data-ttu-id="5a467-128">Update</span><span class="sxs-lookup"><span data-stu-id="5a467-128">Update</span></span>](../api/plannerplan-update.md) | [<span data-ttu-id="5a467-129">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="5a467-129">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="5a467-130">**plannerPlan** オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="5a467-130">Update **plannerPlan** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="5a467-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5a467-131">Properties</span></span>
| <span data-ttu-id="5a467-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5a467-132">Property</span></span>     | <span data-ttu-id="5a467-133">種類</span><span class="sxs-lookup"><span data-stu-id="5a467-133">Type</span></span>   |<span data-ttu-id="5a467-134">説明</span><span class="sxs-lookup"><span data-stu-id="5a467-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5a467-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5a467-135">createdDateTime</span></span>|<span data-ttu-id="5a467-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5a467-136">DateTimeOffset</span></span>|<span data-ttu-id="5a467-p104">読み取り専用。計画の作成日時。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="5a467-p104">Read-only. Date and time at which the plan is created. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="5a467-141">id</span><span class="sxs-lookup"><span data-stu-id="5a467-141">id</span></span>|<span data-ttu-id="5a467-142">String</span><span class="sxs-lookup"><span data-stu-id="5a467-142">String</span></span>| <span data-ttu-id="5a467-143">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="5a467-143">Read-only.</span></span> <span data-ttu-id="5a467-144">計画の ID です。</span><span class="sxs-lookup"><span data-stu-id="5a467-144">ID of the plan.</span></span> <span data-ttu-id="5a467-145">28 の文字、大文字小文字を区別することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="5a467-145">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="5a467-146">サービスの[フォーマットの検証](tasks-identifiers-disclaimer.md)が行われます。</span><span class="sxs-lookup"><span data-stu-id="5a467-146">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="5a467-147">owner</span><span class="sxs-lookup"><span data-stu-id="5a467-147">owner</span></span>|<span data-ttu-id="5a467-148">String</span><span class="sxs-lookup"><span data-stu-id="5a467-148">String</span></span>|<span data-ttu-id="5a467-149">計画を所有する[グループ](group.md)の ID です。</span><span class="sxs-lookup"><span data-stu-id="5a467-149">ID of the [Group](group.md) that owns the plan.</span></span> <span data-ttu-id="5a467-150">このフィールドを設定する前に、有効なグループが存在する必要があります。</span><span class="sxs-lookup"><span data-stu-id="5a467-150">A valid group must exist before this field can be set.</span></span> <span data-ttu-id="5a467-151">設定すると後、は、このプロパティを更新できません。</span><span class="sxs-lookup"><span data-stu-id="5a467-151">After it is set, this property can’t be updated.</span></span>|
|<span data-ttu-id="5a467-152">タイトル</span><span class="sxs-lookup"><span data-stu-id="5a467-152">title</span></span>|<span data-ttu-id="5a467-153">String</span><span class="sxs-lookup"><span data-stu-id="5a467-153">String</span></span>|<span data-ttu-id="5a467-p107">必須。計画のタイトル。</span><span class="sxs-lookup"><span data-stu-id="5a467-p107">Required. Title of the plan.</span></span>|
|<span data-ttu-id="5a467-156">createdBy</span><span class="sxs-lookup"><span data-stu-id="5a467-156">createdBy</span></span>|[<span data-ttu-id="5a467-157">identitySet</span><span class="sxs-lookup"><span data-stu-id="5a467-157">identitySet</span></span>](identityset.md)|<span data-ttu-id="5a467-p108">読み取り専用です。計画を作成したユーザー。</span><span class="sxs-lookup"><span data-stu-id="5a467-p108">Read-only. The user who created the plan.</span></span>|
|<span data-ttu-id="5a467-160">コンテキスト</span><span class="sxs-lookup"><span data-stu-id="5a467-160">contexts</span></span>|[<span data-ttu-id="5a467-161">plannerPlanContextCollection</span><span class="sxs-lookup"><span data-stu-id="5a467-161">plannerPlanContextCollection</span></span>](plannerplancontextcollection.md)| <span data-ttu-id="5a467-162">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="5a467-162">Read-only.</span></span> <span data-ttu-id="5a467-163">このプランが使用されている、追加のユーザー エクスペリエンスは、 [plannerPlanContext](plannerplancontext.md)のエントリとして表されます。</span><span class="sxs-lookup"><span data-stu-id="5a467-163">Additional user experiences in which this plan is used, represented as [plannerPlanContext](plannerplancontext.md) entries.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5a467-164">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5a467-164">Relationships</span></span>
| <span data-ttu-id="5a467-165">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5a467-165">Relationship</span></span> | <span data-ttu-id="5a467-166">型</span><span class="sxs-lookup"><span data-stu-id="5a467-166">Type</span></span>   |<span data-ttu-id="5a467-167">説明</span><span class="sxs-lookup"><span data-stu-id="5a467-167">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5a467-168">buckets</span><span class="sxs-lookup"><span data-stu-id="5a467-168">buckets</span></span>|<span data-ttu-id="5a467-169">[plannerBucket](plannerbucket.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="5a467-169">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="5a467-p110">読み取り専用です。Null 許容型。計画に含まれるバケットのコレクション。</span><span class="sxs-lookup"><span data-stu-id="5a467-p110">Read-only. Nullable. Collection of buckets in the plan.</span></span>|
|<span data-ttu-id="5a467-173">詳細</span><span class="sxs-lookup"><span data-stu-id="5a467-173">details</span></span>|[<span data-ttu-id="5a467-174">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="5a467-174">plannerPlanDetails</span></span>](plannerplandetails.md)| <span data-ttu-id="5a467-p111">読み取り専用です。Null 許容型。計画に関する追加の詳細。</span><span class="sxs-lookup"><span data-stu-id="5a467-p111">Read-only. Nullable. Additional details about the plan.</span></span>|
|<span data-ttu-id="5a467-178">tasks</span><span class="sxs-lookup"><span data-stu-id="5a467-178">tasks</span></span>|<span data-ttu-id="5a467-179">[plannerTask](plannertask.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="5a467-179">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="5a467-p112">読み取り専用です。Null 許容型。計画に含まれるタスクのコレクション。</span><span class="sxs-lookup"><span data-stu-id="5a467-p112">Read-only. Nullable. Collection of tasks in the plan.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5a467-183">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5a467-183">JSON representation</span></span>

<span data-ttu-id="5a467-184">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5a467-184">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
<!-- {
  "type": "#page.annotation",
  "description": "plannerPlan resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
