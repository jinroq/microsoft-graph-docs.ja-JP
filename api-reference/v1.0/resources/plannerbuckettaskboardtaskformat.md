---
title: plannerBucketTaskBoardTaskFormat リソースの種類
description: '**PlannerBucketTaskBoardTaskFormat**リソースは、タスクボードのバケットビューでタスクを正しくレンダリングするために使用される情報を表します (割り当てられているバケット内のタスク別に整理されたビュー)。 各タスクには、1つの**plannerBucketTaskBoardTaskFormat**オブジェクトが関連付けられています。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: dcc78f60decaa50f0ac1a2051b84e2f651e11521
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035329"
---
# <a name="plannerbuckettaskboardtaskformat-resource-type"></a><span data-ttu-id="e2653-104">plannerBucketTaskBoardTaskFormat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e2653-104">plannerBucketTaskBoardTaskFormat resource type</span></span>

<span data-ttu-id="e2653-105">**PlannerBucketTaskBoardTaskFormat**リソースは、タスクボードのバケットビューでタスクを正しくレンダリングするために使用される情報を表します (割り当てられているバケット内のタスク別に整理されたビュー)。</span><span class="sxs-lookup"><span data-stu-id="e2653-105">The **plannerBucketTaskBoardTaskFormat** resource represents the information used to render a task correctly in the Buckets view of the Task Board (a view organized by tasks within the buckets they are assigned to).</span></span> <span data-ttu-id="e2653-106">各[タスク](plannertask.md)には、1つの**plannerBucketTaskBoardTaskFormat**オブジェクトが関連付けられています。</span><span class="sxs-lookup"><span data-stu-id="e2653-106">Each [task](plannertask.md) will have one **plannerBucketTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="e2653-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="e2653-107">Methods</span></span>

| <span data-ttu-id="e2653-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="e2653-108">Method</span></span>           | <span data-ttu-id="e2653-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="e2653-109">Return Type</span></span>    |<span data-ttu-id="e2653-110">説明</span><span class="sxs-lookup"><span data-stu-id="e2653-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e2653-111">Get plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="e2653-111">Get plannerBucketTaskBoardTaskFormat</span></span>](../api/plannerbuckettaskboardtaskformat-get.md) | [<span data-ttu-id="e2653-112">plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="e2653-112">plannerBucketTaskBoardTaskFormat</span></span>](plannerbuckettaskboardtaskformat.md) |<span data-ttu-id="e2653-113">**PlannerBucketTaskBoardTaskFormat**オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="e2653-113">Read properties and relationships of **plannerBucketTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="e2653-114">Update</span><span class="sxs-lookup"><span data-stu-id="e2653-114">Update</span></span>](../api/plannerbuckettaskboardtaskformat-update.md) | [<span data-ttu-id="e2653-115">plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="e2653-115">plannerBucketTaskBoardTaskFormat</span></span>](plannerbuckettaskboardtaskformat.md)  |<span data-ttu-id="e2653-116">**PlannerBucketTaskBoardTaskFormat**オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="e2653-116">Update **plannerBucketTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="e2653-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e2653-117">Properties</span></span>
| <span data-ttu-id="e2653-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e2653-118">Property</span></span>     | <span data-ttu-id="e2653-119">型</span><span class="sxs-lookup"><span data-stu-id="e2653-119">Type</span></span>   |<span data-ttu-id="e2653-120">説明</span><span class="sxs-lookup"><span data-stu-id="e2653-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e2653-121">id</span><span class="sxs-lookup"><span data-stu-id="e2653-121">id</span></span>|<span data-ttu-id="e2653-122">String</span><span class="sxs-lookup"><span data-stu-id="e2653-122">String</span></span>| <span data-ttu-id="e2653-123">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="e2653-123">Read-only.</span></span> <span data-ttu-id="e2653-124">リソースの ID。</span><span class="sxs-lookup"><span data-stu-id="e2653-124">ID of the resource.</span></span> <span data-ttu-id="e2653-125">28 文字長で、大文字と小文字の区別があります。</span><span class="sxs-lookup"><span data-stu-id="e2653-125">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="e2653-126">[書式検証](planner-identifiers-disclaimer.md)はサービスによって行われます。</span><span class="sxs-lookup"><span data-stu-id="e2653-126">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="e2653-127">orderHint</span><span class="sxs-lookup"><span data-stu-id="e2653-127">orderHint</span></span>|<span data-ttu-id="e2653-128">String</span><span class="sxs-lookup"><span data-stu-id="e2653-128">String</span></span>|<span data-ttu-id="e2653-p104">タスク ボードのバケット ビューでタスクの順序付けに使用するヒント。形式は[ここ](planner-order-hint-format.md)の説明に従って定義されます。</span><span class="sxs-lookup"><span data-stu-id="e2653-p104">Hint used to order tasks in the Bucket view of the Task Board. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="e2653-131">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e2653-131">Relationships</span></span>
<span data-ttu-id="e2653-132">なし</span><span class="sxs-lookup"><span data-stu-id="e2653-132">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="e2653-133">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e2653-133">JSON representation</span></span>
<span data-ttu-id="e2653-134">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e2653-134">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.plannerBucketTaskBoardTaskFormat"
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
  "description": "plannerBucketTaskBoardTaskFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
