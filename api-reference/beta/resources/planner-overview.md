---
title: プランナーの REST API を使用します。
description: Graph でプランナーの API を使用するにはタスクを作成し、Office 365 で、グループ内のユーザーに割り当てます。
author: TarkanSevilmis
ms.openlocfilehash: a57bdce9c61046d05bc969ff69d31971a85cf537
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27346740"
---
# <a name="use-the-planner-rest-api"></a><span data-ttu-id="54e0f-103">プランナーの REST API を使用します。</span><span class="sxs-lookup"><span data-stu-id="54e0f-103">Use the Planner REST API</span></span>

> <span data-ttu-id="54e0f-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="54e0f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="54e0f-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="54e0f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="54e0f-106">Graph でプランナーの API を使用するにはタスクを作成し、Office 365 で、グループ内のユーザーに割り当てます。</span><span class="sxs-lookup"><span data-stu-id="54e0f-106">You can use the Planner API in Microsoft Graph to create tasks and assign them to users in a group in Office 365.</span></span>

<span data-ttu-id="54e0f-107">プランナーの API を使用して開始する前に互いにも Office 365 のグループを主なオブジェクトの関係を理解するおくと便利になります。</span><span class="sxs-lookup"><span data-stu-id="54e0f-107">Before you get started with the Planner API, it will be helpful to understand how the main objects relate to each other as well as to Office 365 groups.</span></span>

## <a name="office-365-groups"></a><span data-ttu-id="54e0f-108">Office 365 グループ</span><span class="sxs-lookup"><span data-stu-id="54e0f-108">Office 365 Groups</span></span>

<span data-ttu-id="54e0f-109">Office 365 のグループは、プランナーの API で、計画の所有者です。</span><span class="sxs-lookup"><span data-stu-id="54e0f-109">Office 365 groups are the owners of the plans in the Planner API.</span></span>
<span data-ttu-id="54e0f-110">[グループによって所有されているプランを取得する](../api/plannergroup-list-plans.md)には、次の HTTP 要求を確認します。</span><span class="sxs-lookup"><span data-stu-id="54e0f-110">To [get the plans owned by a group](../api/plannergroup-list-plans.md), make the following HTTP request.</span></span>

``` http
GET /groups/{id}/planner/plans
```

<span data-ttu-id="54e0f-111">[新しい計画を作成する](../api/planner-post-plans.md)をグループにする、その所有者を設定することにより、 `owner` 、プラン オブジェクトのプロパティです。</span><span class="sxs-lookup"><span data-stu-id="54e0f-111">When [creating a new plan](../api/planner-post-plans.md), make a group its owner by setting the `owner` property on a plan object.</span></span> <span data-ttu-id="54e0f-112">プランは、グループが所有する必要があります。</span><span class="sxs-lookup"><span data-stu-id="54e0f-112">Plans must be owned by groups.</span></span>

><span data-ttu-id="54e0f-113">**注:** 計画を作成しているユーザーは、計画を所有するグループのメンバーである必要があります。</span><span class="sxs-lookup"><span data-stu-id="54e0f-113">**Note:** The user who is creating the plan must be a member of the group that will own the plan.</span></span> <span data-ttu-id="54e0f-114">[グループの作成](../api/group-post-groups.md)を使用して新しいグループを作成するときにいない追加されますグループにメンバーとして。</span><span class="sxs-lookup"><span data-stu-id="54e0f-114">When you create a new group by using [Create group](../api/group-post-groups.md), you are not added to the group as a member.</span></span> <span data-ttu-id="54e0f-115">グループが作成されると、自分自身を追加メンバーとして[グループのメンバーの投稿](../api/group-post-members.md)を使用しています。</span><span class="sxs-lookup"><span data-stu-id="54e0f-115">After the group is created, add yourself as a member by using [group post members](../api/group-post-members.md).</span></span>

## <a name="plans"></a><span data-ttu-id="54e0f-116">プラン</span><span class="sxs-lookup"><span data-stu-id="54e0f-116">Plans</span></span>

<span data-ttu-id="54e0f-117">[計画](plannerplan.md)は、[タスク](plannertask.md)のコンテナーです。</span><span class="sxs-lookup"><span data-stu-id="54e0f-117">[Plans](plannerplan.md) are the containers of [tasks](plannertask.md).</span></span> <span data-ttu-id="54e0f-118">[計画にタスクを作成](../api/planner-post-tasks.md)するには、設定、 `planId` 、タスクの作成中に計画の ID をタスク オブジェクトのプロパティです。</span><span class="sxs-lookup"><span data-stu-id="54e0f-118">To [create a task in a plan](../api/planner-post-tasks.md), set the `planId` property on the task object to the ID of the plan while creating the task.</span></span>
<span data-ttu-id="54e0f-119">現在のタスクを計画しなくても作成できません。</span><span class="sxs-lookup"><span data-stu-id="54e0f-119">Tasks currently cannot be created without plans.</span></span>
<span data-ttu-id="54e0f-120">[計画内のタスクを取得](../api/plannerplan-list-tasks.md)するには、次の HTTP 要求を確認します。</span><span class="sxs-lookup"><span data-stu-id="54e0f-120">To [retrieve the tasks in a plan](../api/plannerplan-list-tasks.md), make the following HTTP request.</span></span>

``` http
GET /planner/plans/{id}/tasks
```

## <a name="tasks"></a><span data-ttu-id="54e0f-121">タスク</span><span class="sxs-lookup"><span data-stu-id="54e0f-121">Tasks</span></span>

<span data-ttu-id="54e0f-p106">各タスクは、タスク オブジェクトの [assignments](plannerassignments.md) プロパティに [assignment](plannerassignment.md) を追加することにより、ユーザーに割り当てることができます。タスクを割り当てるユーザーの ID は `assignments` の open プロパティの名前であり、assignment の `orderHint` プロパティを指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="54e0f-p106">Each task can be assigned to a user by adding an [assignment](plannerassignment.md) in the [assignments](plannerassignments.md) property on the task object. The ID of the user to assign the task is the name of the open property on `assignments`, and the `orderHint` property on the assignment must be specified.</span></span>

## <a name="task-and-plan-details"></a><span data-ttu-id="54e0f-124">タスクとプランの詳細</span><span class="sxs-lookup"><span data-stu-id="54e0f-124">Task and plan details</span></span> 

<span data-ttu-id="54e0f-p107">Planner のリソースは、基本オブジェクトと詳細オブジェクトに配置されます。基本オブジェクトは、リスト ビューに適したリソースの共通プロパティへのアクセスを提供し、詳細オブジェクトは、ドリル ダウン ビューに適したリソースの大規模なプロパティへのアクセスを提供します。</span><span class="sxs-lookup"><span data-stu-id="54e0f-p107">Planner resources are arranged into basic objects and detail objects. Basic objects provide access to common properties of the resources, suitable for list views, while the detail objects provide access to large properties of the resources suitable for drill down views.</span></span>

## <a name="visualization"></a><span data-ttu-id="54e0f-127">視覚化</span><span class="sxs-lookup"><span data-stu-id="54e0f-127">Visualization</span></span>

<span data-ttu-id="54e0f-128">作業および計画のデータは別にプランナー API はクライアント間でデータの一般的な視覚エフェクトを作成するためのリソースも備えています。</span><span class="sxs-lookup"><span data-stu-id="54e0f-128">Aside from task and plan data, the Planner API also provides resources for creating a common visualization of data across clients.</span></span> <span data-ttu-id="54e0f-129">ビジュアル化データのいくつかの種類があるタスクについては、次の表に記載されています。</span><span class="sxs-lookup"><span data-stu-id="54e0f-129">Several types of visualization data are available for tasks, as listed in the following table.</span></span>

| <span data-ttu-id="54e0f-130">タスクの表示</span><span class="sxs-lookup"><span data-stu-id="54e0f-130">Tasks are shown as</span></span>                                                                        | <span data-ttu-id="54e0f-131">タスクを順序付ける情報の情報源</span><span class="sxs-lookup"><span data-stu-id="54e0f-131">Tasks are ordered with information from</span></span>                                         |
| :---------------------------------------------------------------------------------------- | :------------------------------------------------------------------------------ |
| <span data-ttu-id="54e0f-132">フラット リスト (プラン内のタスク)</span><span class="sxs-lookup"><span data-stu-id="54e0f-132">Flat list (tasks in a plan)</span></span>                                                               | <span data-ttu-id="54e0f-133">タスクの `orderHint` プロパティ</span><span class="sxs-lookup"><span data-stu-id="54e0f-133">`orderHint` property on tasks</span></span>                                                   |
| <span data-ttu-id="54e0f-134">フラット リスト (ユーザーに割り当てられたタスク)</span><span class="sxs-lookup"><span data-stu-id="54e0f-134">Flat list (tasks assigned to a user)</span></span>                                                      | <span data-ttu-id="54e0f-135">タスクの `assigneePriority` プロパティ</span><span class="sxs-lookup"><span data-stu-id="54e0f-135">`assigneePriority` property on tasks</span></span>                                            |
| <span data-ttu-id="54e0f-136">割り当て先の列を含むボード ビュー (タスク ボードに割り当て)</span><span class="sxs-lookup"><span data-stu-id="54e0f-136">Board view with columns for assignees (assigned to task board)</span></span>                            | <span data-ttu-id="54e0f-137">[assignedToTaskBoardTaskFormat](plannerassignedtotaskboardtaskformat.md) オブジェクト</span><span class="sxs-lookup"><span data-stu-id="54e0f-137">[assignedToTaskBoardTaskFormat](plannerassignedtotaskboardtaskformat.md) object</span></span> |
| <span data-ttu-id="54e0f-138">タスクの進行状況を示す列を含むボード ビュー (進行状況タスク ボード)</span><span class="sxs-lookup"><span data-stu-id="54e0f-138">Board view with columns for progress of the task towards completion (progress task board)</span></span> | <span data-ttu-id="54e0f-139">[progressTaskBoardTaskFormat](plannerprogresstaskboardtaskformat.md)オブジェクト</span><span class="sxs-lookup"><span data-stu-id="54e0f-139">[progressTaskBoardTaskFormat](plannerprogresstaskboardtaskformat.md) object</span></span>     |
| <span data-ttu-id="54e0f-140">タスクのカスタム列を含むボード ビュー (バケット タスク ボード)</span><span class="sxs-lookup"><span data-stu-id="54e0f-140">Board view with custom columns of tasks (bucket task board):</span></span>                              | <span data-ttu-id="54e0f-141">[bucketTaskBoardTaskFormat](plannerbuckettaskboardtaskformat.md) オブジェクト</span><span class="sxs-lookup"><span data-stu-id="54e0f-141">[bucketTaskBoardTaskFormat](plannerbuckettaskboardtaskformat.md) object</span></span>         |

<span data-ttu-id="54e0f-142">バケット タスク ボードのカスタム列は [bucket](plannerbucket.md) オブジェクトで表され、その順序はオブジェクトの `orderHint` プロパティによって表されます。</span><span class="sxs-lookup"><span data-stu-id="54e0f-142">The custom columns in the bucket task board are represented by [bucket](plannerbucket.md) objects, and their order by `orderHint` property on the object.</span></span>

<span data-ttu-id="54e0f-143">[プランナーの順序のヒント](planner-order-hint-format.md)で説明した原則には、すべての順序が制御されます。</span><span class="sxs-lookup"><span data-stu-id="54e0f-143">All the ordering is controlled by the principles described in [Planner order hints](planner-order-hint-format.md).</span></span>

## <span data-ttu-id="54e0f-144"><a name="delta">デルタのクエリを使用して変更履歴の記録します。</a></span><span class="sxs-lookup"><span data-stu-id="54e0f-144"><a name="delta">Track changes using delta query</a></span></span>

<span data-ttu-id="54e0f-145">プランナーのデルタのクエリは、ユーザーが購読しているオブジェクトのクエリをサポートしています。</span><span class="sxs-lookup"><span data-stu-id="54e0f-145">Planner's delta query supports querying objects that the user is subscribed to.</span></span>

<span data-ttu-id="54e0f-146">ユーザーは、次のオブジェクトを購読します。</span><span class="sxs-lookup"><span data-stu-id="54e0f-146">Users are subscribed to the following objects.</span></span>

| <span data-ttu-id="54e0f-147">プランナーのリソースの種類</span><span class="sxs-lookup"><span data-stu-id="54e0f-147">Planner resource type</span></span> | <span data-ttu-id="54e0f-148">購読済みのインスタンス</span><span class="sxs-lookup"><span data-stu-id="54e0f-148">Subscribed instances</span></span>                                                                                                                                                                                    |
| :-------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="54e0f-149">タスク</span><span class="sxs-lookup"><span data-stu-id="54e0f-149">Tasks</span></span>                 | <ul><li><span data-ttu-id="54e0f-150">ユーザーによって作成されました。</span><span class="sxs-lookup"><span data-stu-id="54e0f-150">Created by the user</span></span></li><li><span data-ttu-id="54e0f-151">ユーザーに割り当てられています。</span><span class="sxs-lookup"><span data-stu-id="54e0f-151">Assigned to the user</span></span></li><li><span data-ttu-id="54e0f-152">ユーザーが所有する計画に属しています。</span><span class="sxs-lookup"><span data-stu-id="54e0f-152">Belong to a plan that the user owns</span></span></li><li><span data-ttu-id="54e0f-153">計画の**SharedWith**コレクションをユーザーと共有の計画に含まれています。</span><span class="sxs-lookup"><span data-stu-id="54e0f-153">Contained in a plan shared with the user through the plan's **SharedWith** collection</span></span></li> |
| <span data-ttu-id="54e0f-154">プラン</span><span class="sxs-lookup"><span data-stu-id="54e0f-154">Plans</span></span>                 | <ul><li><span data-ttu-id="54e0f-155">計画の**SharedWith**コレクションをユーザーと共有</span><span class="sxs-lookup"><span data-stu-id="54e0f-155">Shared with the user through the plan's **SharedWith** collection</span></span></li></ul>                                                                                                                     |
| <span data-ttu-id="54e0f-156">バケット</span><span class="sxs-lookup"><span data-stu-id="54e0f-156">Buckets</span></span>               | <ul><li><span data-ttu-id="54e0f-157">計画の**SharedWith**コレクションをユーザーと共有の計画に含まれています。</span><span class="sxs-lookup"><span data-stu-id="54e0f-157">Contained in a plan shared with the user through the plan's **SharedWith** collection</span></span></li></ul>                                                                                                 |  |

### <span data-ttu-id="54e0f-158"><a name="objectcache">デルタ ・ クエリのオブジェクト キャッシュを設定します。</a></span><span class="sxs-lookup"><span data-stu-id="54e0f-158"><a name="objectcache">Populate the object cache for delta queries</a></span></span>

<span data-ttu-id="54e0f-159">プランナーのデルタ ・ クエリ API を使用する場合は、デルタの応答フィードから変更を適用するために観察することで、ユーザーが興味を示しているオブジェクトのローカル キャッシュを保持します。</span><span class="sxs-lookup"><span data-stu-id="54e0f-159">If you want to use the Planner delta query API, maintain a local cache of objects that the user is interested in observing in order to apply the changes from the delta response feed.</span></span>

<span data-ttu-id="54e0f-160">次の種類のプランナーのデルタ ・ クエリが返すことができる現在のデルタ ・ ペイロード オブジェクトになります。</span><span class="sxs-lookup"><span data-stu-id="54e0f-160">The delta payload objects that the Planner delta query can currently return will be of the following types:</span></span>

* [<span data-ttu-id="54e0f-161">plannerTask</span><span class="sxs-lookup"><span data-stu-id="54e0f-161">plannerTask</span></span>](plannertask.md)
* [<span data-ttu-id="54e0f-162">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="54e0f-162">plannerTaskDetails</span></span>](plannertaskdetails.md)
* [<span data-ttu-id="54e0f-163">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="54e0f-163">plannerPlan</span></span>](plannerplan.md)
* [<span data-ttu-id="54e0f-164">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="54e0f-164">plannerPlanDetails</span></span>](plannerplandetails.md)
* [<span data-ttu-id="54e0f-165">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="54e0f-165">plannerBucket</span></span>](plannerbucket.md)
* [<span data-ttu-id="54e0f-166">plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="54e0f-166">plannerAssignedToTaskBoardTaskFormat</span></span>](plannerassignedtotaskboardtaskformat.md)
* [<span data-ttu-id="54e0f-167">plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="54e0f-167">plannerBucketTaskBoardTaskFormat</span></span>](plannerbuckettaskboardtaskformat.md)
* [<span data-ttu-id="54e0f-168">plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="54e0f-168">plannerAssignedToTaskBoardTaskFormat</span></span>](plannerassignedtotaskboardtaskformat.md)

<span data-ttu-id="54e0f-169">使用して、対応する`GET`のリソースをローカルのキャッシュを格納するオブジェクトの初期状態を取得するメソッドです。</span><span class="sxs-lookup"><span data-stu-id="54e0f-169">Use the corresponding `GET` methods on the resource to obtain the initial state of objects to be populated into the local cache.</span></span>

### <a name="differentiating-between-object-creation-and-object-modification"></a><span data-ttu-id="54e0f-170">オブジェクトの作成とオブジェクトの変更の違いを知る</span><span class="sxs-lookup"><span data-stu-id="54e0f-170">Differentiating between object creation and object modification</span></span>

<span data-ttu-id="54e0f-171">特定のシナリオでは、呼び出し元がオブジェクトを作成し、フィードのプランナーのデルタのクエリ内のオブジェクトの変更を区別する必要があります。</span><span class="sxs-lookup"><span data-stu-id="54e0f-171">In certain scenarios, the caller might want to distinguish between object creation and object modification within Planner's delta query feed.</span></span>

<span data-ttu-id="54e0f-172">これらのガイドラインを使用して、オブジェクトの作成を推論することができます。</span><span class="sxs-lookup"><span data-stu-id="54e0f-172">These guidelines can be used to infer object creation:</span></span>

* <span data-ttu-id="54e0f-173">`createdBy`プロパティは、新しく作成されたオブジェクトにのみ表示されます。</span><span class="sxs-lookup"><span data-stu-id="54e0f-173">The `createdBy` property will only appear on newly created objects.</span></span>
* <span data-ttu-id="54e0f-174">新しく作成された A`plannerTask`オブジェクトに対応する、続いて`plannerTaskDetails`オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="54e0f-174">A newly created `plannerTask` object will be followed by its corresponding `plannerTaskDetails` object.</span></span>
* <span data-ttu-id="54e0f-175">新しく作成された A`plannerPlan`オブジェクトに対応する、続いて`plannerPlanDetails`オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="54e0f-175">A newly created `plannerPlan` object will be followed by its corresponding `plannerPlanDetails` object.</span></span>

### <a name="usage"></a><span data-ttu-id="54e0f-176">使用方法</span><span class="sxs-lookup"><span data-stu-id="54e0f-176">Usage</span></span>

<span data-ttu-id="54e0f-177">呼び出し元は、購読しているオブジェクトが含まれているキャッシュを持つと思われます。</span><span class="sxs-lookup"><span data-stu-id="54e0f-177">The caller is expected to have a cache containing subscribed objects.</span></span> <span data-ttu-id="54e0f-178">購読しているオブジェクトのローカル キャッシュを設定する方法についての詳細は、[デルタのクエリでオブジェクト キャッシュの作成](#populate-the-object-cache-for-delta-queries)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="54e0f-178">For details about how to fill the local cache of subscribed objects, see [Populate the object cache for delta queries](#populate-the-object-cache-for-delta-queries).</span></span>

<span data-ttu-id="54e0f-179">プランナーのデルタのクエリの呼び出しのフローは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="54e0f-179">Planner's delta query call flow is as follows:</span></span>

1. <span data-ttu-id="54e0f-180">デルタ同期クエリを開始する呼び出し元を取得する、`nextLink`と変更の空のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="54e0f-180">The caller initiates a delta sync query, obtaining a `nextLink` and an empty collection of changes.</span></span>
2. <span data-ttu-id="54e0f-181">呼び出し元する必要があります[デルタ クエリでオブジェクト キャッシュの設定](#populate-the-object-cache-for-delta-queries)とオブジェクトをユーザーが購読して、そのキャッシュを更新します。</span><span class="sxs-lookup"><span data-stu-id="54e0f-181">The caller must [populate the object cache for delta queries](#populate-the-object-cache-for-delta-queries) with objects that the user is subscribed to, updating its cache.</span></span>
3. <span data-ttu-id="54e0f-182">呼び出し元に依存して、 `nextLink` 、新しいを取得する最初のデルタ ・同期クエリで提供されている`deltaLink`前の手順の変更を反映します。</span><span class="sxs-lookup"><span data-stu-id="54e0f-182">The caller follows the `nextLink` provided in the initial delta sync query to obtain a new `deltaLink` to any changes since previous step.</span></span>
4. <span data-ttu-id="54e0f-183">呼び出し元に返されたデルタのキャッシュ内のオブジェクトに対して変更が適用されます。</span><span class="sxs-lookup"><span data-stu-id="54e0f-183">The caller applies the changes in the returned delta response to the objects in its cache.</span></span>
5. <span data-ttu-id="54e0f-184">呼び出し元は、次の deltaLink を取得する新しい deltaLink に依存して、現在以降の変更`deltaLink`が生成されました。</span><span class="sxs-lookup"><span data-stu-id="54e0f-184">The caller follows the new deltaLink to obtain the next deltaLink and changes since the current `deltaLink` was generated.</span></span>
6. <span data-ttu-id="54e0f-185">呼び出し元が (もしあれば) 変更が適用され、短時間を待機する前に実行する前にステップし、この手順です。</span><span class="sxs-lookup"><span data-stu-id="54e0f-185">The caller applies the changes (if any) and waits a short time before rerunning the previous step and this step.</span></span>

## <a name="planner-resource-versioning"></a><span data-ttu-id="54e0f-186">Planner のリソースのバージョン管理</span><span class="sxs-lookup"><span data-stu-id="54e0f-186">Planner resource versioning</span></span>

<span data-ttu-id="54e0f-187">プランナーのバージョンすべてのリソースの**etag**を使用します。</span><span class="sxs-lookup"><span data-stu-id="54e0f-187">Planner versions all resources using **etags**.</span></span> <span data-ttu-id="54e0f-188">返されるこれらの**etag**が`@odata.etag`の各リソースのプロパティです。</span><span class="sxs-lookup"><span data-stu-id="54e0f-188">These **etags** are returned with `@odata.etag` property on each resource.</span></span> <span data-ttu-id="54e0f-189">`PATCH``DELETE`を使用して指定するのには既知のクライアントによって最後の**etag**を要求、`If-Match`ヘッダー。</span><span class="sxs-lookup"><span data-stu-id="54e0f-189">`PATCH` and `DELETE` requests require the last **etag** known by the client to be specified with a `If-Match` header.</span></span>
<span data-ttu-id="54e0f-190">プランナーは、目的の変更が新しい変更を受け入れ、プランナーのサービスで同じリソースと競合していない場合、古いバージョンのリソースへの変更を使用できます。</span><span class="sxs-lookup"><span data-stu-id="54e0f-190">Planner allows changes to older versions of resources, if the intended change does not conflict with newer changes accepted by the Planner service on the same resource.</span></span> <span data-ttu-id="54e0f-191">**Etag**値が大きい序数の文字列比較で計算することで同じリソースの**etag**のどちらの方が新しいクライアントを識別できます。</span><span class="sxs-lookup"><span data-stu-id="54e0f-191">The clients can identify which **etag** for the same resource is newer by calculating which **etag** value is greater in ordinal string comparison.</span></span> <span data-ttu-id="54e0f-192">各リソースには、独自の**etag**があります。</span><span class="sxs-lookup"><span data-stu-id="54e0f-192">Each resource has a unique **etag**.</span></span> <span data-ttu-id="54e0f-193">包含関係では、ある方を含め、さまざまなリソースの Etag 値を比較することはできません。</span><span class="sxs-lookup"><span data-stu-id="54e0f-193">Etag values for different resources, including those with containment relationships, cannot be compared.</span></span>
<span data-ttu-id="54e0f-194">クライアント アプリケーションは、バージョン管理を処理するために期待される関連[のエラー コード](/graph/errors) **409** 、 **412**項目の最新バージョンの読み取りと変更の競合を解決します。</span><span class="sxs-lookup"><span data-stu-id="54e0f-194">The client apps are expected to handle versioning related [error codes](/graph/errors) **409** and **412** by reading the latest version of the item and resolving the conflicting changes.</span></span>

## <a name="common-planner-error-conditions"></a><span data-ttu-id="54e0f-195">一般的な Planner のエラー条件</span><span class="sxs-lookup"><span data-stu-id="54e0f-195">Common Planner error conditions</span></span>

<span data-ttu-id="54e0f-196">Microsoft Graph に適用される[一般的なエラー](/graph/errors)のほかに、Planner API に固有のエラー条件もあります。</span><span class="sxs-lookup"><span data-stu-id="54e0f-196">In addition to [general errors](/graph/errors) that apply to Microsoft Graph, some error conditions are specific to the Planner API.</span></span>

### <a name="400-bad-request"></a><span data-ttu-id="54e0f-197">400 要求が正しくありません</span><span class="sxs-lookup"><span data-stu-id="54e0f-197">400 Bad request</span></span>

<span data-ttu-id="54e0f-198">いくつかの一般的なシナリオでは、`POST`と`PATCH`の要求は、400 のステータス コードを返すことができます。</span><span class="sxs-lookup"><span data-stu-id="54e0f-198">In some common scenarios, `POST` and `PATCH` requests can return a 400 status code.</span></span> <span data-ttu-id="54e0f-199">以下は、いくつかの一般的な原因です。</span><span class="sxs-lookup"><span data-stu-id="54e0f-199">The following are some of the common causes:</span></span>

* <span data-ttu-id="54e0f-p112">Open Type プロパティが正しい型でないか、型が指定されていないか、またはプロパティが含まれていません。たとえば、複雑な値が指定された [plannerAssignments](plannerassignments.md) プロパティは、値 `microsoft.graph.plannerAssignment` を指定した `@odata.type` プロパティで宣言する必要があります。</span><span class="sxs-lookup"><span data-stu-id="54e0f-p112">Open Type properties are not of correct types, or the type isn't specified, or they do not contain any properties. For example, [plannerAssignments](plannerassignments.md) properties with complex values need to declare `@odata.type` property with value `microsoft.graph.plannerAssignment`.</span></span>
* <span data-ttu-id="54e0f-p113">ORDER ヒントの値が[正しい書式](planner-order-hint-format.md)になっていません。たとえば、ORDER ヒントの値は、クライアントに返される値に直接設定されています。</span><span class="sxs-lookup"><span data-stu-id="54e0f-p113">Order hint values do not have the [correct format](planner-order-hint-format.md). For example, an order hint value is being set directly to the value returned to the client.</span></span>
* <span data-ttu-id="54e0f-p114">データが論理的に矛盾しています。たとえば、タスクの開始日がタスクの期日よりも後になる場合などです。</span><span class="sxs-lookup"><span data-stu-id="54e0f-p114">The data is logically inconsistent. For example, start date of task is later than due date of the task.</span></span>

### <a name="403-forbidden"></a><span data-ttu-id="54e0f-206">403 アクセスは許可されていません</span><span class="sxs-lookup"><span data-stu-id="54e0f-206">403 Forbidden</span></span>

<span data-ttu-id="54e0f-207">一般的なエラーだけでなくプランナー API も 403 ステータス コードを返しますサービスで定義された制限を超えているとき。</span><span class="sxs-lookup"><span data-stu-id="54e0f-207">In addition to the general errors, the Planner API also returns the 403 status code when a service-defined limit has been exceeded.</span></span> <span data-ttu-id="54e0f-208">この場合は、`code`エラーのリソースの種類のプロパティには、要求によって制限の種類が表示されます。</span><span class="sxs-lookup"><span data-stu-id="54e0f-208">If this is the case, the `code` property on the error resource type will indicate the type of the limit exceeded by the request.</span></span>
<span data-ttu-id="54e0f-209">制限の種類の有効な値を次に示します。</span><span class="sxs-lookup"><span data-stu-id="54e0f-209">The following are the possible values for the limit types.</span></span>

| <span data-ttu-id="54e0f-210">値</span><span class="sxs-lookup"><span data-stu-id="54e0f-210">Value</span></span>                         | <span data-ttu-id="54e0f-211">説明</span><span class="sxs-lookup"><span data-stu-id="54e0f-211">Description</span></span>                                                                                                                                                                                              |
| :---------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="54e0f-212">MaximumProjectsOwnedByUser</span><span class="sxs-lookup"><span data-stu-id="54e0f-212">MaximumProjectsOwnedByUser</span></span>    | <span data-ttu-id="54e0f-p116">グループが所有するプランの最大数の制限を超過しています。この制限は、[plannerPlan](plannerplan.md) リソースの `owner` プロパティに基づいています。</span><span class="sxs-lookup"><span data-stu-id="54e0f-p116">The maximum number of Plans owned by a group limit has been exceeded. This limit is based on the `owner` property on the [plannerPlan](plannerplan.md) resource.</span></span>                                         |
| <span data-ttu-id="54e0f-215">MaximumProjectsSharedWithUser</span><span class="sxs-lookup"><span data-stu-id="54e0f-215">MaximumProjectsSharedWithUser</span></span> | <span data-ttu-id="54e0f-p117">ユーザーが共有するプランの最大数の制限を超過しています。この制限は、[plannerPlanDetails](plannerplandetails.md) リソースの `sharedWith` プロパティに基づいています。</span><span class="sxs-lookup"><span data-stu-id="54e0f-p117">The maximum number of Plans shared with a user limit has been exceeded.  This limit is based on the `sharedWith` property on the [plannerPlanDetails](plannerplandetails.md) resource.</span></span>                   |
| <span data-ttu-id="54e0f-218">MaximumTasksCreatedByUser</span><span class="sxs-lookup"><span data-stu-id="54e0f-218">MaximumTasksCreatedByUser</span></span>     | <span data-ttu-id="54e0f-p118">ユーザーが作成するタスクの最大数の制限を超過しています。この制限は、[plannerTask](plannertask.md) リソースの `createdBy` プロパティに基づいています。</span><span class="sxs-lookup"><span data-stu-id="54e0f-p118">The maximum number of Tasks created by a user limit has been exceeded. This limit is based on the `createdBy` property on the [plannerTask](plannertask.md) resource.</span></span>                                    |
| <span data-ttu-id="54e0f-221">MaximumTasksAssignedToUser</span><span class="sxs-lookup"><span data-stu-id="54e0f-221">MaximumTasksAssignedToUser</span></span>    | <span data-ttu-id="54e0f-p119">ユーザーに割り当てられるタスクの最大数の制限を超過しています。この制限は、[plannerTask](plannertask.md) リソースの `assignments` プロパティに基づいています。</span><span class="sxs-lookup"><span data-stu-id="54e0f-p119">The maximum number of Tasks assigned to a user limit has been exceeded. This limit is based on the `assignments` property on the [plannerTask](plannertask.md) resource.</span></span>                                 |
| <span data-ttu-id="54e0f-224">MaximumTasksInProject</span><span class="sxs-lookup"><span data-stu-id="54e0f-224">MaximumTasksInProject</span></span>         | <span data-ttu-id="54e0f-p120">プランにおけるタスクの最大数の制限を超過しています。この制限は、[plannerTask](plannertask.md) リソースの `planId` プロパティに基づいています。</span><span class="sxs-lookup"><span data-stu-id="54e0f-p120">The maximum number of Tasks in a Plan limit has been exceeded. This limit is based on the `planId` property on the [plannerTask](plannertask.md) resource.</span></span>                                               |
| <span data-ttu-id="54e0f-227">MaximumActiveTasksInProject</span><span class="sxs-lookup"><span data-stu-id="54e0f-227">MaximumActiveTasksInProject</span></span>   | <span data-ttu-id="54e0f-p121">プランで完了されないタスクの最大数の制限を超過しています。この制限は、[plannerTask](plannertask.md) リソースの `planId` および `percentComplete` プロパティに基づいています。</span><span class="sxs-lookup"><span data-stu-id="54e0f-p121">The maximum number of Tasks that aren't completed in a Plan limit has been exceeded. This limit is based on the `planId` and `percentComplete` properties on the [plannerTask](plannertask.md) resource.</span></span> |
| <span data-ttu-id="54e0f-230">MaximumBucketsInProject</span><span class="sxs-lookup"><span data-stu-id="54e0f-230">MaximumBucketsInProject</span></span>       | <span data-ttu-id="54e0f-p122">プランにおけるバケットの最大数の制限を超過しています。この制限は、[plannerBucket](plannerbucket.md) リソースの `planId` プロパティに基づいています。</span><span class="sxs-lookup"><span data-stu-id="54e0f-p122">The maximum number of Buckets in a Plan limit has been exceeded. This limit is based on the `planId` property on the [plannerBucket](plannerbucket.md) resource.</span></span>                                         |
| <span data-ttu-id="54e0f-233">MaximumUsersSharedWithProject</span><span class="sxs-lookup"><span data-stu-id="54e0f-233">MaximumUsersSharedWithProject</span></span> | <span data-ttu-id="54e0f-234">[plannerPlanDetails](plannerplandetails.md) リソースの `sharedWith` プロパティに含まれる値が多すぎます。</span><span class="sxs-lookup"><span data-stu-id="54e0f-234">The `sharedWith` property on the [plannerPlanDetails](plannerplandetails.md) resource contains too many values.</span></span>                                                                                          |
| <span data-ttu-id="54e0f-235">MaximumReferencesOnTask</span><span class="sxs-lookup"><span data-stu-id="54e0f-235">MaximumReferencesOnTask</span></span>       | <span data-ttu-id="54e0f-236">[plannerTaskDetails](plannertaskdetails.md) リソースの `references` プロパティに含まれる値が多すぎます。</span><span class="sxs-lookup"><span data-stu-id="54e0f-236">The `references` property on the [plannerTaskDetails](plannertaskdetails.md) resource contains too many values.</span></span>                                                                                          |
| <span data-ttu-id="54e0f-237">MaximumChecklistItemsOnTask</span><span class="sxs-lookup"><span data-stu-id="54e0f-237">MaximumChecklistItemsOnTask</span></span>   | <span data-ttu-id="54e0f-238">[plannerTaskDetails](plannertaskdetails.md) リソースの `checklist` プロパティに含まれる値が多すぎます。</span><span class="sxs-lookup"><span data-stu-id="54e0f-238">The `checklist` property on the [plannerTaskDetails](plannertaskdetails.md) resource contains too many values.</span></span>                                                                                           |
| <span data-ttu-id="54e0f-239">MaximumAssigneesInTasks</span><span class="sxs-lookup"><span data-stu-id="54e0f-239">MaximumAssigneesInTasks</span></span>       | <span data-ttu-id="54e0f-240">[plannerTask](plannertask.md) リソースの `assignments` プロパティに含まれる値が多すぎます。</span><span class="sxs-lookup"><span data-stu-id="54e0f-240">The `assignments` property on the [plannerTask](plannertask.md) resource contains too many values.</span></span>                                                                                                       |
| <span data-ttu-id="54e0f-241">MaximumFavoritePlansForUser</span><span class="sxs-lookup"><span data-stu-id="54e0f-241">MaximumFavoritePlansForUser</span></span>   | <span data-ttu-id="54e0f-242">`favoritePlanReferences` [PlannerUser](planneruser.md)リソースのプロパティに値が多すぎますが含まれています。</span><span class="sxs-lookup"><span data-stu-id="54e0f-242">The `favoritePlanReferences` property on the [plannerUser](planneruser.md) resource contains too many values.</span></span>                                                                                            |
| <span data-ttu-id="54e0f-243">MaximumRecentPlansForUser</span><span class="sxs-lookup"><span data-stu-id="54e0f-243">MaximumRecentPlansForUser</span></span>     | <span data-ttu-id="54e0f-244">`recentPlanReferences` [PlannerUser](planneruser.md)リソースのプロパティに値が多すぎますが含まれています。</span><span class="sxs-lookup"><span data-stu-id="54e0f-244">The `recentPlanReferences` property on the [plannerUser](planneruser.md) resource contains too many values.</span></span>                                                                                              |
| <span data-ttu-id="54e0f-245">MaximumContextsOnPlan</span><span class="sxs-lookup"><span data-stu-id="54e0f-245">MaximumContextsOnPlan</span></span>         | <span data-ttu-id="54e0f-246">`contexts` [PlannerPlan](plannerplan.md)リソースのプロパティに値が多すぎますが含まれています。</span><span class="sxs-lookup"><span data-stu-id="54e0f-246">The `contexts` property on the [plannerPlan](plannerplan.md) resource contains too many values.</span></span>                                                                                                          |
| <span data-ttu-id="54e0f-247">MaximumPlannerPlans</span><span class="sxs-lookup"><span data-stu-id="54e0f-247">MaximumPlannerPlans</span></span>       | <span data-ttu-id="54e0f-248">グループには、計画が既に含まれています。</span><span class="sxs-lookup"><span data-stu-id="54e0f-248">The group already contains a Plan.</span></span> <span data-ttu-id="54e0f-249">現在、グループは 1 つの計画のみ含めることができます。</span><span class="sxs-lookup"><span data-stu-id="54e0f-249">Currently, groups can only contain one Plan.</span></span> <span data-ttu-id="54e0f-250">**注:** いくつかの Microsoft アプリケーションでは、この制限を超えることができます。</span><span class="sxs-lookup"><span data-stu-id="54e0f-250">**Note:** Some Microsoft apps can exceed this limit.</span></span> <span data-ttu-id="54e0f-251">今後、すべてのアプリケーションにこの機能は拡張します。</span><span class="sxs-lookup"><span data-stu-id="54e0f-251">In the future, we will extend this capability to all apps.</span></span>                                                                                                      |

### <a name="412-precondition-failed"></a><span data-ttu-id="54e0f-252">412 必須条件に失敗しました</span><span class="sxs-lookup"><span data-stu-id="54e0f-252">412 Precondition Failed</span></span> 

<span data-ttu-id="54e0f-253">平面のすべての API `POST`、 `PATCH`、および`DELETE`要求を`If-Match`ヘッダーは、要求の対象となるリソースの最後の既知の etag 値を指定します。</span><span class="sxs-lookup"><span data-stu-id="54e0f-253">All Planer API `POST`, `PATCH`, and `DELETE` requests require the `If-Match` header to be specified with the last known etag value of the resource that is subject to the request.</span></span>
<span data-ttu-id="54e0f-254">412 のステータス コードは、要求で指定された etag 値には不要になったサービス内のリソースのバージョンが一致する場合にも返されます。</span><span class="sxs-lookup"><span data-stu-id="54e0f-254">The 412 status code can also be returned if the etag value specified in the request no longer matches a version of the resource in the service.</span></span> <span data-ttu-id="54e0f-255">この例では、クライアントは、リソースの読み取りを再試行する必要があり、新しい etag を取得します。</span><span class="sxs-lookup"><span data-stu-id="54e0f-255">In this case, the clients should read the resource again and get a new etag.</span></span>
