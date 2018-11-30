---
title: plannerAssignedToTaskBoardTaskFormat リソースの種類
description: '**PlannerAssignedToTaskBoardTaskFormat** リソースは、タスク ボードの AssignedTo ビューを正しく表示するための情報を示します (ビューはタスクが割り当てられているユーザーごとに整理されます)。各 task にはそれぞれ **plannerAssignedToTaskBoardTaskFormat** オブジェクトが 1 つ関連付けられています。'
ms.openlocfilehash: 8fc96d6fa7d4f05f6bc81f7030ebe766bf769e40
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070624"
---
# <a name="plannerassignedtotaskboardtaskformat-resource-type"></a><span data-ttu-id="2b7fb-104">plannerAssignedToTaskBoardTaskFormat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2b7fb-104">plannerAssignedToTaskBoardTaskFormat resource type</span></span>

> <span data-ttu-id="2b7fb-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2b7fb-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2b7fb-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2b7fb-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2b7fb-p103">**PlannerAssignedToTaskBoardTaskFormat** リソースは、タスク ボードの AssignedTo ビューを正しく表示するための情報を示します (ビューはタスクが割り当てられているユーザーごとに整理されます)。各 [task](plannertask.md) にはそれぞれ **plannerAssignedToTaskBoardTaskFormat** オブジェクトが 1 つ関連付けられています。</span><span class="sxs-lookup"><span data-stu-id="2b7fb-p103">The **plannerAssignedToTaskBoardTaskFormat** resource represents the information used to render a task correctly in the AssignedTo view of the Task Board (a view organized by users to whom tasks are assigned to). Each [task](plannertask.md) will have one **plannerAssignedToTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="2b7fb-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="2b7fb-109">Methods</span></span>

| <span data-ttu-id="2b7fb-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="2b7fb-110">Method</span></span>           | <span data-ttu-id="2b7fb-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="2b7fb-111">Return Type</span></span>    |<span data-ttu-id="2b7fb-112">説明</span><span class="sxs-lookup"><span data-stu-id="2b7fb-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2b7fb-113">Get plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="2b7fb-113">Get plannerAssignedToTaskBoardTaskFormat</span></span>](../api/plannerassignedtotaskboardtaskformat-get.md) | [<span data-ttu-id="2b7fb-114">plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="2b7fb-114">plannerAssignedToTaskBoardTaskFormat</span></span>](plannerassignedtotaskboardtaskformat.md) |<span data-ttu-id="2b7fb-115">**plannerAssignedToTaskBoardTaskFormat** オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="2b7fb-115">Read properties and relationships of **plannerAssignedToTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="2b7fb-116">Update</span><span class="sxs-lookup"><span data-stu-id="2b7fb-116">Update</span></span>](../api/plannerassignedtotaskboardtaskformat-update.md) | [<span data-ttu-id="2b7fb-117">plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="2b7fb-117">plannerAssignedToTaskBoardTaskFormat</span></span>](plannerassignedtotaskboardtaskformat.md)  |<span data-ttu-id="2b7fb-118">**plannerAssignedToTaskBoardTaskFormat** オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="2b7fb-118">Update **plannerAssignedToTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="2b7fb-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2b7fb-119">Properties</span></span>
| <span data-ttu-id="2b7fb-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2b7fb-120">Property</span></span>     | <span data-ttu-id="2b7fb-121">型</span><span class="sxs-lookup"><span data-stu-id="2b7fb-121">Type</span></span>   |<span data-ttu-id="2b7fb-122">説明</span><span class="sxs-lookup"><span data-stu-id="2b7fb-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2b7fb-123">id</span><span class="sxs-lookup"><span data-stu-id="2b7fb-123">id</span></span>|<span data-ttu-id="2b7fb-124">String</span><span class="sxs-lookup"><span data-stu-id="2b7fb-124">String</span></span>| <span data-ttu-id="2b7fb-125">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="2b7fb-125">Read-only.</span></span> <span data-ttu-id="2b7fb-126">リソースの ID です。</span><span class="sxs-lookup"><span data-stu-id="2b7fb-126">ID of the resource.</span></span> <span data-ttu-id="2b7fb-127">28 の文字、大文字小文字を区別することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="2b7fb-127">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="2b7fb-128">サービスの[フォーマットの検証](tasks-identifiers-disclaimer.md)が行われます。</span><span class="sxs-lookup"><span data-stu-id="2b7fb-128">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="2b7fb-129">orderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="2b7fb-129">orderHintsByAssignee</span></span>|[<span data-ttu-id="2b7fb-130">plannerOrderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="2b7fb-130">plannerOrderHintsByAssignee</span></span>](plannerorderhintsbyassignee.md)|<span data-ttu-id="2b7fb-p105">タスク ボードの AssignedTo ビューでのタスクの順序付けに使用するヒントのディクショナリ。各エントリのキーは、タスクが割り当てられているユーザーのいずれかであり、値は順序のヒントです。それぞれの値の形式は[ここ](planner-order-hint-format.md)で説明するとおり定義されます。</span><span class="sxs-lookup"><span data-stu-id="2b7fb-p105">Dictionary of hints used to order tasks on the AssignedTo view of the Task Board. The key of each entry is one of the users the task is assigned to and the value is the order hint. The format of each value is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="2b7fb-134">unassignedOrderHint</span><span class="sxs-lookup"><span data-stu-id="2b7fb-134">unassignedOrderHint</span></span>|<span data-ttu-id="2b7fb-135">String</span><span class="sxs-lookup"><span data-stu-id="2b7fb-135">String</span></span>|<span data-ttu-id="2b7fb-p106">タスクが誰にも割り当てられていない場合、または orderHintsByAssignee ディクショナリに、タスクが割り当てられているユーザーのヒントの順序が指定されない場合に、タスク ボードの AssignedTo ビューでのタスクの順序付けに使用するヒントの値。形式は[ここ](planner-order-hint-format.md)の説明に従って定義されます。</span><span class="sxs-lookup"><span data-stu-id="2b7fb-p106">Hint value used to order the task on the AssignedTo view of the Task Board when the task is not assigned to anyone, or if the orderHintsByAssignee dictionary does not provide an order hint for the user the task is assigned to. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="2b7fb-138">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2b7fb-138">Relationships</span></span>
<span data-ttu-id="2b7fb-139">なし</span><span class="sxs-lookup"><span data-stu-id="2b7fb-139">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="2b7fb-140">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2b7fb-140">JSON representation</span></span>
<span data-ttu-id="2b7fb-141">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2b7fb-141">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "plannerAssignedToTaskBoardTaskFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->