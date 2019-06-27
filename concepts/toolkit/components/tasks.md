---
title: Microsoft Graph ツールキットの Tasks コンポーネント
description: タスクコンポーネントを使用すると、ユーザーはタスクの表示、追加、削除、完了、または編集を行うことができます。 Microsoft Planner または Microsoft To Do のすべてのタスクで動作します。
localization_priority: Normal
author: benotter
ms.openlocfilehash: 3c2017acd7fe054c71a609c8d908e119e12a590b
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/26/2019
ms.locfileid: "35243052"
---
# <a name="tasks-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="5b8ad-104">Microsoft Graph ツールキットの Tasks コンポーネント</span><span class="sxs-lookup"><span data-stu-id="5b8ad-104">Tasks component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="5b8ad-105">タスクコンポーネントを使用すると、ユーザーはタスクの表示、追加、削除、完了、または編集を行うことができます。</span><span class="sxs-lookup"><span data-stu-id="5b8ad-105">The Tasks component enables the user to view, add, remove, complete, or edit tasks.</span></span> <span data-ttu-id="5b8ad-106">Microsoft Planner または Microsoft のタスクで機能します。</span><span class="sxs-lookup"><span data-stu-id="5b8ad-106">It works with tasks in Microsoft Planner or Microsoft To-Do.</span></span>

## <a name="example"></a><span data-ttu-id="5b8ad-107">例</span><span class="sxs-lookup"><span data-stu-id="5b8ad-107">Example</span></span>

[<span data-ttu-id="5b8ad-108">jsfiddle の例</span><span class="sxs-lookup"><span data-stu-id="5b8ad-108">jsfiddle example</span></span>](https://jsfiddle.net/metulev/qhg68m31/)

````html
    <mgt-tasks></mgt-tasks>
````

## <a name="properties"></a><span data-ttu-id="5b8ad-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5b8ad-109">Properties</span></span>

| <span data-ttu-id="5b8ad-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5b8ad-110">Property</span></span> | <span data-ttu-id="5b8ad-111">属性</span><span class="sxs-lookup"><span data-stu-id="5b8ad-111">Attribute</span></span> | <span data-ttu-id="5b8ad-112">説明</span><span class="sxs-lookup"><span data-stu-id="5b8ad-112">Description</span></span> |
| -- | -- | -- |
| `dataSource` | `data-source="todo/planner"` | <span data-ttu-id="5b8ad-113">タスクのデータソースを設定します。 Microsoft To Do または Microsoft Planner のいずれかです。</span><span class="sxs-lookup"><span data-stu-id="5b8ad-113">Sets the data source for tasks - either Microsoft To-Do, or Microsoft Planner.</span></span> <span data-ttu-id="5b8ad-114">既定値は `planner` です。</span><span class="sxs-lookup"><span data-stu-id="5b8ad-114">Default is `planner`.</span></span> |
| `readOnly` | `read-only` | <span data-ttu-id="5b8ad-115">タスクのインターフェイスを読み取り専用に設定します (タスクの追加や削除は行われません)。</span><span class="sxs-lookup"><span data-stu-id="5b8ad-115">Sets the task interface to be read only (no adding or removing tasks).</span></span> <span data-ttu-id="5b8ad-116">既定値は `false` です。</span><span class="sxs-lookup"><span data-stu-id="5b8ad-116">Default is `false`.</span></span> |
| `initialId` | `initial-id="planner_id/folder_id"` | <span data-ttu-id="5b8ad-117">最初に表示されたプランナーまたは folder を指定された ID に設定します。</span><span class="sxs-lookup"><span data-stu-id="5b8ad-117">Sets the initially displayed planner or folder to the provided ID.</span></span> |
| `initialBucketId` | `initial-bucket-id="bucket_id"` | <span data-ttu-id="5b8ad-118">最初に表示されるバケット (Planner データソースのみ) を指定された ID に設定します。</span><span class="sxs-lookup"><span data-stu-id="5b8ad-118">Sets the initially displayed bucket (Planner Data-Source Only) to the provided ID.</span></span> |
| `targetId` | `target-id="planner_id/folder_id"` | <span data-ttu-id="5b8ad-119">タスクインターフェイスを、指定したプランナーまたはフォルダー ID にロックします。</span><span class="sxs-lookup"><span data-stu-id="5b8ad-119">Locks the tasks interface to the provided planner or folder ID.</span></span> |
| `targetBucketId` | `target-bucket-id="bucket_id"` | <span data-ttu-id="5b8ad-120">タスクインターフェイスを、指定されたバケット ID にロックします (Planner データソースのみ)。</span><span class="sxs-lookup"><span data-stu-id="5b8ad-120">Locks the tasks interface to the provided bucket ID (Planner Data-Source Only).</span></span> |

<span data-ttu-id="5b8ad-121">次に例を示します。</span><span class="sxs-lookup"><span data-stu-id="5b8ad-121">The following is an example.</span></span>

````html
<mgt-tasks read-only initial-id="12345"></mgt-tasks>
````

## <a name="custom-css-variables"></a><span data-ttu-id="5b8ad-122">カスタム CSS 変数</span><span class="sxs-lookup"><span data-stu-id="5b8ad-122">Custom CSS variables</span></span>

````css
mgt-tasks {
--tasks-header-padding
--tasks-header-margin 

--tasks-title-padding
--tasks-plan-title-font-size
--tasks-plan-title-padding

--tasks-new-button-width
--tasks-new-button-height
--tasks-new-button-color
--tasks-new-button-background
--tasks-new-button-border
--tasks-new-button-hover-background
--tasks-new-button-active-background

--tasks-new-task-name-margin

--task-margin
--task-box-shadow
--task-background
--task-border

--task-header-color
--task-header-margin

--task-detail-icon-margin

--task-new-margin
--task-new-border
--task-new-line-margin
--tasks-new-line-border
--task-new-input-margin
--task-new-input-padding
--task-new-input-font-size
--task-new-input-active-border
--task-new-select-border

--task-new-add-button-background
--task-new-add-button-disabled-background
--task-new-cancel-button-color

--task-complete-background
--task-complete-border
--task-complete-header-color
--task-complete-detail-color
--task-complete-detail-icon-color
}
````

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="5b8ad-123">Microsoft Graph のアクセス許可</span><span class="sxs-lookup"><span data-stu-id="5b8ad-123">Microsoft Graph permissions</span></span>

<span data-ttu-id="5b8ad-124">このコントロールでは、次の Microsoft Graph Api とアクセス許可を使用します。</span><span class="sxs-lookup"><span data-stu-id="5b8ad-124">This control uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="5b8ad-125">リソース</span><span class="sxs-lookup"><span data-stu-id="5b8ad-125">Resource</span></span> | <span data-ttu-id="5b8ad-126">アクセス許可/スコープ</span><span class="sxs-lookup"><span data-stu-id="5b8ad-126">Permission/scope</span></span> |
| - | - |
| <span data-ttu-id="5b8ad-127">プラン/プラン</span><span class="sxs-lookup"><span data-stu-id="5b8ad-127">/me/planner/plans</span></span> | `Group.Read.All` |
| <span data-ttu-id="5b8ad-128">/planner/plans/$ {id}</span><span class="sxs-lookup"><span data-stu-id="5b8ad-128">/planner/plans/${id}</span></span> | <span data-ttu-id="5b8ad-129">`Group.Read.All`, `Group.ReadWrite.All`</span><span class="sxs-lookup"><span data-stu-id="5b8ad-129"></span></span> |
| <span data-ttu-id="5b8ad-130">/プラン</span><span class="sxs-lookup"><span data-stu-id="5b8ad-130">/planner/tasks</span></span> | `Group.ReadWrite.All` |
| <span data-ttu-id="5b8ad-131">/Me/Outlook/taskgroups</span><span class="sxs-lookup"><span data-stu-id="5b8ad-131">/me/outlook/taskGroups</span></span> | `Tasks.Read` |
| <span data-ttu-id="5b8ad-132">/Me/Outlook/taskfolders</span><span class="sxs-lookup"><span data-stu-id="5b8ad-132">/me/outlook/taskFolders</span></span> | <span data-ttu-id="5b8ad-133">`Tasks.Read`, `Tasks.ReadWrite`</span><span class="sxs-lookup"><span data-stu-id="5b8ad-133"></span></span> |
| <span data-ttu-id="5b8ad-134">/me/outlook/tasks</span><span class="sxs-lookup"><span data-stu-id="5b8ad-134">/me/outlook/tasks</span></span> | `Tasks.ReadWrite` |

<span data-ttu-id="5b8ad-135">Microsoft Planner データソースの場合、フェッチおよび読み取りタスクには、グループの読み取り権限が必要です。</span><span class="sxs-lookup"><span data-stu-id="5b8ad-135">For the Microsoft Planner data source, fetching and reading tasks requires the Groups.Read.All permission.</span></span> <span data-ttu-id="5b8ad-136">タスクを追加、更新、または削除するには、すべてのアクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="5b8ad-136">Adding, updating, or removing tasks requires the Groups.ReadWrite.All permission.</span></span>

<span data-ttu-id="5b8ad-137">Microsoft Todo データソースの場合は、タスクを取得および読み取りするための読み取りアクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="5b8ad-137">For the Microsoft Todo data source, the Tasks.Read permission is required for fetching and reading tasks.</span></span> <span data-ttu-id="5b8ad-138">タスクを追加、更新、または削除するには、タスクの読み取りアクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="5b8ad-138">Adding, updating, or removing tasks requires the Tasks.ReadWrite permission.</span></span>

## <a name="authentication"></a><span data-ttu-id="5b8ad-139">認証</span><span class="sxs-lookup"><span data-stu-id="5b8ad-139">Authentication</span></span>

<span data-ttu-id="5b8ad-140">タスクコンポーネントは、[認証のドキュメント](./../providers.md)で説明されているグローバル認証プロバイダを使用します。</span><span class="sxs-lookup"><span data-stu-id="5b8ad-140">The tasks component uses the global authentication provider described in the [authentication documentation](./../providers.md).</span></span>
