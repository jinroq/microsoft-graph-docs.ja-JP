---
title: plannerProgressTaskBoardTaskFormat リソースの種類
description: '**PlannerProgressTaskBoardTaskFormat**リソースは、タスクボードの進行状況ビュー (タスクオブジェクトの達成率フィールドの状態によって整理されたビュー、未開始の列) を表す情報を表します。、実行中、完了)。 各タスクには、1つの**plannerProgressTaskBoardTaskFormat**オブジェクトが関連付けられています。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 6b92cbd231e0cd194b49c11c25d24b93933abbe7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035176"
---
# <a name="plannerprogresstaskboardtaskformat-resource-type"></a><span data-ttu-id="1a83a-104">plannerProgressTaskBoardTaskFormat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1a83a-104">plannerProgressTaskBoardTaskFormat resource type</span></span>

<span data-ttu-id="1a83a-105">**PlannerProgressTaskBoardTaskFormat**リソースは、タスクボードの進行状況ビュー (タスクオブジェクトの達成率フィールドの状態によって整理されたビュー、未開始の列) を表す情報を表します。、実行中、完了)。</span><span class="sxs-lookup"><span data-stu-id="1a83a-105">The **plannerProgressTaskBoardTaskFormat** resource represents the information used to render a task correctly in the Progress view of the Task Board (a view organized by the state of the PercentComplete field on the task object, with columns for Not Started, In Progress and Complete).</span></span> <span data-ttu-id="1a83a-106">各[タスク](plannertask.md)には、1つの**plannerProgressTaskBoardTaskFormat**オブジェクトが関連付けられています。</span><span class="sxs-lookup"><span data-stu-id="1a83a-106">Each [task](plannertask.md) will have one **plannerProgressTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="1a83a-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="1a83a-107">Methods</span></span>

| <span data-ttu-id="1a83a-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="1a83a-108">Method</span></span>           | <span data-ttu-id="1a83a-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="1a83a-109">Return Type</span></span>    |<span data-ttu-id="1a83a-110">説明</span><span class="sxs-lookup"><span data-stu-id="1a83a-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1a83a-111">Get plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="1a83a-111">Get plannerProgressTaskBoardTaskFormat</span></span>](../api/plannerprogresstaskboardtaskformat-get.md) | [<span data-ttu-id="1a83a-112">plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="1a83a-112">plannerProgressTaskBoardTaskFormat</span></span>](plannerprogresstaskboardtaskformat.md) |<span data-ttu-id="1a83a-113">**PlannerProgressTaskBoardTaskFormat**オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="1a83a-113">Read properties and relationships of **plannerProgressTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="1a83a-114">Update</span><span class="sxs-lookup"><span data-stu-id="1a83a-114">Update</span></span>](../api/plannerprogresstaskboardtaskformat-update.md) | [<span data-ttu-id="1a83a-115">plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="1a83a-115">plannerProgressTaskBoardTaskFormat</span></span>](plannerprogresstaskboardtaskformat.md)    |<span data-ttu-id="1a83a-116">**PlannerProgressTaskBoardTaskFormat**オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="1a83a-116">Update **plannerProgressTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="1a83a-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1a83a-117">Properties</span></span>
| <span data-ttu-id="1a83a-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1a83a-118">Property</span></span>     | <span data-ttu-id="1a83a-119">型</span><span class="sxs-lookup"><span data-stu-id="1a83a-119">Type</span></span>   |<span data-ttu-id="1a83a-120">説明</span><span class="sxs-lookup"><span data-stu-id="1a83a-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1a83a-121">id</span><span class="sxs-lookup"><span data-stu-id="1a83a-121">id</span></span>|<span data-ttu-id="1a83a-122">String</span><span class="sxs-lookup"><span data-stu-id="1a83a-122">String</span></span>| <span data-ttu-id="1a83a-123">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="1a83a-123">Read-only.</span></span> <span data-ttu-id="1a83a-124">リソースの ID。</span><span class="sxs-lookup"><span data-stu-id="1a83a-124">ID of the resource.</span></span> <span data-ttu-id="1a83a-125">28 文字長で、大文字と小文字の区別があります。</span><span class="sxs-lookup"><span data-stu-id="1a83a-125">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="1a83a-126">[書式検証](planner-identifiers-disclaimer.md)はサービスによって行われます。</span><span class="sxs-lookup"><span data-stu-id="1a83a-126">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="1a83a-127">orderHint</span><span class="sxs-lookup"><span data-stu-id="1a83a-127">orderHint</span></span>|<span data-ttu-id="1a83a-128">String</span><span class="sxs-lookup"><span data-stu-id="1a83a-128">String</span></span>|<span data-ttu-id="1a83a-p104">タスク ボードの進行状況ビューでタスクの順序付けに使用するヒントの値。形式は[ここ](planner-order-hint-format.md)の説明に従って定義されます。</span><span class="sxs-lookup"><span data-stu-id="1a83a-p104">Hint value used to order the task on the Progress view of the Task Board. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="1a83a-131">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1a83a-131">Relationships</span></span>
<span data-ttu-id="1a83a-132">なし</span><span class="sxs-lookup"><span data-stu-id="1a83a-132">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="1a83a-133">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1a83a-133">JSON representation</span></span>
<span data-ttu-id="1a83a-134">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1a83a-134">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.plannerProgressTaskBoardTaskFormat"
}-->

```json
{
  "id": "String (identifier)",
  "orderHint": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerProgressTaskBoardTaskFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
