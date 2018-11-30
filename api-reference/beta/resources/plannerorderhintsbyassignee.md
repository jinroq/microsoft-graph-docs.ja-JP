---
title: plannerOrderHintsByAssignee リソースの種類
description: '**PlannerOrderHintsByAssignee**は、タスクの掲示板のビューに割り当てられているタスクの順序を示すために、plannerTask のリソースの割り当て先の命令のヒントを含むリソースです。'
ms.openlocfilehash: a15a1f81b348958e5c38189db10743b83d72050f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068202"
---
# <a name="plannerorderhintsbyassignee-resource-type"></a><span data-ttu-id="0ac30-103">plannerOrderHintsByAssignee リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0ac30-103">plannerOrderHintsByAssignee resource type</span></span>

> <span data-ttu-id="0ac30-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0ac30-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0ac30-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0ac30-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0ac30-p102">**plannerOrderHintsByAssignee** には、タスク ボードの [割り当て先ユーザー/グループ] ビューのタスクの順序を示す、[plannerTask](plannertask.md) リソースの担当者の[順序に関するヒント](planner-order-hint-format.md)が含まれます。この型はオープン型です。プロパティは、タスクに割り当てられているユーザーの ID で、値は順序のヒントです。</span><span class="sxs-lookup"><span data-stu-id="0ac30-p102">The **plannerOrderHintsByAssignee** is a resource that contains [ordering hints](planner-order-hint-format.md) for assignees in a [plannerTask](plannertask.md) resource, to indicate the order of the task in Assigned To view of the Task Board. This type is an open type. The properties are the ids of users assigned to the task, and the values are order hints.</span></span>

## <a name="properties"></a><span data-ttu-id="0ac30-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0ac30-109">Properties</span></span>
<span data-ttu-id="0ac30-p103">クライアントは、オープン型のプロパティを定義できます。この場合、クライアントは、タスクに割り当てられているユーザーの ID をプロパティ名として指定し、有効な[順序のヒント](planner-order-hint-format.md)を値として指定する必要があります。プロパティは、この型から削除できません。サービスは、含まれている [plannerTask](plannertask.md) の割り当てが更新されると、値を自動的に削除します</span><span class="sxs-lookup"><span data-stu-id="0ac30-p103">Properties of an Open Type can be defined by the client. In this case, the client must provide ids of users assigned to the task as property names, and a valid [order hint](planner-order-hint-format.md) as the value. Properties cannot be removed from this type. The service will automatically remove values as the assignments on the containing [plannerTask](plannertask.md) are updated.</span></span>

<span data-ttu-id="0ac30-114">例:</span><span class="sxs-lookup"><span data-stu-id="0ac30-114">Example:</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerOrderHintsByAssignee"
}-->

```json
{
  "ca2a1df2-e36b-4987-9f6b-0ea462f4eb47": "String",
  "4e98f8f1-bb03-4015-b8e0-19bb370949d8": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerOrderHintsByAssignee resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->