---
title: Planner のタスクおよびプラン API の概要
description: Planner は、チームが作業を組織するためのシンプルかつビジュアルな手段を提供します。 顧客は Planner を使用することにより、プランを作成したり、タスクを組織して割り当てたり、進捗状況を共有したり、コンテンツに対して共同作業をしたりできます。  Planner は、タスク ボード、グラフ ページ、スケジュール ビューなどのインタラクティブなエクスペリエンスを提供し、Office 365 を通じた機能統合を実現します。
author: TarkanSevilmis
localization_priority: Priority
ms.prod: planner
ms.openlocfilehash: c2e8be27eeb4f91b3030701e2f8416fecf29c2d7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32564231"
---
# <a name="planner-tasks-and-plans-api-overview"></a><span data-ttu-id="4c4af-105">Planner のタスクおよびプラン API の概要</span><span class="sxs-lookup"><span data-stu-id="4c4af-105">Planner tasks and plans API overview</span></span>
<span data-ttu-id="4c4af-106">Planner は、チームが作業を組織するためのシンプルかつビジュアルな手段を提供します。</span><span class="sxs-lookup"><span data-stu-id="4c4af-106">Planner provides a simple and visual way for teams to organize their work.</span></span> <span data-ttu-id="4c4af-107">顧客は Planner を使用することにより、プランを作成したり、タスクを組織して割り当てたり、進捗状況を共有したり、コンテンツに対して共同作業をしたりできます。</span><span class="sxs-lookup"><span data-stu-id="4c4af-107">Customers can use Planner to create plans, organize and assign tasks, share progress, and collaborate on content.</span></span>  <span data-ttu-id="4c4af-108">Planner は、タスク ボード、グラフ ページ、スケジュール ビューなどのインタラクティブなエクスペリエンスを提供し、Office 365 を通じた機能統合を実現します。</span><span class="sxs-lookup"><span data-stu-id="4c4af-108">Planner provides several interactive experiences including a task board, a charts page, and a schedule view, as well as integrations throughout Office 365.</span></span>

<span data-ttu-id="4c4af-109">**Office 365 Planner タスク ボード**</span><span class="sxs-lookup"><span data-stu-id="4c4af-109">**Office 365 Planner task board**</span></span>

<span data-ttu-id="4c4af-110">![Office 365 Planner タスク ボードのスクリーン ショット](images/plannerboard.png "Planner ボードの画像")</span><span class="sxs-lookup"><span data-stu-id="4c4af-110">![Screenshot of an Office 365 Planner task board](images/plannerboard.png "Image of Planner board")</span></span>


## <a name="why-integrate-with-planner-tasks"></a><span data-ttu-id="4c4af-111">Planner タスクを統合する理由</span><span class="sxs-lookup"><span data-stu-id="4c4af-111">Why integrate with Planner tasks?</span></span>
<span data-ttu-id="4c4af-112">Planner は、Office 365 でのコラボレーション エクスペリエンスのためのタスク追跡機能を提供します。</span><span class="sxs-lookup"><span data-stu-id="4c4af-112">Planner provides task tracking capabilities for collaboration experiences in Office 365.</span></span> <span data-ttu-id="4c4af-113">エンド ユーザーのチームやグループのためのタスク追跡機能や作業を組織する機能が必要な場合、Planner が最適です。</span><span class="sxs-lookup"><span data-stu-id="4c4af-113">If your scenarios require tracking tasks and organizing work for a team or group of end users, Planner is the right service for you.</span></span> <span data-ttu-id="4c4af-114">Planner 統合は、Office 365 でコラボレーションする何百万というユーザーに達するのに役立ちます。</span><span class="sxs-lookup"><span data-stu-id="4c4af-114">Planner integration can help you reach the millions of users collaborating on Office 365.</span></span> 

### <a name="organize-your-teams-work"></a><span data-ttu-id="4c4af-115">チームの作業を組織する</span><span class="sxs-lookup"><span data-stu-id="4c4af-115">Organize your team’s work</span></span>
<span data-ttu-id="4c4af-116">Planner は、チームを立ち上げ、[タスクを作成し](/graph/api/planner-post-tasks?view=graph-rest-1.0)、それをチームの他のメンバーに割り当てるための共有スペースを提供します。</span><span class="sxs-lookup"><span data-stu-id="4c4af-116">Planner provides a shared space where you can build a team, [create tasks](/graph/api/planner-post-tasks?view=graph-rest-1.0), and assign them to others on the team.</span></span> <span data-ttu-id="4c4af-117">Planner を利用すれば、誰が何をしているのかを容易に把握でき、順調に事が進んでいるかどうかを確認できます。期限、進捗状況、説明などの追加情報によりタスクを更新し、カスタマイズ可能なバケットとカテゴリ ラベルによりタスクを詳細に組織することができます。</span><span class="sxs-lookup"><span data-stu-id="4c4af-117">Planner makes it easy for everyone to know who’s doing what and if things are on track. You can update tasks with additional information like due dates, progress, and descriptions, and then further organize tasks with customizable buckets and category labels.</span></span>   

### <a name="collaborate-across-office-365"></a><span data-ttu-id="4c4af-118">Office 365 を通じた共同作業</span><span class="sxs-lookup"><span data-stu-id="4c4af-118">Collaborate across Office 365</span></span>
<span data-ttu-id="4c4af-119">Planner は、Office 365 を通じてコラボレーション エクスペリエンスに統合されています。</span><span class="sxs-lookup"><span data-stu-id="4c4af-119">Planner integrates into collaboration experiences across Office 365.</span></span> <span data-ttu-id="4c4af-120">Planner の Web およびモバイル クライアントに加えて、ユーザーは Planner のプランやタスクを SharePoint および Microsoft Teams から表示したり更新したりできます。</span><span class="sxs-lookup"><span data-stu-id="4c4af-120">In addition to Planner web and mobile clients, users can view and update Planner plans and tasks from within SharePoint and Microsoft Teams.</span></span>  

<span data-ttu-id="4c4af-121">Planner 自体でも Microsoft Graph および Office 365 のグループ サービスが利用されています。</span><span class="sxs-lookup"><span data-stu-id="4c4af-121">Planner itself is also powered by the Microsoft Graph and the Office 365 group service.</span></span> <span data-ttu-id="4c4af-122">アップロードして Planner タスクに添付するファイルは、SharePoint に保存されます。</span><span class="sxs-lookup"><span data-stu-id="4c4af-122">Files that you upload and attach to Planner tasks are stored in SharePoint.</span></span> <span data-ttu-id="4c4af-123">Planner のコメントは、Outlook のグループ会話に基づいています。</span><span class="sxs-lookup"><span data-stu-id="4c4af-123">Planner comments are based on Outlook group conversations.</span></span>

<!-- Add image
Note: Put an image here showing the relationship between Planner and other things
-->

### <a name="automate-the-creation-of-plans-and-tasks"></a><span data-ttu-id="4c4af-124">プランおよびタスクの作成の自動化</span><span class="sxs-lookup"><span data-stu-id="4c4af-124">Automate the creation of plans and tasks</span></span>
<span data-ttu-id="4c4af-125">繰り返されるプロセスやプロジェクト タイプの作業をしていますか。</span><span class="sxs-lookup"><span data-stu-id="4c4af-125">Are you working on repeated process or project type?</span></span> <span data-ttu-id="4c4af-126">Planner API を使用することにより、プランやタスク リストの作成を自動化できます。</span><span class="sxs-lookup"><span data-stu-id="4c4af-126">You can use the Planner API to automate the creation of a plan and a list of tasks.</span></span>  
 
## <a name="top-planner-api-tasks"></a><span data-ttu-id="4c4af-127">Planner API のトップ タスク</span><span class="sxs-lookup"><span data-stu-id="4c4af-127">Top Planner API tasks</span></span>

|<span data-ttu-id="4c4af-128">操作</span><span class="sxs-lookup"><span data-stu-id="4c4af-128">Operation</span></span>|<span data-ttu-id="4c4af-129">URL</span><span class="sxs-lookup"><span data-stu-id="4c4af-129">URL</span></span>|
|:--------|:--|
|<span data-ttu-id="4c4af-130">グループの[プラン](/graph/api/resources/plannerplan?view=graph-rest-beta)をすべて表示</span><span class="sxs-lookup"><span data-stu-id="4c4af-130">See all the [plans](/graph/api/resources/plannerplan?view=graph-rest-beta) for a group</span></span>|<span data-ttu-id="4c4af-131">GET [https://graph.microsoft.com/v1.0/groups/{id}/planner/plans](https://developer.microsoft.com/graph/graph-explorer?request=groups/{id}/planner/plans&version=v1.0)</span><span class="sxs-lookup"><span data-stu-id="4c4af-131">GET [https://graph.microsoft.com/v1.0/groups/{id}/planner/plans](https://developer.microsoft.com/graph/graph-explorer?request=groups/{id}/planner/plans&version=v1.0)</span></span>|
|<span data-ttu-id="4c4af-132">プラン内の[タスク](/graph/api/resources/plannertask?view=graph-rest-beta)を表示</span><span class="sxs-lookup"><span data-stu-id="4c4af-132">See [tasks](/graph/api/resources/plannertask?view=graph-rest-beta) in a plan</span></span>|<span data-ttu-id="4c4af-133">GET [https://graph.microsoft.com/v1.0/planner/plans/{id}/tasks](https://developer.microsoft.com/graph/graph-explorer?request=planner/plans/{id}/tasks&version=v1.0)</span><span class="sxs-lookup"><span data-stu-id="4c4af-133">GET [https://graph.microsoft.com/v1.0/planner/plans/{id}/tasks](https://developer.microsoft.com/graph/graph-explorer?request=planner/plans/{id}/tasks&version=v1.0)</span></span>|
|<span data-ttu-id="4c4af-134">複数のプランを通じて自分に割り当てられている[マイ タスク](/graph/api/planneruser-list-tasks?view=graph-rest-beta)をすべて表示</span><span class="sxs-lookup"><span data-stu-id="4c4af-134">See all [my tasks](/graph/api/planneruser-list-tasks?view=graph-rest-beta) assigned to me across plans</span></span>|<span data-ttu-id="4c4af-135">GET [https://graph.microsoft.com/v1.0/me/planner/tasks/](https://developer.microsoft.com/graph/graph-explorer?request=me/planner/tasks/&version=v1.0)</span><span class="sxs-lookup"><span data-stu-id="4c4af-135">GET [https://graph.microsoft.com/v1.0/me/planner/tasks/](https://developer.microsoft.com/graph/graph-explorer?request=me/planner/tasks/&version=v1.0)</span></span>|
|[<span data-ttu-id="4c4af-136">新しいタスクを作成</span><span class="sxs-lookup"><span data-stu-id="4c4af-136">Create a new task</span></span>](/graph/api/planner-post-tasks?view=graph-rest-1.0)|<span data-ttu-id="4c4af-137">POST [https://graph.microsoft.com/v1.0/planner/tasks](https://developer.microsoft.com/graph/graph-explorer?request=groups/{id}/planner/plans&version=v1.0)</span><span class="sxs-lookup"><span data-stu-id="4c4af-137">POST [https://graph.microsoft.com/v1.0/planner/tasks](https://developer.microsoft.com/graph/graph-explorer?request=groups/{id}/planner/plans&version=v1.0)</span></span>|
|[<span data-ttu-id="4c4af-138">タスクを更新</span><span class="sxs-lookup"><span data-stu-id="4c4af-138">Update a task</span></span>](/graph/api/plannertask-update?view=graph-rest-1.0)|<span data-ttu-id="4c4af-139">PATCH [https://graph.microsoft.com/v1.0/planner/tasks/{task-id}](https://developer.microsoft.com/graph/graph-explorer?request=groups/{id}/planner/plans&version=v1.0)</span><span class="sxs-lookup"><span data-stu-id="4c4af-139">PATCH [https://graph.microsoft.com/v1.0/planner/tasks/{task-id}](https://developer.microsoft.com/graph/graph-explorer?request=groups/{id}/planner/plans&version=v1.0)</span></span>|
|[<span data-ttu-id="4c4af-140">タスクを削除</span><span class="sxs-lookup"><span data-stu-id="4c4af-140">Delete a task</span></span>](/graph/api/plannertask-delete?view=graph-rest-1.0)|<span data-ttu-id="4c4af-141">DELETE [https://graph.microsoft.com/v1.0/planner/tasks/{id}](https://developer.microsoft.com/graph/graph-explorer?request=groups/{id}/planner/plans&version=v1.0)</span><span class="sxs-lookup"><span data-stu-id="4c4af-141">DELETE [https://graph.microsoft.com/v1.0/planner/tasks/{id}](https://developer.microsoft.com/graph/graph-explorer?request=groups/{id}/planner/plans&version=v1.0)</span></span>|

## <a name="api-reference"></a><span data-ttu-id="4c4af-142">API リファレンス</span><span class="sxs-lookup"><span data-stu-id="4c4af-142">API reference</span></span>
<span data-ttu-id="4c4af-143">このサービスの API リファレンスをお探しですか?</span><span class="sxs-lookup"><span data-stu-id="4c4af-143">Looking for the API reference for this service?</span></span>

- [<span data-ttu-id="4c4af-144">Microsoft Graph v1.0 の Planner API</span><span class="sxs-lookup"><span data-stu-id="4c4af-144">Planner API in Microsoft Graph v1.0</span></span>](/graph/api/resources/planner-overview?view=graph-rest-1.0)
- [<span data-ttu-id="4c4af-145">Microsoft Graph ベータ版の Planner API</span><span class="sxs-lookup"><span data-stu-id="4c4af-145">Planner API in Microsoft Graph beta</span></span>](/graph/api/resources/planner-overview?view=graph-rest-beta)


## <a name="next-steps"></a><span data-ttu-id="4c4af-146">次のステップ</span><span class="sxs-lookup"><span data-stu-id="4c4af-146">Next steps</span></span>

- [<span data-ttu-id="4c4af-147">Planner API を使用する</span><span class="sxs-lookup"><span data-stu-id="4c4af-147">Use the Planner API</span></span>](/graph/api/resources/planner-overview?view=graph-rest-1.0)
- [<span data-ttu-id="4c4af-148">プランを操作する</span><span class="sxs-lookup"><span data-stu-id="4c4af-148">Work with plans</span></span>](/graph/api/resources/planner-overview?view=graph-rest-1.0#plans)
- [<span data-ttu-id="4c4af-149">タスクを操作する</span><span class="sxs-lookup"><span data-stu-id="4c4af-149">Work with tasks</span></span>](/graph/api/resources/planner-overview?view=graph-rest-1.0#tasks)
