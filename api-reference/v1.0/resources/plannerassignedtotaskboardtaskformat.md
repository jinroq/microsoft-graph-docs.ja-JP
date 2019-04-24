---
title: plannerAssignedToTaskBoardTaskFormat リソースの種類
description: '**plannerAssignedToTaskBoardTaskFormat**リソースは、タスクボードの担当者ビューでタスクを正しくレンダリングするために使用される情報を表します (タスクが割り当てられるユーザーによって整理されたビュー)。 各タスクには、1つの**plannerAssignedToTaskBoardTaskFormat**オブジェクトが関連付けられています。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: d59c8c45c998012cacdf4616f1e31f490bec5791
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462313"
---
# <a name="plannerassignedtotaskboardtaskformat-resource-type"></a><span data-ttu-id="11deb-104">plannerAssignedToTaskBoardTaskFormat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="11deb-104">plannerAssignedToTaskBoardTaskFormat resource type</span></span>

<span data-ttu-id="11deb-105">**plannerAssignedToTaskBoardTaskFormat**リソースは、タスクボードの担当者ビューでタスクを正しくレンダリングするために使用される情報を表します (タスクが割り当てられるユーザーによって整理されたビュー)。</span><span class="sxs-lookup"><span data-stu-id="11deb-105">The **plannerAssignedToTaskBoardTaskFormat** resource represents the information used to render a task correctly in the AssignedTo view of the Task Board (a view organized by users to whom tasks are assigned to).</span></span> <span data-ttu-id="11deb-106">各[タスク](plannertask.md)には、1つの**plannerAssignedToTaskBoardTaskFormat**オブジェクトが関連付けられています。</span><span class="sxs-lookup"><span data-stu-id="11deb-106">Each [task](plannertask.md) will have one **plannerAssignedToTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="11deb-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="11deb-107">Methods</span></span>

| <span data-ttu-id="11deb-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="11deb-108">Method</span></span>           | <span data-ttu-id="11deb-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="11deb-109">Return Type</span></span>    |<span data-ttu-id="11deb-110">説明</span><span class="sxs-lookup"><span data-stu-id="11deb-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="11deb-111">Get plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="11deb-111">Get plannerAssignedToTaskBoardTaskFormat</span></span>](../api/plannerassignedtotaskboardtaskformat-get.md) | [<span data-ttu-id="11deb-112">plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="11deb-112">plannerAssignedToTaskBoardTaskFormat</span></span>](plannerassignedtotaskboardtaskformat.md) |<span data-ttu-id="11deb-113">**plannerAssignedToTaskBoardTaskFormat**オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="11deb-113">Read properties and relationships of **plannerAssignedToTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="11deb-114">Update</span><span class="sxs-lookup"><span data-stu-id="11deb-114">Update</span></span>](../api/plannerassignedtotaskboardtaskformat-update.md) | [<span data-ttu-id="11deb-115">plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="11deb-115">plannerAssignedToTaskBoardTaskFormat</span></span>](plannerassignedtotaskboardtaskformat.md)  |<span data-ttu-id="11deb-116">**plannerAssignedToTaskBoardTaskFormat**オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="11deb-116">Update **plannerAssignedToTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="11deb-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="11deb-117">Properties</span></span>
| <span data-ttu-id="11deb-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="11deb-118">Property</span></span>     | <span data-ttu-id="11deb-119">型</span><span class="sxs-lookup"><span data-stu-id="11deb-119">Type</span></span>   |<span data-ttu-id="11deb-120">説明</span><span class="sxs-lookup"><span data-stu-id="11deb-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="11deb-121">id</span><span class="sxs-lookup"><span data-stu-id="11deb-121">id</span></span>|<span data-ttu-id="11deb-122">String</span><span class="sxs-lookup"><span data-stu-id="11deb-122">String</span></span>| <span data-ttu-id="11deb-123">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="11deb-123">Read-only.</span></span> <span data-ttu-id="11deb-124">リソースの ID。</span><span class="sxs-lookup"><span data-stu-id="11deb-124">ID of the resource.</span></span> <span data-ttu-id="11deb-125">28 文字長で、大文字と小文字の区別があります。</span><span class="sxs-lookup"><span data-stu-id="11deb-125">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="11deb-126">[書式検証](planner-identifiers-disclaimer.md)はサービスによって行われます。</span><span class="sxs-lookup"><span data-stu-id="11deb-126">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="11deb-127">orderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="11deb-127">orderHintsByAssignee</span></span>|[<span data-ttu-id="11deb-128">plannerOrderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="11deb-128">plannerOrderHintsByAssignee</span></span>](plannerorderhintsbyassignee.md)|<span data-ttu-id="11deb-p104">タスク ボードの AssignedTo ビューでのタスクの順序付けに使用するヒントのディクショナリ。各エントリのキーは、タスクが割り当てられているユーザーのいずれかであり、値は順序のヒントです。それぞれの値の形式は[ここ](planner-order-hint-format.md)で説明するとおり定義されます。</span><span class="sxs-lookup"><span data-stu-id="11deb-p104">Dictionary of hints used to order tasks on the AssignedTo view of the Task Board. The key of each entry is one of the users the task is assigned to and the value is the order hint. The format of each value is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="11deb-132">unassignedOrderHint</span><span class="sxs-lookup"><span data-stu-id="11deb-132">unassignedOrderHint</span></span>|<span data-ttu-id="11deb-133">String</span><span class="sxs-lookup"><span data-stu-id="11deb-133">String</span></span>|<span data-ttu-id="11deb-p105">タスクが誰にも割り当てられていない場合、または orderHintsByAssignee ディクショナリに、タスクが割り当てられているユーザーのヒントの順序が指定されない場合に、タスク ボードの AssignedTo ビューでのタスクの順序付けに使用するヒントの値。形式は[ここ](planner-order-hint-format.md)の説明に従って定義されます。</span><span class="sxs-lookup"><span data-stu-id="11deb-p105">Hint value used to order the task on the AssignedTo view of the Task Board when the task is not assigned to anyone, or if the orderHintsByAssignee dictionary does not provide an order hint for the user the task is assigned to. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="11deb-136">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="11deb-136">Relationships</span></span>
<span data-ttu-id="11deb-137">なし</span><span class="sxs-lookup"><span data-stu-id="11deb-137">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="11deb-138">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="11deb-138">JSON representation</span></span>
<span data-ttu-id="11deb-139">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="11deb-139">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
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
