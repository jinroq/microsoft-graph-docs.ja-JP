---
title: plan リソースの種類を計画する
description: プラン**** リソースは、Office 365 のプランを表します。 プランは、グループが所有することができ、プランのタスクのコレクションが含まれています。 また、プランのコレクションを持つこともできます。 各プランオブジェクトには details オブジェクトがあり、プランに関する詳細情報を含めることができます。 グループ、プラン、およびタスク間の関係の詳細については、「Planner」を参照してください。
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: f37f6ea08f2951256e2d7f94cf9abad7e8ac60b2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32578870"
---
# <a name="plannerplan-resource-type"></a><span data-ttu-id="b524f-107">plan リソースの種類を計画する</span><span class="sxs-lookup"><span data-stu-id="b524f-107">plannerPlan resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b524f-108">プラン\*\*\*\* リソースは、Office 365 のプランを表します。</span><span class="sxs-lookup"><span data-stu-id="b524f-108">The **plannerPlan** resource represents a plan in Office 365.</span></span> <span data-ttu-id="b524f-109">プランは、[グループ](group.md)が所有することができ、プランの[タスク](plannertask.md)のコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="b524f-109">A plan can be owned by a [group](group.md) and contains a collection of [plannerTasks](plannertask.md).</span></span> <span data-ttu-id="b524f-110">また、[プラン](plannerbucket.md)のコレクションを持つこともできます。</span><span class="sxs-lookup"><span data-stu-id="b524f-110">It can also have a collection of [plannerBuckets](plannerbucket.md).</span></span> <span data-ttu-id="b524f-111">各プランオブジェクトには[details](plannerplandetails.md)オブジェクトがあり、プランに関する詳細情報を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="b524f-111">Each plan object has a [details](plannerplandetails.md) object which can contain more information about the plan.</span></span> <span data-ttu-id="b524f-112">グループ、プラン、およびタスク間の関係の詳細については、「 [Planner](planner-overview.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b524f-112">For more information about the relationships between groups, plans, and tasks, see [Planner](planner-overview.md).</span></span>



## <a name="methods"></a><span data-ttu-id="b524f-113">メソッド</span><span class="sxs-lookup"><span data-stu-id="b524f-113">Methods</span></span>

| <span data-ttu-id="b524f-114">メソッド</span><span class="sxs-lookup"><span data-stu-id="b524f-114">Method</span></span>           | <span data-ttu-id="b524f-115">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="b524f-115">Return Type</span></span>    |<span data-ttu-id="b524f-116">説明</span><span class="sxs-lookup"><span data-stu-id="b524f-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b524f-117">Get plannerPlan</span><span class="sxs-lookup"><span data-stu-id="b524f-117">Get plannerPlan</span></span>](../api/plannerplan-get.md) | [<span data-ttu-id="b524f-118">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="b524f-118">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="b524f-119">**plan**オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="b524f-119">Read properties and relationships of **plannerPlan** object.</span></span>|
|[<span data-ttu-id="b524f-120">バケットをリストする</span><span class="sxs-lookup"><span data-stu-id="b524f-120">List buckets</span></span>](../api/plannerplan-list-buckets.md) |<span data-ttu-id="b524f-121">[プラン | バケット](plannerbucket.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="b524f-121">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="b524f-122">**プラン**を取得するオブジェクトコレクション。</span><span class="sxs-lookup"><span data-stu-id="b524f-122">Get a **plannerBucket** object collection.</span></span>|
|[<span data-ttu-id="b524f-123">タスクを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="b524f-123">List tasks</span></span>](../api/plannerplan-list-tasks.md) |<span data-ttu-id="b524f-124">[plannerTask](plannertask.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b524f-124">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="b524f-125">プランを取得する**タスク**オブジェクトコレクション。</span><span class="sxs-lookup"><span data-stu-id="b524f-125">Get a **plannerTask** object collection.</span></span>|
|[<span data-ttu-id="b524f-126">更新する</span><span class="sxs-lookup"><span data-stu-id="b524f-126">Update</span></span>](../api/plannerplan-update.md) | [<span data-ttu-id="b524f-127">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="b524f-127">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="b524f-128">**plan**オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="b524f-128">Update **plannerPlan** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="b524f-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b524f-129">Properties</span></span>
| <span data-ttu-id="b524f-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b524f-130">Property</span></span>     | <span data-ttu-id="b524f-131">型</span><span class="sxs-lookup"><span data-stu-id="b524f-131">Type</span></span>   |<span data-ttu-id="b524f-132">説明</span><span class="sxs-lookup"><span data-stu-id="b524f-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b524f-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b524f-133">createdDateTime</span></span>|<span data-ttu-id="b524f-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b524f-134">DateTimeOffset</span></span>|<span data-ttu-id="b524f-p103">読み取り専用。計画の作成日時。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="b524f-p103">Read-only. Date and time at which the plan is created. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="b524f-139">id</span><span class="sxs-lookup"><span data-stu-id="b524f-139">id</span></span>|<span data-ttu-id="b524f-140">String</span><span class="sxs-lookup"><span data-stu-id="b524f-140">String</span></span>| <span data-ttu-id="b524f-141">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="b524f-141">Read-only.</span></span> <span data-ttu-id="b524f-142">プランの ID。</span><span class="sxs-lookup"><span data-stu-id="b524f-142">ID of the plan.</span></span> <span data-ttu-id="b524f-143">28 文字長で、大文字と小文字の区別があります。</span><span class="sxs-lookup"><span data-stu-id="b524f-143">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="b524f-144">[書式検証](tasks-identifiers-disclaimer.md)はサービスによって行われます。</span><span class="sxs-lookup"><span data-stu-id="b524f-144">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="b524f-145">owner</span><span class="sxs-lookup"><span data-stu-id="b524f-145">owner</span></span>|<span data-ttu-id="b524f-146">String</span><span class="sxs-lookup"><span data-stu-id="b524f-146">String</span></span>|<span data-ttu-id="b524f-147">プランを所有する[グループ](group.md)の ID。</span><span class="sxs-lookup"><span data-stu-id="b524f-147">ID of the [Group](group.md) that owns the plan.</span></span> <span data-ttu-id="b524f-148">このフィールドを設定するためには、有効なグループが存在していなければなりません。</span><span class="sxs-lookup"><span data-stu-id="b524f-148">A valid group must exist before this field can be set.</span></span> <span data-ttu-id="b524f-149">設定された後は、このプロパティは更新できません。</span><span class="sxs-lookup"><span data-stu-id="b524f-149">After it is set, this property can’t be updated.</span></span>|
|<span data-ttu-id="b524f-150">title</span><span class="sxs-lookup"><span data-stu-id="b524f-150">title</span></span>|<span data-ttu-id="b524f-151">String</span><span class="sxs-lookup"><span data-stu-id="b524f-151">String</span></span>|<span data-ttu-id="b524f-152">必須。</span><span class="sxs-lookup"><span data-stu-id="b524f-152">Required.</span></span> <span data-ttu-id="b524f-153">計画のタイトル。</span><span class="sxs-lookup"><span data-stu-id="b524f-153">Title of the plan.</span></span>|
|<span data-ttu-id="b524f-154">createdBy</span><span class="sxs-lookup"><span data-stu-id="b524f-154">createdBy</span></span>|[<span data-ttu-id="b524f-155">identitySet</span><span class="sxs-lookup"><span data-stu-id="b524f-155">identitySet</span></span>](identityset.md)|<span data-ttu-id="b524f-156">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="b524f-156">Read-only.</span></span> <span data-ttu-id="b524f-157">プランを作成したユーザー。</span><span class="sxs-lookup"><span data-stu-id="b524f-157">The user who created the plan.</span></span>|
|<span data-ttu-id="b524f-158">状況</span><span class="sxs-lookup"><span data-stu-id="b524f-158">contexts</span></span>|[<span data-ttu-id="b524f-159">plannerPlanContextCollection</span><span class="sxs-lookup"><span data-stu-id="b524f-159">plannerPlanContextCollection</span></span>](plannerplancontextcollection.md)| <span data-ttu-id="b524f-160">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="b524f-160">Read-only.</span></span> <span data-ttu-id="b524f-161">このプランが使用される追加のユーザーエクスペリエンス。このプランは、[コンテキスト](plannerplancontext.md)エントリをプランとして表現します。</span><span class="sxs-lookup"><span data-stu-id="b524f-161">Additional user experiences in which this plan is used, represented as [plannerPlanContext](plannerplancontext.md) entries.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b524f-162">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b524f-162">Relationships</span></span>
| <span data-ttu-id="b524f-163">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b524f-163">Relationship</span></span> | <span data-ttu-id="b524f-164">型</span><span class="sxs-lookup"><span data-stu-id="b524f-164">Type</span></span>   |<span data-ttu-id="b524f-165">説明</span><span class="sxs-lookup"><span data-stu-id="b524f-165">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b524f-166">buckets</span><span class="sxs-lookup"><span data-stu-id="b524f-166">buckets</span></span>|<span data-ttu-id="b524f-167">[プラン | バケット](plannerbucket.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="b524f-167">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="b524f-p109">読み取り専用。Null 許容型。計画に含まれるバケットのコレクション。</span><span class="sxs-lookup"><span data-stu-id="b524f-p109">Read-only. Nullable. Collection of buckets in the plan.</span></span>|
|<span data-ttu-id="b524f-171">details</span><span class="sxs-lookup"><span data-stu-id="b524f-171">details</span></span>|[<span data-ttu-id="b524f-172">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="b524f-172">plannerPlanDetails</span></span>](plannerplandetails.md)| <span data-ttu-id="b524f-173">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="b524f-173">Read-only.</span></span> <span data-ttu-id="b524f-174">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="b524f-174">Nullable.</span></span> <span data-ttu-id="b524f-175">計画に関する追加の詳細。</span><span class="sxs-lookup"><span data-stu-id="b524f-175">Additional details about the plan.</span></span>|
|<span data-ttu-id="b524f-176">tasks</span><span class="sxs-lookup"><span data-stu-id="b524f-176">tasks</span></span>|<span data-ttu-id="b524f-177">[plannerTask](plannertask.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b524f-177">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="b524f-178">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="b524f-178">Read-only.</span></span> <span data-ttu-id="b524f-179">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="b524f-179">Nullable.</span></span> <span data-ttu-id="b524f-180">計画に含まれるタスクのコレクション。</span><span class="sxs-lookup"><span data-stu-id="b524f-180">Collection of tasks in the plan.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b524f-181">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b524f-181">JSON representation</span></span>

<span data-ttu-id="b524f-182">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b524f-182">Here is a JSON representation of the resource.</span></span>

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
