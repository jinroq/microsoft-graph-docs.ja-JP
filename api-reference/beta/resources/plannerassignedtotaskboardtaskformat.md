---
title: plannerAssignedToTaskBoardTaskFormat リソースの種類
description: '**PlannerAssignedToTaskBoardTaskFormat**リソースは、タスクボードの担当者ビューでタスクを正しくレンダリングするために使用される情報を表します (タスクが割り当てられるユーザーによって整理されたビュー)。 各タスクには、1つの**plannerAssignedToTaskBoardTaskFormat**オブジェクトが関連付けられています。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: a67f085b5e6a7984e1b73358defb28c783d2ec10
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009140"
---
# <a name="plannerassignedtotaskboardtaskformat-resource-type"></a><span data-ttu-id="8284f-104">plannerAssignedToTaskBoardTaskFormat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8284f-104">plannerAssignedToTaskBoardTaskFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8284f-105">**PlannerAssignedToTaskBoardTaskFormat**リソースは、タスクボードの担当者ビューでタスクを正しくレンダリングするために使用される情報を表します (タスクが割り当てられるユーザーによって整理されたビュー)。</span><span class="sxs-lookup"><span data-stu-id="8284f-105">The **plannerAssignedToTaskBoardTaskFormat** resource represents the information used to render a task correctly in the AssignedTo view of the Task Board (a view organized by users to whom tasks are assigned to).</span></span> <span data-ttu-id="8284f-106">各[タスク](plannertask.md)には、1つの**plannerAssignedToTaskBoardTaskFormat**オブジェクトが関連付けられています。</span><span class="sxs-lookup"><span data-stu-id="8284f-106">Each [task](plannertask.md) will have one **plannerAssignedToTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="8284f-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="8284f-107">Methods</span></span>

| <span data-ttu-id="8284f-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="8284f-108">Method</span></span>           | <span data-ttu-id="8284f-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="8284f-109">Return Type</span></span>    |<span data-ttu-id="8284f-110">説明</span><span class="sxs-lookup"><span data-stu-id="8284f-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8284f-111">Get plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="8284f-111">Get plannerAssignedToTaskBoardTaskFormat</span></span>](../api/plannerassignedtotaskboardtaskformat-get.md) | [<span data-ttu-id="8284f-112">plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="8284f-112">plannerAssignedToTaskBoardTaskFormat</span></span>](plannerassignedtotaskboardtaskformat.md) |<span data-ttu-id="8284f-113">**PlannerAssignedToTaskBoardTaskFormat**オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="8284f-113">Read properties and relationships of **plannerAssignedToTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="8284f-114">Update</span><span class="sxs-lookup"><span data-stu-id="8284f-114">Update</span></span>](../api/plannerassignedtotaskboardtaskformat-update.md) | [<span data-ttu-id="8284f-115">plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="8284f-115">plannerAssignedToTaskBoardTaskFormat</span></span>](plannerassignedtotaskboardtaskformat.md)  |<span data-ttu-id="8284f-116">**PlannerAssignedToTaskBoardTaskFormat**オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="8284f-116">Update **plannerAssignedToTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="8284f-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8284f-117">Properties</span></span>
| <span data-ttu-id="8284f-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8284f-118">Property</span></span>     | <span data-ttu-id="8284f-119">型</span><span class="sxs-lookup"><span data-stu-id="8284f-119">Type</span></span>   |<span data-ttu-id="8284f-120">説明</span><span class="sxs-lookup"><span data-stu-id="8284f-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8284f-121">id</span><span class="sxs-lookup"><span data-stu-id="8284f-121">id</span></span>|<span data-ttu-id="8284f-122">String</span><span class="sxs-lookup"><span data-stu-id="8284f-122">String</span></span>| <span data-ttu-id="8284f-123">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="8284f-123">Read-only.</span></span> <span data-ttu-id="8284f-124">リソースの ID。</span><span class="sxs-lookup"><span data-stu-id="8284f-124">ID of the resource.</span></span> <span data-ttu-id="8284f-125">28 文字長で、大文字と小文字の区別があります。</span><span class="sxs-lookup"><span data-stu-id="8284f-125">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="8284f-126">[書式検証](tasks-identifiers-disclaimer.md)はサービスによって行われます。</span><span class="sxs-lookup"><span data-stu-id="8284f-126">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="8284f-127">orderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="8284f-127">orderHintsByAssignee</span></span>|[<span data-ttu-id="8284f-128">plannerOrderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="8284f-128">plannerOrderHintsByAssignee</span></span>](plannerorderhintsbyassignee.md)|<span data-ttu-id="8284f-p104">タスク ボードの AssignedTo ビューでのタスクの順序付けに使用するヒントのディクショナリ。各エントリのキーは、タスクが割り当てられているユーザーのいずれかであり、値は順序のヒントです。それぞれの値の形式は[ここ](planner-order-hint-format.md)で説明するとおり定義されます。</span><span class="sxs-lookup"><span data-stu-id="8284f-p104">Dictionary of hints used to order tasks on the AssignedTo view of the Task Board. The key of each entry is one of the users the task is assigned to and the value is the order hint. The format of each value is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="8284f-132">unassignedOrderHint</span><span class="sxs-lookup"><span data-stu-id="8284f-132">unassignedOrderHint</span></span>|<span data-ttu-id="8284f-133">String</span><span class="sxs-lookup"><span data-stu-id="8284f-133">String</span></span>|<span data-ttu-id="8284f-p105">タスクが誰にも割り当てられていない場合、または orderHintsByAssignee ディクショナリに、タスクが割り当てられているユーザーのヒントの順序が指定されない場合に、タスク ボードの AssignedTo ビューでのタスクの順序付けに使用するヒントの値。形式は[ここ](planner-order-hint-format.md)の説明に従って定義されます。</span><span class="sxs-lookup"><span data-stu-id="8284f-p105">Hint value used to order the task on the AssignedTo view of the Task Board when the task is not assigned to anyone, or if the orderHintsByAssignee dictionary does not provide an order hint for the user the task is assigned to. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="8284f-136">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8284f-136">Relationships</span></span>
<span data-ttu-id="8284f-137">なし</span><span class="sxs-lookup"><span data-stu-id="8284f-137">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="8284f-138">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8284f-138">JSON representation</span></span>
<span data-ttu-id="8284f-139">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8284f-139">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerAssignedToTaskBoardTaskFormat"
}-->

```json
{
  "id": "String (identifier)",
  "orderHintsByAssignee": {"@odata.type": "microsoft.graph.plannerOrderHintsByAssignee"},
  "unassignedOrderHint": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerAssignedToTaskBoardTaskFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
