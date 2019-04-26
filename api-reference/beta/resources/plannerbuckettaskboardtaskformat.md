---
title: plannerBucketTaskBoardTaskFormat リソースの種類
description: '**plannerBucketTaskBoardTaskFormat**リソースは、タスクボードのバケットビューでタスクを正しくレンダリングするために使用される情報を表します (割り当てられているバケット内のタスク別に整理されたビュー)。 各タスクには、1つの**plannerBucketTaskBoardTaskFormat**オブジェクトが関連付けられています。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: d40234fd729b849fee9fa789b9ae410eb0147f45
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344595"
---
# <a name="plannerbuckettaskboardtaskformat-resource-type"></a><span data-ttu-id="1e907-104">plannerBucketTaskBoardTaskFormat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1e907-104">plannerBucketTaskBoardTaskFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1e907-105">**plannerBucketTaskBoardTaskFormat**リソースは、タスクボードのバケットビューでタスクを正しくレンダリングするために使用される情報を表します (割り当てられているバケット内のタスク別に整理されたビュー)。</span><span class="sxs-lookup"><span data-stu-id="1e907-105">The **plannerBucketTaskBoardTaskFormat** resource represents the information used to render a task correctly in the Buckets view of the Task Board (a view organized by tasks within the buckets they are assigned to).</span></span> <span data-ttu-id="1e907-106">各[タスク](plannertask.md)には、1つの**plannerBucketTaskBoardTaskFormat**オブジェクトが関連付けられています。</span><span class="sxs-lookup"><span data-stu-id="1e907-106">Each [task](plannertask.md) will have one **plannerBucketTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="1e907-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="1e907-107">Methods</span></span>

| <span data-ttu-id="1e907-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="1e907-108">Method</span></span>           | <span data-ttu-id="1e907-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="1e907-109">Return Type</span></span>    |<span data-ttu-id="1e907-110">説明</span><span class="sxs-lookup"><span data-stu-id="1e907-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1e907-111">Get plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="1e907-111">Get plannerBucketTaskBoardTaskFormat</span></span>](../api/plannerbuckettaskboardtaskformat-get.md) | [<span data-ttu-id="1e907-112">plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="1e907-112">plannerBucketTaskBoardTaskFormat</span></span>](plannerbuckettaskboardtaskformat.md) |<span data-ttu-id="1e907-113">**plannerBucketTaskBoardTaskFormat**オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="1e907-113">Read properties and relationships of **plannerBucketTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="1e907-114">更新する</span><span class="sxs-lookup"><span data-stu-id="1e907-114">Update</span></span>](../api/plannerbuckettaskboardtaskformat-update.md) | [<span data-ttu-id="1e907-115">plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="1e907-115">plannerBucketTaskBoardTaskFormat</span></span>](plannerbuckettaskboardtaskformat.md)  |<span data-ttu-id="1e907-116">**plannerBucketTaskBoardTaskFormat**オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="1e907-116">Update **plannerBucketTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="1e907-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1e907-117">Properties</span></span>
| <span data-ttu-id="1e907-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1e907-118">Property</span></span>     | <span data-ttu-id="1e907-119">型</span><span class="sxs-lookup"><span data-stu-id="1e907-119">Type</span></span>   |<span data-ttu-id="1e907-120">説明</span><span class="sxs-lookup"><span data-stu-id="1e907-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1e907-121">id</span><span class="sxs-lookup"><span data-stu-id="1e907-121">id</span></span>|<span data-ttu-id="1e907-122">String</span><span class="sxs-lookup"><span data-stu-id="1e907-122">String</span></span>| <span data-ttu-id="1e907-123">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="1e907-123">Read-only.</span></span> <span data-ttu-id="1e907-124">リソースの ID。</span><span class="sxs-lookup"><span data-stu-id="1e907-124">ID of the resource.</span></span> <span data-ttu-id="1e907-125">28 文字長で、大文字と小文字の区別があります。</span><span class="sxs-lookup"><span data-stu-id="1e907-125">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="1e907-126">[書式検証](tasks-identifiers-disclaimer.md)はサービスによって行われます。</span><span class="sxs-lookup"><span data-stu-id="1e907-126">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="1e907-127">orderHint</span><span class="sxs-lookup"><span data-stu-id="1e907-127">orderHint</span></span>|<span data-ttu-id="1e907-128">String</span><span class="sxs-lookup"><span data-stu-id="1e907-128">String</span></span>|<span data-ttu-id="1e907-p104">タスク ボードのバケット ビューでタスクの順序付けに使用するヒント。形式は[ここ](planner-order-hint-format.md)の説明に従って定義されます。</span><span class="sxs-lookup"><span data-stu-id="1e907-p104">Hint used to order tasks in the Bucket view of the Task Board. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="1e907-131">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1e907-131">Relationships</span></span>
<span data-ttu-id="1e907-132">なし</span><span class="sxs-lookup"><span data-stu-id="1e907-132">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="1e907-133">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1e907-133">JSON representation</span></span>
<span data-ttu-id="1e907-134">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1e907-134">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
<!--
{
  "type": "#page.annotation",
  "description": "plannerBucketTaskBoardTaskFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
