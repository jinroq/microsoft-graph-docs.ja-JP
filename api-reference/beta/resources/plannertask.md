---
title: plannerTask のリソースの種類
description: '**plannerTask** リソースは、Office 365 の Planner のタスクを表します。Planner のタスクは plan に格納され、また、タスクは計画の中の bucket に割り当てることができます。各タスクオブジェクトには、タスクについてのより詳細な情報を保持するための details オブジェクトがあります。グループ、プラン、タスクの関係についての詳細は「概要」を参照してください。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 1eb718daad405fb6aaed2f170747bc91dad47b76
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009000"
---
# <a name="plannertask-resource-type"></a><span data-ttu-id="9fcd6-106">plannerTask のリソースの種類</span><span class="sxs-lookup"><span data-stu-id="9fcd6-106">plannerTask resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9fcd6-p102">**plannerTask** リソースは、Office 365 の Planner のタスクを表します。Planner のタスクは [plan](plannerplan.md) に格納され、また、タスクは計画の中の [bucket](plannerbucket.md) に割り当てることができます。各タスクオブジェクトには、タスクについてのより詳細な情報を保持するための [details](plannertaskdetails.md) オブジェクトがあります。グループ、プラン、タスクの関係についての詳細は「[概要](planner-overview.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9fcd6-p102">The **plannerTask** resource represents a Planner task in Office 365. A Planner task is contained in a [plan](plannerplan.md) and can be assigned to a [bucket](plannerbucket.md) in a plan. Each task object has a [details](plannertaskdetails.md) object which can contain more information about the task. See [overview](planner-overview.md) for more information regarding relationships between group, plan and task.</span></span>


## <a name="methods"></a><span data-ttu-id="9fcd6-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="9fcd6-111">Methods</span></span>

| <span data-ttu-id="9fcd6-112">メソッド</span><span class="sxs-lookup"><span data-stu-id="9fcd6-112">Method</span></span>           | <span data-ttu-id="9fcd6-113">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="9fcd6-113">Return Type</span></span>    |<span data-ttu-id="9fcd6-114">説明</span><span class="sxs-lookup"><span data-stu-id="9fcd6-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9fcd6-115">Get plannerTask</span><span class="sxs-lookup"><span data-stu-id="9fcd6-115">Get plannerTask</span></span>](../api/plannertask-get.md) | [<span data-ttu-id="9fcd6-116">plannerTask</span><span class="sxs-lookup"><span data-stu-id="9fcd6-116">plannerTask</span></span>](plannertask.md) |<span data-ttu-id="9fcd6-117">**plannerTask** オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="9fcd6-117">Read properties and relationships of **plannerTask** object.</span></span>|
|[<span data-ttu-id="9fcd6-118">Update</span><span class="sxs-lookup"><span data-stu-id="9fcd6-118">Update</span></span>](../api/plannertask-update.md) | [<span data-ttu-id="9fcd6-119">plannerTask</span><span class="sxs-lookup"><span data-stu-id="9fcd6-119">plannerTask</span></span>](plannertask.md) |<span data-ttu-id="9fcd6-120">**plannerTask** オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="9fcd6-120">Update **plannerTask** object.</span></span> |
|[<span data-ttu-id="9fcd6-121">Delete</span><span class="sxs-lookup"><span data-stu-id="9fcd6-121">Delete</span></span>](../api/plannertask-delete.md) | <span data-ttu-id="9fcd6-122">なし</span><span class="sxs-lookup"><span data-stu-id="9fcd6-122">None</span></span> |<span data-ttu-id="9fcd6-123">**plannerTask** オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="9fcd6-123">Delete **plannerTask** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="9fcd6-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9fcd6-124">Properties</span></span>
| <span data-ttu-id="9fcd6-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9fcd6-125">Property</span></span>     | <span data-ttu-id="9fcd6-126">型</span><span class="sxs-lookup"><span data-stu-id="9fcd6-126">Type</span></span>   |<span data-ttu-id="9fcd6-127">説明</span><span class="sxs-lookup"><span data-stu-id="9fcd6-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9fcd6-128">activeChecklistItemCount</span><span class="sxs-lookup"><span data-stu-id="9fcd6-128">activeChecklistItemCount</span></span>|<span data-ttu-id="9fcd6-129">Int32</span><span class="sxs-lookup"><span data-stu-id="9fcd6-129">Int32</span></span>|<span data-ttu-id="9fcd6-130">チェックリストの項目数。値が `false` である場合は、不完全な項目があることを示します。</span><span class="sxs-lookup"><span data-stu-id="9fcd6-130">Number of checklist items with value set to `false`, representing incomplete items.</span></span>|
|<span data-ttu-id="9fcd6-131">appliedCategories</span><span class="sxs-lookup"><span data-stu-id="9fcd6-131">appliedCategories</span></span>|[<span data-ttu-id="9fcd6-132">plannerAppliedCategories</span><span class="sxs-lookup"><span data-stu-id="9fcd6-132">plannerAppliedCategories</span></span>](plannerappliedcategories.md)|<span data-ttu-id="9fcd6-p103">タスクが適用されているカテゴリ。可能な値については、「[適用されるカテゴリ](plannerappliedcategories.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9fcd6-p103">The categories to which the task has been applied. See [applied Categories](plannerappliedcategories.md) for possible values.</span></span>|
|<span data-ttu-id="9fcd6-135">assigneePriority</span><span class="sxs-lookup"><span data-stu-id="9fcd6-135">assigneePriority</span></span>|<span data-ttu-id="9fcd6-136">String</span><span class="sxs-lookup"><span data-stu-id="9fcd6-136">String</span></span>|<span data-ttu-id="9fcd6-p104">リスト ビューでこの種類の項目の順序付けに使用するヒント。形式は[ここ](planner-order-hint-format.md)の説明に従って定義されます。</span><span class="sxs-lookup"><span data-stu-id="9fcd6-p104">Hint used to order items of this type in a list view. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="9fcd6-139">assignments</span><span class="sxs-lookup"><span data-stu-id="9fcd6-139">assignments</span></span>|[<span data-ttu-id="9fcd6-140">plannerAssignments</span><span class="sxs-lookup"><span data-stu-id="9fcd6-140">plannerAssignments</span></span>](plannerassignments.md)|<span data-ttu-id="9fcd6-141">タスクが割り当てられている一連の担当者。</span><span class="sxs-lookup"><span data-stu-id="9fcd6-141">The set of assignees the task is assigned to.</span></span>|
|<span data-ttu-id="9fcd6-142">bucketId</span><span class="sxs-lookup"><span data-stu-id="9fcd6-142">bucketId</span></span>|<span data-ttu-id="9fcd6-143">String</span><span class="sxs-lookup"><span data-stu-id="9fcd6-143">String</span></span>|<span data-ttu-id="9fcd6-144">タスクが属しているバケット ID。</span><span class="sxs-lookup"><span data-stu-id="9fcd6-144">Bucket ID to which the task belongs.</span></span> <span data-ttu-id="9fcd6-145">バケットは、タスクが存在している計画に含まれている必要があります。</span><span class="sxs-lookup"><span data-stu-id="9fcd6-145">The bucket needs to be in the plan that the task is in.</span></span> <span data-ttu-id="9fcd6-146">28 文字長で、大文字と小文字の区別があります。</span><span class="sxs-lookup"><span data-stu-id="9fcd6-146">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="9fcd6-147">[書式検証](tasks-identifiers-disclaimer.md)はサービスによって行われます。</span><span class="sxs-lookup"><span data-stu-id="9fcd6-147">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span> |
|<span data-ttu-id="9fcd6-148">checklistItemCount</span><span class="sxs-lookup"><span data-stu-id="9fcd6-148">checklistItemCount</span></span>|<span data-ttu-id="9fcd6-149">Int32</span><span class="sxs-lookup"><span data-stu-id="9fcd6-149">Int32</span></span>|<span data-ttu-id="9fcd6-150">タスクに存在するチェックリストの項目の数です。</span><span class="sxs-lookup"><span data-stu-id="9fcd6-150">Number of checklist items that are present on the task.</span></span>|
|<span data-ttu-id="9fcd6-151">completedBy</span><span class="sxs-lookup"><span data-stu-id="9fcd6-151">completedBy</span></span>|[<span data-ttu-id="9fcd6-152">identitySet</span><span class="sxs-lookup"><span data-stu-id="9fcd6-152">identitySet</span></span>](identityset.md)|<span data-ttu-id="9fcd6-153">タスクを完了したユーザーの ID。</span><span class="sxs-lookup"><span data-stu-id="9fcd6-153">Identity of the user that completed the task.</span></span>|
|<span data-ttu-id="9fcd6-154">CompletedDateTime</span><span class="sxs-lookup"><span data-stu-id="9fcd6-154">completedDateTime</span></span>|<span data-ttu-id="9fcd6-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9fcd6-155">DateTimeOffset</span></span>|<span data-ttu-id="9fcd6-p106">読み取り専用。タスクの `'percentComplete'` が `'100'` にセットされる日時。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="9fcd6-p106">Read-only. Date and time at which the `'percentComplete'` of the task is set to `'100'`. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="9fcd6-160">conversationThreadId</span><span class="sxs-lookup"><span data-stu-id="9fcd6-160">conversationThreadId</span></span>|<span data-ttu-id="9fcd6-161">String</span><span class="sxs-lookup"><span data-stu-id="9fcd6-161">String</span></span>|<span data-ttu-id="9fcd6-p107">タスク内の会話のスレッド ID。これは、グループ内に作成された会話スレッド オブジェクトの ID です。</span><span class="sxs-lookup"><span data-stu-id="9fcd6-p107">Thread ID of the conversation on the task. This is the ID of the conversation thread object created in the group.</span></span>|
|<span data-ttu-id="9fcd6-164">createdBy</span><span class="sxs-lookup"><span data-stu-id="9fcd6-164">createdBy</span></span>|[<span data-ttu-id="9fcd6-165">identitySet</span><span class="sxs-lookup"><span data-stu-id="9fcd6-165">identitySet</span></span>](identityset.md)|<span data-ttu-id="9fcd6-166">タスクを作成したユーザーの ID。</span><span class="sxs-lookup"><span data-stu-id="9fcd6-166">Identity of the user that created the task.</span></span>|
|<span data-ttu-id="9fcd6-167">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9fcd6-167">createdDateTime</span></span>|<span data-ttu-id="9fcd6-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9fcd6-168">DateTimeOffset</span></span>|<span data-ttu-id="9fcd6-p108">読み取り専用。タスクが作成された日時。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="9fcd6-p108">Read-only. Date and time at which the task is created. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="9fcd6-173">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="9fcd6-173">dueDateTime</span></span>|<span data-ttu-id="9fcd6-174">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9fcd6-174">DateTimeOffset</span></span>|<span data-ttu-id="9fcd6-p109">タスクが期限切れになる日時。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="9fcd6-p109">Date and time at which the task is due. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="9fcd6-178">hasDescription</span><span class="sxs-lookup"><span data-stu-id="9fcd6-178">hasDescription</span></span>|<span data-ttu-id="9fcd6-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="9fcd6-179">Boolean</span></span>|<span data-ttu-id="9fcd6-p110">読み取り専用。タスクの details オブジェクトが保持する説明が空でない場合、値は `true` になり、そうでない場合は `false` になります。</span><span class="sxs-lookup"><span data-stu-id="9fcd6-p110">Read-only. Value is `true` if the details object of the task has a non-empty description and `false` otherwise.</span></span>|
|<span data-ttu-id="9fcd6-182">id</span><span class="sxs-lookup"><span data-stu-id="9fcd6-182">id</span></span>|<span data-ttu-id="9fcd6-183">String</span><span class="sxs-lookup"><span data-stu-id="9fcd6-183">String</span></span>|<span data-ttu-id="9fcd6-184">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="9fcd6-184">Read-only.</span></span> <span data-ttu-id="9fcd6-185">タスクの ID。</span><span class="sxs-lookup"><span data-stu-id="9fcd6-185">ID of the task.</span></span> <span data-ttu-id="9fcd6-186">28 文字長で、大文字と小文字の区別があります。</span><span class="sxs-lookup"><span data-stu-id="9fcd6-186">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="9fcd6-187">[書式検証](tasks-identifiers-disclaimer.md)はサービスによって行われます。</span><span class="sxs-lookup"><span data-stu-id="9fcd6-187">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="9fcd6-188">orderHint</span><span class="sxs-lookup"><span data-stu-id="9fcd6-188">orderHint</span></span>|<span data-ttu-id="9fcd6-189">String</span><span class="sxs-lookup"><span data-stu-id="9fcd6-189">String</span></span>|<span data-ttu-id="9fcd6-p112">リスト ビューでこの種類の項目の順序付けに使用するヒント。形式は[ここ](planner-order-hint-format.md)の説明に従って定義されます。</span><span class="sxs-lookup"><span data-stu-id="9fcd6-p112">Hint used to order items of this type in a list view. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="9fcd6-192">percentComplete</span><span class="sxs-lookup"><span data-stu-id="9fcd6-192">percentComplete</span></span>|<span data-ttu-id="9fcd6-193">Int32</span><span class="sxs-lookup"><span data-stu-id="9fcd6-193">Int32</span></span>|<span data-ttu-id="9fcd6-p113">タスクの完了の割合。`100` に設定すると、タスクが完了したと見なされます。</span><span class="sxs-lookup"><span data-stu-id="9fcd6-p113">Percentage of task completion. When set to `100`, the task is considered completed.</span></span> |
|<span data-ttu-id="9fcd6-196">planId</span><span class="sxs-lookup"><span data-stu-id="9fcd6-196">planId</span></span>|<span data-ttu-id="9fcd6-197">String</span><span class="sxs-lookup"><span data-stu-id="9fcd6-197">String</span></span>|<span data-ttu-id="9fcd6-198">タスクが属している計画 ID。</span><span class="sxs-lookup"><span data-stu-id="9fcd6-198">Plan ID to which the task belongs.</span></span>|
|<span data-ttu-id="9fcd6-199">previewType</span><span class="sxs-lookup"><span data-stu-id="9fcd6-199">previewType</span></span>|<span data-ttu-id="9fcd6-200">String</span><span class="sxs-lookup"><span data-stu-id="9fcd6-200">String</span></span>|<span data-ttu-id="9fcd6-201">タスクに表示されるプレビューの種類を設定します。</span><span class="sxs-lookup"><span data-stu-id="9fcd6-201">This sets the type of preview that shows up on the task.</span></span> <span data-ttu-id="9fcd6-202">可能な値は、`automatic`、`noPreview`、`checklist`、`description`、`reference` です。</span><span class="sxs-lookup"><span data-stu-id="9fcd6-202">Possible values are: `automatic`, `noPreview`, `checklist`, `description`, `reference`.</span></span>|
|<span data-ttu-id="9fcd6-203">referenceCount</span><span class="sxs-lookup"><span data-stu-id="9fcd6-203">referenceCount</span></span>|<span data-ttu-id="9fcd6-204">Int32</span><span class="sxs-lookup"><span data-stu-id="9fcd6-204">Int32</span></span>|<span data-ttu-id="9fcd6-205">タスクに上に存在している外部への参照の数。</span><span class="sxs-lookup"><span data-stu-id="9fcd6-205">Number of external references that exist on the task.</span></span>|
|<span data-ttu-id="9fcd6-206">startDateTime</span><span class="sxs-lookup"><span data-stu-id="9fcd6-206">startDateTime</span></span>|<span data-ttu-id="9fcd6-207">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9fcd6-207">DateTimeOffset</span></span>|<span data-ttu-id="9fcd6-p115">タスクが開始される日時。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="9fcd6-p115">Date and time at which the task starts. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="9fcd6-211">title</span><span class="sxs-lookup"><span data-stu-id="9fcd6-211">title</span></span>|<span data-ttu-id="9fcd6-212">String</span><span class="sxs-lookup"><span data-stu-id="9fcd6-212">String</span></span>|<span data-ttu-id="9fcd6-213">タスクのタイトル。</span><span class="sxs-lookup"><span data-stu-id="9fcd6-213">Title of the task.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9fcd6-214">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="9fcd6-214">Relationships</span></span>
| <span data-ttu-id="9fcd6-215">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="9fcd6-215">Relationship</span></span> | <span data-ttu-id="9fcd6-216">型</span><span class="sxs-lookup"><span data-stu-id="9fcd6-216">Type</span></span>   |<span data-ttu-id="9fcd6-217">説明</span><span class="sxs-lookup"><span data-stu-id="9fcd6-217">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9fcd6-218">assignedToTaskBoardFormat</span><span class="sxs-lookup"><span data-stu-id="9fcd6-218">assignedToTaskBoardFormat</span></span>|[<span data-ttu-id="9fcd6-219">plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="9fcd6-219">plannerAssignedToTaskBoardTaskFormat</span></span>](plannerassignedtotaskboardtaskformat.md)| <span data-ttu-id="9fcd6-p116">読み取り専用。Null 許容型。assignedTo 別にグループ化されるときに、タスク ボード ビューにタスクを正しくレンダリングするために使用されます。</span><span class="sxs-lookup"><span data-stu-id="9fcd6-p116">Read-only. Nullable. Used to render the task correctly in the task board view when grouped by assignedTo.</span></span>|
|<span data-ttu-id="9fcd6-223">bucketTaskBoardFormat</span><span class="sxs-lookup"><span data-stu-id="9fcd6-223">bucketTaskBoardFormat</span></span>|[<span data-ttu-id="9fcd6-224">plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="9fcd6-224">plannerBucketTaskBoardTaskFormat</span></span>](plannerbuckettaskboardtaskformat.md)| <span data-ttu-id="9fcd6-p117">読み取り専用。Null 許容型。バケット別にグループ化されるときに、タスク ボード ビューにタスクを正しくレンダリングするために使用されます。</span><span class="sxs-lookup"><span data-stu-id="9fcd6-p117">Read-only. Nullable. Used to render the task correctly in the task board view when grouped by bucket.</span></span>|
|<span data-ttu-id="9fcd6-228">詳細</span><span class="sxs-lookup"><span data-stu-id="9fcd6-228">details</span></span>|[<span data-ttu-id="9fcd6-229">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="9fcd6-229">plannerTaskDetails</span></span>](plannertaskdetails.md)| <span data-ttu-id="9fcd6-p118">読み取り専用。Null 許容型。タスクに関する追加の詳細。</span><span class="sxs-lookup"><span data-stu-id="9fcd6-p118">Read-only. Nullable. Additional details about the task.</span></span>|
|<span data-ttu-id="9fcd6-233">progressTaskBoardFormat</span><span class="sxs-lookup"><span data-stu-id="9fcd6-233">progressTaskBoardFormat</span></span>|[<span data-ttu-id="9fcd6-234">plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="9fcd6-234">plannerProgressTaskBoardTaskFormat</span></span>](plannerprogresstaskboardtaskformat.md)| <span data-ttu-id="9fcd6-p119">読み取り専用。Null 許容型。進捗状態別にグループ化されるときに、タスク ボード ビューにタスクを正しくレンダリングするために使用されます。</span><span class="sxs-lookup"><span data-stu-id="9fcd6-p119">Read-only. Nullable. Used to render the task correctly in the task board view when grouped by progress.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9fcd6-238">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9fcd6-238">JSON representation</span></span>
<span data-ttu-id="9fcd6-239">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="9fcd6-239">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",  
  "@odata.type": "microsoft.graph.plannerTask"
}-->

```json
{
  "activeChecklistItemCount": 1024,
  "appliedCategories": {"@odata.type": "microsoft.graph.plannerAppliedCategories"},
  "assigneePriority": "String",
  "assignments": {"@odata.type": "microsoft.graph.plannerAssignments"},
  "bucketId": "String",
  "checklistItemCount": 1024,
  "completedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "completedDateTime": "String (timestamp)",
  "conversationThreadId": "String",
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "dueDateTime": "String (timestamp)",
  "hasDescription": true,
  "id": "String (identifier)",
  "orderHint": "String",
  "percentComplete": 1024,
  "planId": "String",
  "previewType": "String",
  "referenceCount": 1024,
  "startDateTime": "String (timestamp)",
  "title": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerTask resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
