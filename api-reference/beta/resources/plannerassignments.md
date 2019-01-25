---
title: plannerAssignments リソースの種類
description: '**PlannerAssignments**リソースでは、plannerTask のリソースの割り当てを表します。 この型は、オープン型です。 このタイプの場合は、各プロパティ名 '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 2c379c786e3b94395aa3de7bc382e184db0fcc24
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29507769"
---
# <a name="plannerassignments-resource-type"></a><span data-ttu-id="724c7-105">plannerAssignments リソースの種類</span><span class="sxs-lookup"><span data-stu-id="724c7-105">plannerAssignments resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="724c7-p102">**plannerAssignments** リソースは [plannerTask](plannertask.md) リソースの割り当てを表します。この型はオープン型です。この型の各プロパティ名は、タスクが割り当てられているユーザー オブジェクトの ID です。ユーザーは、orderHint プロパティが値として設定されている [plannerassignment](plannerassignment.md) オブジェクトとそれぞれの ID を使った名前の付いた新しいプロパティを作成して、タスクに割り当てることができます。担当者は、それぞれの ID を使った名前の付いたプロパティを null に設定することによって、タスクからの割り当てを解除できます。</span><span class="sxs-lookup"><span data-stu-id="724c7-p102">The **plannerAssignments** resource represents assignments of a [plannerTask](plannertask.md) resource. This type is an open type. Each property name in this type is the ID of a user object a task is assigned to. The users can be assigned to tasks with creating new properties named with their ID, with a [plannerassignment](plannerassignment.md) object with orderHint property populated as the value. The assignees can be unassigned from the task by setting the propety named with their ID to null.</span></span>


## <a name="properties"></a><span data-ttu-id="724c7-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="724c7-111">Properties</span></span>
<span data-ttu-id="724c7-p103">クライアントは、オープン型のプロパティを定義できます。ただしこの場合、クライアントは割り当て済みユーザーの ID をプロパティ名として指定する必要があります。担当者を作成または変更する場合はプロパティを **plannerAssignment** オブジェクトに設定し、削除する場合は null に設定します。</span><span class="sxs-lookup"><span data-stu-id="724c7-p103">Properties of an Open Type can be defined by the client. In this case though, the client must provide assigned user's IDs as property names. The property must be set to a **plannerAssignment** object to create or modify assignees, and to null to remove them.</span></span>

<span data-ttu-id="724c7-115">例:</span><span class="sxs-lookup"><span data-stu-id="724c7-115">Example:</span></span>

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
<span data-ttu-id="724c7-p104">この例では、ID が ca2a1df2-e36b-4987-9f6b-0ea462f4eb47 のユーザーをタスクの担当者リストから削除し、ユーザー ID が 4e98f8f1-bb03-4015-b8e0-19bb370949d8 の担当者の順序を変更します。ID が 4e98f8f1-bb03-4015-b8e0-19bb370949d8 のユーザーにタスクがまだ割り当てられていない場合は、この値を使って割り当てを更新すると、タスクがこのユーザーに割り当てられます。</span><span class="sxs-lookup"><span data-stu-id="724c7-p104">This example removes user with ID ca2a1df2-e36b-4987-9f6b-0ea462f4eb47 from the assignees list of the task, while changing the order of the assignee with user ID 4e98f8f1-bb03-4015-b8e0-19bb370949d8. If the task isn't already assigned to user with ID 4e98f8f1-bb03-4015-b8e0-19bb370949d8, updating the assignments with this value will assign the task to this user.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerAssignments resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerassignments.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
