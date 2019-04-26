---
title: プランの割り当てリソースの種類
description: '[ **plan** ] [割り当て] リソースは、"プラン" タスクリソースの割り当てを表します。 この型はオープン型です。 この型の各プロパティの名前 '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 2f26bab4eb69a79f4bd18f80128e4445217a1ae7
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344572"
---
# <a name="plannerassignments-resource-type"></a><span data-ttu-id="4798a-105">プランの割り当てリソースの種類</span><span class="sxs-lookup"><span data-stu-id="4798a-105">plannerAssignments resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4798a-106">[ **plan** ] [割り当て] リソースは、"[プラン" タスク](plannertask.md)リソースの割り当てを表します。</span><span class="sxs-lookup"><span data-stu-id="4798a-106">The **plannerAssignments** resource represents assignments of a [plannerTask](plannertask.md) resource.</span></span> <span data-ttu-id="4798a-107">この型はオープン型です。</span><span class="sxs-lookup"><span data-stu-id="4798a-107">This type is an open type.</span></span> <span data-ttu-id="4798a-108">この型の各プロパティ名は、タスクが割り当てられているユーザーオブジェクトの ID です。</span><span class="sxs-lookup"><span data-stu-id="4798a-108">Each property name in this type is the ID of a user object a task is assigned to.</span></span> <span data-ttu-id="4798a-109">ユーザーは、ID でという名前の新しいプロパティを作成してタスクに割り当てることができます。このオブジェクトには、値として orderhint プロパティが設定された[プランの assignment](plannerassignment.md)オブジェクトがあります。</span><span class="sxs-lookup"><span data-stu-id="4798a-109">The users can be assigned to tasks with creating new properties named with their ID, with a [plannerassignment](plannerassignment.md) object with orderHint property populated as the value.</span></span> <span data-ttu-id="4798a-110">parenttab の ID を null に設定することによって、タスクの割り当てを解除することができます。</span><span class="sxs-lookup"><span data-stu-id="4798a-110">The assignees can be unassigned from the task by setting the propety named with their ID to null.</span></span>


## <a name="properties"></a><span data-ttu-id="4798a-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4798a-111">Properties</span></span>
<span data-ttu-id="4798a-112">オープン型のプロパティは、クライアントで定義できます。</span><span class="sxs-lookup"><span data-stu-id="4798a-112">Properties of an Open Type can be defined by the client.</span></span> <span data-ttu-id="4798a-113">ただし、この場合、クライアントは、割り当てられたユーザーの id をプロパティ名として提供する必要があります。</span><span class="sxs-lookup"><span data-stu-id="4798a-113">In this case though, the client must provide assigned user's IDs as property names.</span></span> <span data-ttu-id="4798a-114">タスク実施者を作成または変更するには、このプロパティを**plan**オブジェクトに設定する必要があります。削除するには null に設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="4798a-114">The property must be set to a **plannerAssignment** object to create or modify assignees, and to null to remove them.</span></span>

<span data-ttu-id="4798a-115">例:</span><span class="sxs-lookup"><span data-stu-id="4798a-115">Example:</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerAssignments"
}-->

```json
{
  "ca2a1df2-e36b-4987-9f6b-0ea462f4eb47": null,
  "4e98f8f1-bb03-4015-b8e0-19bb370949d8": { 
      "@odata.type": "microsoft.graph.plannerAssignment",
      "orderHint": "String"
    }
}
```
<span data-ttu-id="4798a-116">この例では、id ca2a1df2-e36b-4987-9f6b-0ea462f4eb47 を持つユーザーをタスクのタスク実施者リストから削除し、ユーザー id 4e98f8f1-bb03-4015-b8e0-19bb370949d8 を使用して担当者の順序を変更します。</span><span class="sxs-lookup"><span data-stu-id="4798a-116">This example removes user with ID ca2a1df2-e36b-4987-9f6b-0ea462f4eb47 from the assignees list of the task, while changing the order of the assignee with user ID 4e98f8f1-bb03-4015-b8e0-19bb370949d8.</span></span> <span data-ttu-id="4798a-117">タスクが ID 4e98f8f1-bb03-4015-b8e0-19bb370949d8 のユーザーにまだ割り当てられていない場合は、この値を使用して割り当てを更新すると、このユーザーにタスクが割り当てられます。</span><span class="sxs-lookup"><span data-stu-id="4798a-117">If the task isn't already assigned to user with ID 4e98f8f1-bb03-4015-b8e0-19bb370949d8, updating the assignments with this value will assign the task to this user.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerAssignments resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
