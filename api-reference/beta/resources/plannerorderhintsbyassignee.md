---
title: plannerOrderHintsByAssignee リソースの種類
description: '**plannerOrderHintsByAssignee**は、タスクに割り当てられたタスクの順序を示すために、タスクリソースの担当者の注文ヒントを含むリソースです。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 428944f9d622bba8db5d700b8d113a2c5b476301
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344439"
---
# <a name="plannerorderhintsbyassignee-resource-type"></a><span data-ttu-id="e3e8d-103">plannerOrderHintsByAssignee リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e3e8d-103">plannerOrderHintsByAssignee resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e3e8d-104">**plannerOrderHintsByAssignee**は、タスクに割り当てられたタスクの順序を示すために、[タスク](plannertask.md)リソースの担当者の注文[ヒント](planner-order-hint-format.md)を含むリソースです。</span><span class="sxs-lookup"><span data-stu-id="e3e8d-104">The **plannerOrderHintsByAssignee** is a resource that contains [ordering hints](planner-order-hint-format.md) for assignees in a [plannerTask](plannertask.md) resource, to indicate the order of the task in Assigned To view of the Task Board.</span></span>
<span data-ttu-id="e3e8d-105">この型はオープン型です。</span><span class="sxs-lookup"><span data-stu-id="e3e8d-105">This type is an open type.</span></span> <span data-ttu-id="e3e8d-106">プロパティは、タスクに割り当てられたユーザーの id であり、値は order ヒントです。</span><span class="sxs-lookup"><span data-stu-id="e3e8d-106">The properties are the ids of users assigned to the task, and the values are order hints.</span></span>

## <a name="properties"></a><span data-ttu-id="e3e8d-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e3e8d-107">Properties</span></span>
<span data-ttu-id="e3e8d-108">オープン型のプロパティは、クライアントで定義できます。</span><span class="sxs-lookup"><span data-stu-id="e3e8d-108">Properties of an Open Type can be defined by the client.</span></span> <span data-ttu-id="e3e8d-109">この場合、クライアントは、タスクに割り当てられているユーザーの id をプロパティ名として指定し、有効な[順序ヒント](planner-order-hint-format.md)を値として指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="e3e8d-109">In this case, the client must provide ids of users assigned to the task as property names, and a valid [order hint](planner-order-hint-format.md) as the value.</span></span>
<span data-ttu-id="e3e8d-110">プロパティをこの型から削除することはできません。</span><span class="sxs-lookup"><span data-stu-id="e3e8d-110">Properties cannot be removed from this type.</span></span> <span data-ttu-id="e3e8d-111">このサービスは、を含む[プランのタスク](plannertask.md)が更新されたときに、自動的に値を削除します。</span><span class="sxs-lookup"><span data-stu-id="e3e8d-111">The service will automatically remove values as the assignments on the containing [plannerTask](plannertask.md) are updated.</span></span>

<span data-ttu-id="e3e8d-112">例:</span><span class="sxs-lookup"><span data-stu-id="e3e8d-112">Example:</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "plannerOrderHintsByAssignee resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
