---
title: plannerPlan リソースの種類
description: '**plannerPlan** リソースは、Office 365 での計画を表します。 計画は group によって所有され、plannerTasks のコレクションが含まれています。 plannerBuckets のコレクションを含む場合もあります。 各計画オブジェクトには details オブジェクトがあり、計画に関する詳細情報が含まれていることがあります。 グループ、計画、タスク間のリレーションシップの詳細については、「Planner」を参照してください。'
localization_priority: Priority
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 9e77f2c0163f9093d931c46098498caa8c43f42c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462292"
---
# <a name="plannerplan-resource-type"></a><span data-ttu-id="c4583-107">plannerPlan リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c4583-107">plannerPlan resource type</span></span>

<span data-ttu-id="c4583-108">**plannerPlan** リソースは、Office 365 での計画を表します。</span><span class="sxs-lookup"><span data-stu-id="c4583-108">The **plannerPlan** resource represents a plan in Office 365.</span></span> <span data-ttu-id="c4583-109">計画は [group](group.md) によって所有され、[plannerTasks](plannertask.md) のコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="c4583-109">A plan can be owned by a [group](group.md) and contains a collection of [plannerTasks](plannertask.md).</span></span> <span data-ttu-id="c4583-110">[plannerBuckets](plannerbucket.md) のコレクションを含む場合もあります。</span><span class="sxs-lookup"><span data-stu-id="c4583-110">It can also have a collection of [plannerBuckets](plannerbucket.md).</span></span> <span data-ttu-id="c4583-111">各計画オブジェクトには [details](plannerplandetails.md) オブジェクトがあり、計画に関する詳細情報が含まれていることがあります。</span><span class="sxs-lookup"><span data-stu-id="c4583-111">Each plan object has a [details](plannerplandetails.md) object that can contain more information about the plan.</span></span> <span data-ttu-id="c4583-112">グループ、計画、タスク間のリレーションシップの詳細については、「[Planner](planner-overview.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c4583-112">For more information about the relationships between groups, plans, and tasks, see [Planner](planner-overview.md).</span></span>

## <a name="methods"></a><span data-ttu-id="c4583-113">メソッド</span><span class="sxs-lookup"><span data-stu-id="c4583-113">Methods</span></span>

| <span data-ttu-id="c4583-114">メソッド</span><span class="sxs-lookup"><span data-stu-id="c4583-114">Method</span></span>           | <span data-ttu-id="c4583-115">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="c4583-115">Return Type</span></span>    |<span data-ttu-id="c4583-116">説明</span><span class="sxs-lookup"><span data-stu-id="c4583-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c4583-117">Get plannerPlan</span><span class="sxs-lookup"><span data-stu-id="c4583-117">Get plannerPlan</span></span>](../api/plannerplan-get.md) | [<span data-ttu-id="c4583-118">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="c4583-118">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="c4583-119">**plannerPlan** オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="c4583-119">Read properties and relationships of user object.</span></span>|
|[<span data-ttu-id="c4583-120">List buckets</span><span class="sxs-lookup"><span data-stu-id="c4583-120">List buckets</span></span>](../api/plannerplan-list-buckets.md) |<span data-ttu-id="c4583-121">[plannerBucket](plannerbucket.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c4583-121">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="c4583-122">**plannerBucket** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="c4583-122">Get a CalendarGroup object collection.</span></span>|
|[<span data-ttu-id="c4583-123">List tasks</span><span class="sxs-lookup"><span data-stu-id="c4583-123">List tasks</span></span>](../api/plannerplan-list-tasks.md) |<span data-ttu-id="c4583-124">[plannerTask](plannertask.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c4583-124">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="c4583-125">**plannerTask** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="c4583-125">Get a Calendar object collection.</span></span>|
|[<span data-ttu-id="c4583-126">Update</span><span class="sxs-lookup"><span data-stu-id="c4583-126">Update</span></span>](../api/plannerplan-update.md) | [<span data-ttu-id="c4583-127">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="c4583-127">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="c4583-128">**plannerPlan** オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="c4583-128">Update **plannerPlan** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="c4583-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c4583-129">Properties</span></span>
| <span data-ttu-id="c4583-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c4583-130">Property</span></span>     | <span data-ttu-id="c4583-131">型</span><span class="sxs-lookup"><span data-stu-id="c4583-131">Type</span></span>   |<span data-ttu-id="c4583-132">説明</span><span class="sxs-lookup"><span data-stu-id="c4583-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c4583-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c4583-133">createdDateTime</span></span>|<span data-ttu-id="c4583-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c4583-134">DateTimeOffset</span></span>|<span data-ttu-id="c4583-p103">読み取り専用。計画の作成日時。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="c4583-p103">Read-only. Date and time at which the plan is created. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="c4583-139">id</span><span class="sxs-lookup"><span data-stu-id="c4583-139">id</span></span>|<span data-ttu-id="c4583-140">String</span><span class="sxs-lookup"><span data-stu-id="c4583-140">String</span></span>| <span data-ttu-id="c4583-141">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="c4583-141">Read-only.</span></span> <span data-ttu-id="c4583-142">計画の ID。</span><span class="sxs-lookup"><span data-stu-id="c4583-142">ID of the message</span></span> <span data-ttu-id="c4583-143">28 文字長で、大文字と小文字の区別があります。</span><span class="sxs-lookup"><span data-stu-id="c4583-143">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="c4583-144">[書式検証](planner-identifiers-disclaimer.md)はサービスによって行われます。</span><span class="sxs-lookup"><span data-stu-id="c4583-144">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="c4583-145">owner</span><span class="sxs-lookup"><span data-stu-id="c4583-145">owner</span></span>|<span data-ttu-id="c4583-146">String</span><span class="sxs-lookup"><span data-stu-id="c4583-146">String</span></span>|<span data-ttu-id="c4583-147">計画を所有している [Group](group.md) の ID。</span><span class="sxs-lookup"><span data-stu-id="c4583-147">ID of the principal that owns the lock.</span></span> <span data-ttu-id="c4583-148">このフィールドを設定するためには、有効なグループが存在していなければなりません。</span><span class="sxs-lookup"><span data-stu-id="c4583-148">A valid group must exist before this field can be set.</span></span> <span data-ttu-id="c4583-149">設定すると、このプロパティを更新することはできません。</span><span class="sxs-lookup"><span data-stu-id="c4583-149">After it is set, this property can’t be updated.</span></span>|
|<span data-ttu-id="c4583-150">title</span><span class="sxs-lookup"><span data-stu-id="c4583-150">title</span></span>|<span data-ttu-id="c4583-151">String</span><span class="sxs-lookup"><span data-stu-id="c4583-151">String</span></span>|<span data-ttu-id="c4583-152">必須。</span><span class="sxs-lookup"><span data-stu-id="c4583-152">Required.</span></span> <span data-ttu-id="c4583-153">計画のタイトル。</span><span class="sxs-lookup"><span data-stu-id="c4583-153">Title of the plan.</span></span>|
|<span data-ttu-id="c4583-154">createdBy</span><span class="sxs-lookup"><span data-stu-id="c4583-154">createdBy</span></span>|[<span data-ttu-id="c4583-155">identitySet</span><span class="sxs-lookup"><span data-stu-id="c4583-155">identitySet</span></span>](identityset.md)|<span data-ttu-id="c4583-156">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="c4583-156">Read-only.</span></span> <span data-ttu-id="c4583-157">計画を作成したユーザー。</span><span class="sxs-lookup"><span data-stu-id="c4583-157">The name of the user who created the page.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c4583-158">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c4583-158">Relationships</span></span>
| <span data-ttu-id="c4583-159">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c4583-159">Relationship</span></span> | <span data-ttu-id="c4583-160">型</span><span class="sxs-lookup"><span data-stu-id="c4583-160">Type</span></span>   |<span data-ttu-id="c4583-161">説明</span><span class="sxs-lookup"><span data-stu-id="c4583-161">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c4583-162">buckets</span><span class="sxs-lookup"><span data-stu-id="c4583-162">buckets</span></span>|<span data-ttu-id="c4583-163">[plannerBucket](plannerbucket.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c4583-163">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="c4583-p108">読み取り専用です。Null 許容型。計画に含まれるバケットのコレクション。</span><span class="sxs-lookup"><span data-stu-id="c4583-p108">Read-only. Nullable. Collection of buckets in the plan.</span></span>|
|<span data-ttu-id="c4583-167">詳細</span><span class="sxs-lookup"><span data-stu-id="c4583-167">details</span></span>|[<span data-ttu-id="c4583-168">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="c4583-168">plannerPlanDetails</span></span>](plannerplandetails.md)| <span data-ttu-id="c4583-169">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="c4583-169">Read-only.</span></span> <span data-ttu-id="c4583-170">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="c4583-170">Nullable.</span></span> <span data-ttu-id="c4583-171">計画に関する追加の詳細。</span><span class="sxs-lookup"><span data-stu-id="c4583-171">Additional details about the plan.</span></span>|
|<span data-ttu-id="c4583-172">tasks</span><span class="sxs-lookup"><span data-stu-id="c4583-172">tasks</span></span>|<span data-ttu-id="c4583-173">[plannerTask](plannertask.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c4583-173">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="c4583-174">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="c4583-174">Read-only.</span></span> <span data-ttu-id="c4583-175">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="c4583-175">Nullable.</span></span> <span data-ttu-id="c4583-176">計画に含まれるタスクのコレクション。</span><span class="sxs-lookup"><span data-stu-id="c4583-176">Collection of tasks in the plan.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c4583-177">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c4583-177">JSON representation</span></span>

<span data-ttu-id="c4583-178">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c4583-178">Here is a JSON representation of the resource.</span></span>

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
