---
title: plannerAssignedToTaskBoardTaskFormat リソースの種類
description: '**PlannerAssignedToTaskBoardTaskFormat** リソースは、タスク ボードの AssignedTo ビューを正しく表示するための情報を示します (ビューはタスクが割り当てられているユーザーごとに整理されます)。各 **task** にはそれぞれ plannerAssignedToTaskBoardTaskFormat オブジェクトが 1 つ関連付けられています。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 6a7aa230a610ec63559797d058cbc3f64ffe843d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529818"
---
# <a name="plannerassignedtotaskboardtaskformat-resource-type"></a><span data-ttu-id="70416-104">plannerAssignedToTaskBoardTaskFormat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="70416-104">plannerAssignedToTaskBoardTaskFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="70416-p102">**PlannerAssignedToTaskBoardTaskFormat** リソースは、タスク ボードの AssignedTo ビューを正しく表示するための情報を示します (ビューはタスクが割り当てられているユーザーごとに整理されます)。各 [task](plannertask.md) にはそれぞれ **plannerAssignedToTaskBoardTaskFormat** オブジェクトが 1 つ関連付けられています。</span><span class="sxs-lookup"><span data-stu-id="70416-p102">The **plannerAssignedToTaskBoardTaskFormat** resource represents the information used to render a task correctly in the AssignedTo view of the Task Board (a view organized by users to whom tasks are assigned to). Each [task](plannertask.md) will have one **plannerAssignedToTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="70416-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="70416-107">Methods</span></span>

| <span data-ttu-id="70416-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="70416-108">Method</span></span>           | <span data-ttu-id="70416-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="70416-109">Return Type</span></span>    |<span data-ttu-id="70416-110">説明</span><span class="sxs-lookup"><span data-stu-id="70416-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="70416-111">Get plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="70416-111">Get plannerAssignedToTaskBoardTaskFormat</span></span>](../api/plannerassignedtotaskboardtaskformat-get.md) | [<span data-ttu-id="70416-112">plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="70416-112">plannerAssignedToTaskBoardTaskFormat</span></span>](plannerassignedtotaskboardtaskformat.md) |<span data-ttu-id="70416-113">**plannerAssignedToTaskBoardTaskFormat** オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="70416-113">Read properties and relationships of **plannerAssignedToTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="70416-114">Update</span><span class="sxs-lookup"><span data-stu-id="70416-114">Update</span></span>](../api/plannerassignedtotaskboardtaskformat-update.md) | [<span data-ttu-id="70416-115">plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="70416-115">plannerAssignedToTaskBoardTaskFormat</span></span>](plannerassignedtotaskboardtaskformat.md)  |<span data-ttu-id="70416-116">**plannerAssignedToTaskBoardTaskFormat** オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="70416-116">Update **plannerAssignedToTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="70416-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="70416-117">Properties</span></span>
| <span data-ttu-id="70416-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="70416-118">Property</span></span>     | <span data-ttu-id="70416-119">型</span><span class="sxs-lookup"><span data-stu-id="70416-119">Type</span></span>   |<span data-ttu-id="70416-120">説明</span><span class="sxs-lookup"><span data-stu-id="70416-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="70416-121">id</span><span class="sxs-lookup"><span data-stu-id="70416-121">id</span></span>|<span data-ttu-id="70416-122">String</span><span class="sxs-lookup"><span data-stu-id="70416-122">String</span></span>| <span data-ttu-id="70416-123">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="70416-123">Read-only.</span></span> <span data-ttu-id="70416-124">リソースの ID です。</span><span class="sxs-lookup"><span data-stu-id="70416-124">ID of the resource.</span></span> <span data-ttu-id="70416-125">28 の文字、大文字小文字を区別することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="70416-125">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="70416-126">サービスの[フォーマットの検証](tasks-identifiers-disclaimer.md)が行われます。</span><span class="sxs-lookup"><span data-stu-id="70416-126">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="70416-127">orderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="70416-127">orderHintsByAssignee</span></span>|[<span data-ttu-id="70416-128">plannerOrderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="70416-128">plannerOrderHintsByAssignee</span></span>](plannerorderhintsbyassignee.md)|<span data-ttu-id="70416-p104">タスク ボードの AssignedTo ビューでのタスクの順序付けに使用するヒントのディクショナリ。各エントリのキーは、タスクが割り当てられているユーザーのいずれかであり、値は順序のヒントです。それぞれの値の形式は[ここ](planner-order-hint-format.md)で説明するとおり定義されます。</span><span class="sxs-lookup"><span data-stu-id="70416-p104">Dictionary of hints used to order tasks on the AssignedTo view of the Task Board. The key of each entry is one of the users the task is assigned to and the value is the order hint. The format of each value is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="70416-132">unassignedOrderHint</span><span class="sxs-lookup"><span data-stu-id="70416-132">unassignedOrderHint</span></span>|<span data-ttu-id="70416-133">String</span><span class="sxs-lookup"><span data-stu-id="70416-133">String</span></span>|<span data-ttu-id="70416-p105">タスクが誰にも割り当てられていない場合、または orderHintsByAssignee ディクショナリに、タスクが割り当てられているユーザーのヒントの順序が指定されない場合に、タスク ボードの AssignedTo ビューでのタスクの順序付けに使用するヒントの値。形式は[ここ](planner-order-hint-format.md)の説明に従って定義されます。</span><span class="sxs-lookup"><span data-stu-id="70416-p105">Hint value used to order the task on the AssignedTo view of the Task Board when the task is not assigned to anyone, or if the orderHintsByAssignee dictionary does not provide an order hint for the user the task is assigned to. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="70416-136">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="70416-136">Relationships</span></span>
<span data-ttu-id="70416-137">なし</span><span class="sxs-lookup"><span data-stu-id="70416-137">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="70416-138">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="70416-138">JSON representation</span></span>
<span data-ttu-id="70416-139">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="70416-139">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerassignedtotaskboardtaskformat.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
