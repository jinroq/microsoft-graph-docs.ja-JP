---
title: plannerPlan リソースの種類
description: '**PlannerPlan**リソースでは、Office 365 のプランを表します。 計画は、グループが所有することができ、plannerTasks のコレクションが含まれています。 PlannerBuckets のコレクションもあります。 各プラン オブジェクトには、計画の詳細を含めることができる詳細オブジェクトがあります。 グループ、計画、およびタスク間の関係の詳細については、プランナーを参照してください。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: f37f6ea08f2951256e2d7f94cf9abad7e8ac60b2
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529552"
---
# <a name="plannerplan-resource-type"></a><span data-ttu-id="19c35-107">plannerPlan リソースの種類</span><span class="sxs-lookup"><span data-stu-id="19c35-107">plannerPlan resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="19c35-108">**PlannerPlan**リソースでは、Office 365 のプランを表します。</span><span class="sxs-lookup"><span data-stu-id="19c35-108">The **plannerPlan** resource represents a plan in Office 365.</span></span> <span data-ttu-id="19c35-109">計画は、[グループ](group.md)が所有することができ、 [plannerTasks](plannertask.md)のコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="19c35-109">A plan can be owned by a [group](group.md) and contains a collection of [plannerTasks](plannertask.md).</span></span> <span data-ttu-id="19c35-110">[PlannerBuckets](plannerbucket.md)のコレクションもあります。</span><span class="sxs-lookup"><span data-stu-id="19c35-110">It can also have a collection of [plannerBuckets](plannerbucket.md).</span></span> <span data-ttu-id="19c35-111">各プラン オブジェクトには、計画の詳細を含めることができる[詳細](plannerplandetails.md)オブジェクトがあります。</span><span class="sxs-lookup"><span data-stu-id="19c35-111">Each plan object has a [details](plannerplandetails.md) object which can contain more information about the plan.</span></span> <span data-ttu-id="19c35-112">グループ、計画、およびタスク間の関係の詳細については、[プランナー](planner-overview.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="19c35-112">For more information about the relationships between groups, plans, and tasks, see [Planner](planner-overview.md).</span></span>



## <a name="methods"></a><span data-ttu-id="19c35-113">メソッド</span><span class="sxs-lookup"><span data-stu-id="19c35-113">Methods</span></span>

| <span data-ttu-id="19c35-114">メソッド</span><span class="sxs-lookup"><span data-stu-id="19c35-114">Method</span></span>           | <span data-ttu-id="19c35-115">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="19c35-115">Return Type</span></span>    |<span data-ttu-id="19c35-116">説明</span><span class="sxs-lookup"><span data-stu-id="19c35-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="19c35-117">Get plannerPlan</span><span class="sxs-lookup"><span data-stu-id="19c35-117">[Get plannerPlan](../api/plannerplan-get.md)</span></span> | [<span data-ttu-id="19c35-118">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="19c35-118">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="19c35-119">plannerPlan オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="19c35-119">Read properties and relationships of **plannerPlan** object.</span></span>|
|<span data-ttu-id="19c35-120">List buckets</span><span class="sxs-lookup"><span data-stu-id="19c35-120">[List buckets](../api/plannerplan-list-buckets.md)</span></span> |<span data-ttu-id="19c35-121">[plannerBucket](plannerbucket.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="19c35-121">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="19c35-122">plannerBucket オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="19c35-122">Get a **plannerBucket** object collection.</span></span>|
|[<span data-ttu-id="19c35-123">List tasks</span><span class="sxs-lookup"><span data-stu-id="19c35-123">List tasks</span></span>](../api/plannerplan-list-tasks.md) |<span data-ttu-id="19c35-124">[plannerTask](plannertask.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="19c35-124">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="19c35-125">**plannerTask** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="19c35-125">Get a **plannerTask** object collection.</span></span>|
|[<span data-ttu-id="19c35-126">Update</span><span class="sxs-lookup"><span data-stu-id="19c35-126">Update</span></span>](../api/plannerplan-update.md) | [<span data-ttu-id="19c35-127">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="19c35-127">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="19c35-128">plannerPlan オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="19c35-128">Update **plannerPlan** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="19c35-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="19c35-129">Properties</span></span>
| <span data-ttu-id="19c35-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="19c35-130">Property</span></span>     | <span data-ttu-id="19c35-131">型</span><span class="sxs-lookup"><span data-stu-id="19c35-131">Type</span></span>   |<span data-ttu-id="19c35-132">説明</span><span class="sxs-lookup"><span data-stu-id="19c35-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="19c35-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="19c35-133">createdDateTime</span></span>|<span data-ttu-id="19c35-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="19c35-134">DateTimeOffset</span></span>|<span data-ttu-id="19c35-p103">読み取り専用。計画の作成日時。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="19c35-p103">Read-only. Date and time at which the plan is created. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="19c35-139">id</span><span class="sxs-lookup"><span data-stu-id="19c35-139">id</span></span>|<span data-ttu-id="19c35-140">文字列</span><span class="sxs-lookup"><span data-stu-id="19c35-140">String</span></span>| <span data-ttu-id="19c35-141">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="19c35-141">Read-only.</span></span> <span data-ttu-id="19c35-142">計画の ID です。</span><span class="sxs-lookup"><span data-stu-id="19c35-142">ID of the plan.</span></span> <span data-ttu-id="19c35-143">28 の文字、大文字小文字を区別することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="19c35-143">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="19c35-144">サービスの[フォーマットの検証](tasks-identifiers-disclaimer.md)が行われます。</span><span class="sxs-lookup"><span data-stu-id="19c35-144">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="19c35-145">owner</span><span class="sxs-lookup"><span data-stu-id="19c35-145">owner</span></span>|<span data-ttu-id="19c35-146">String</span><span class="sxs-lookup"><span data-stu-id="19c35-146">String</span></span>|<span data-ttu-id="19c35-147">計画を所有する[グループ](group.md)の ID です。</span><span class="sxs-lookup"><span data-stu-id="19c35-147">ID of the [Group](group.md) that owns the plan.</span></span> <span data-ttu-id="19c35-148">このフィールドを設定する前に、有効なグループが存在する必要があります。</span><span class="sxs-lookup"><span data-stu-id="19c35-148">A valid group must exist before this field can be set.</span></span> <span data-ttu-id="19c35-149">設定すると後、は、このプロパティを更新できません。</span><span class="sxs-lookup"><span data-stu-id="19c35-149">After it is set, this property can’t be updated.</span></span>|
|<span data-ttu-id="19c35-150">タイトル</span><span class="sxs-lookup"><span data-stu-id="19c35-150">title</span></span>|<span data-ttu-id="19c35-151">String</span><span class="sxs-lookup"><span data-stu-id="19c35-151">String</span></span>|<span data-ttu-id="19c35-p106">必須。計画のタイトル。</span><span class="sxs-lookup"><span data-stu-id="19c35-p106">Required. Title of the plan.</span></span>|
|<span data-ttu-id="19c35-154">createdBy</span><span class="sxs-lookup"><span data-stu-id="19c35-154">createdBy</span></span>|[<span data-ttu-id="19c35-155">identitySet</span><span class="sxs-lookup"><span data-stu-id="19c35-155">identitySet</span></span>](identityset.md)|<span data-ttu-id="19c35-p107">読み取り専用です。計画を作成したユーザー。</span><span class="sxs-lookup"><span data-stu-id="19c35-p107">Read-only. The user who created the plan.</span></span>|
|<span data-ttu-id="19c35-158">コンテキスト</span><span class="sxs-lookup"><span data-stu-id="19c35-158">contexts</span></span>|[<span data-ttu-id="19c35-159">plannerPlanContextCollection</span><span class="sxs-lookup"><span data-stu-id="19c35-159">plannerPlanContextCollection</span></span>](plannerplancontextcollection.md)| <span data-ttu-id="19c35-160">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="19c35-160">Read-only.</span></span> <span data-ttu-id="19c35-161">このプランが使用されている、追加のユーザー エクスペリエンスは、 [plannerPlanContext](plannerplancontext.md)のエントリとして表されます。</span><span class="sxs-lookup"><span data-stu-id="19c35-161">Additional user experiences in which this plan is used, represented as [plannerPlanContext](plannerplancontext.md) entries.</span></span>|

## <a name="relationships"></a><span data-ttu-id="19c35-162">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="19c35-162">Relationships</span></span>
| <span data-ttu-id="19c35-163">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="19c35-163">Relationship</span></span> | <span data-ttu-id="19c35-164">型</span><span class="sxs-lookup"><span data-stu-id="19c35-164">Type</span></span>   |<span data-ttu-id="19c35-165">説明</span><span class="sxs-lookup"><span data-stu-id="19c35-165">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="19c35-166">buckets</span><span class="sxs-lookup"><span data-stu-id="19c35-166">buckets</span></span>|<span data-ttu-id="19c35-167">[plannerBucket](plannerbucket.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="19c35-167">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="19c35-p109">読み取り専用です。Null 許容型。計画に含まれるバケットのコレクション。</span><span class="sxs-lookup"><span data-stu-id="19c35-p109">Read-only. Nullable. Collection of buckets in the plan.</span></span>|
|<span data-ttu-id="19c35-171">詳細</span><span class="sxs-lookup"><span data-stu-id="19c35-171">details</span></span>|[<span data-ttu-id="19c35-172">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="19c35-172">plannerPlanDetails</span></span>](plannerplandetails.md)| <span data-ttu-id="19c35-p110">読み取り専用です。Null 許容型。計画に関する追加の詳細。</span><span class="sxs-lookup"><span data-stu-id="19c35-p110">Read-only. Nullable. Additional details about the plan.</span></span>|
|<span data-ttu-id="19c35-176">tasks</span><span class="sxs-lookup"><span data-stu-id="19c35-176">tasks</span></span>|<span data-ttu-id="19c35-177">[plannerTask](plannertask.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="19c35-177">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="19c35-p111">読み取り専用です。Null 許容型。計画に含まれるタスクのコレクション。</span><span class="sxs-lookup"><span data-stu-id="19c35-p111">Read-only. Nullable. Collection of tasks in the plan.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="19c35-181">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="19c35-181">JSON representation</span></span>

<span data-ttu-id="19c35-182">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="19c35-182">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "plannerPlan resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerplan.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
