---
title: plannerBucketTaskBoardTaskFormat リソースの種類
description: '**plannerBucketTaskBoardTaskFormat** リソースは、タスク ボードのバケット ビューでタスクを正しく表示するための情報を示します (ビューは割り当てられているバケット内のタスクごとに整理されます)。各 task にはそれぞれ **plannerBucketTaskBoardTaskFormat** オブジェクトが 1 つ関連付けられています。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: ea557bad20aa0fd10a73e71902b959913e8fff12
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986195"
---
# <a name="plannerbuckettaskboardtaskformat-resource-type"></a><span data-ttu-id="6a79f-104">plannerBucketTaskBoardTaskFormat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6a79f-104">plannerBucketTaskBoardTaskFormat resource type</span></span>

> <span data-ttu-id="6a79f-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6a79f-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6a79f-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6a79f-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6a79f-p103">**plannerBucketTaskBoardTaskFormat** リソースは、タスク ボードのバケット ビューでタスクを正しく表示するための情報を示します (ビューは割り当てられているバケット内のタスクごとに整理されます)。各 [task](plannertask.md) にはそれぞれ **plannerBucketTaskBoardTaskFormat** オブジェクトが 1 つ関連付けられています。</span><span class="sxs-lookup"><span data-stu-id="6a79f-p103">The **plannerBucketTaskBoardTaskFormat** resource represents the information used to render a task correctly in the Buckets view of the Task Board (a view organized by tasks within the buckets they are assigned to). Each [task](plannertask.md) will have one **plannerBucketTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="6a79f-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="6a79f-109">Methods</span></span>

| <span data-ttu-id="6a79f-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="6a79f-110">Method</span></span>           | <span data-ttu-id="6a79f-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="6a79f-111">Return Type</span></span>    |<span data-ttu-id="6a79f-112">説明</span><span class="sxs-lookup"><span data-stu-id="6a79f-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6a79f-113">plannerBucketTaskBoardTaskFormat の取得</span><span class="sxs-lookup"><span data-stu-id="6a79f-113">Get plannerBucketTaskBoardTaskFormat</span></span>](../api/plannerbuckettaskboardtaskformat-get.md) | [<span data-ttu-id="6a79f-114">plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="6a79f-114">plannerBucketTaskBoardTaskFormat</span></span>](plannerbuckettaskboardtaskformat.md) |<span data-ttu-id="6a79f-115">**plannerBucketTaskBoardTaskFormat** オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="6a79f-115">Read properties and relationships of **plannerBucketTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="6a79f-116">Update</span><span class="sxs-lookup"><span data-stu-id="6a79f-116">Update</span></span>](../api/plannerbuckettaskboardtaskformat-update.md) | [<span data-ttu-id="6a79f-117">plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="6a79f-117">plannerBucketTaskBoardTaskFormat</span></span>](plannerbuckettaskboardtaskformat.md)  |<span data-ttu-id="6a79f-118">**plannerBucketTaskBoardTaskFormat** オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="6a79f-118">Update **plannerBucketTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="6a79f-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6a79f-119">Properties</span></span>
| <span data-ttu-id="6a79f-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6a79f-120">Property</span></span>     | <span data-ttu-id="6a79f-121">種類</span><span class="sxs-lookup"><span data-stu-id="6a79f-121">Type</span></span>   |<span data-ttu-id="6a79f-122">説明</span><span class="sxs-lookup"><span data-stu-id="6a79f-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6a79f-123">ID</span><span class="sxs-lookup"><span data-stu-id="6a79f-123">id</span></span>|<span data-ttu-id="6a79f-124">String</span><span class="sxs-lookup"><span data-stu-id="6a79f-124">String</span></span>| <span data-ttu-id="6a79f-125">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="6a79f-125">Read-only.</span></span> <span data-ttu-id="6a79f-126">リソースの ID です。</span><span class="sxs-lookup"><span data-stu-id="6a79f-126">ID of the resource.</span></span> <span data-ttu-id="6a79f-127">28 の文字、大文字小文字を区別することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="6a79f-127">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="6a79f-128">サービスの[フォーマットの検証](tasks-identifiers-disclaimer.md)が行われます。</span><span class="sxs-lookup"><span data-stu-id="6a79f-128">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="6a79f-129">orderHint</span><span class="sxs-lookup"><span data-stu-id="6a79f-129">orderHint</span></span>|<span data-ttu-id="6a79f-130">String</span><span class="sxs-lookup"><span data-stu-id="6a79f-130">String</span></span>|<span data-ttu-id="6a79f-p105">タスク ボードのバケット ビューでタスクの順序付けに使用するヒント。形式は[ここ](planner-order-hint-format.md)の説明に従って定義されます。</span><span class="sxs-lookup"><span data-stu-id="6a79f-p105">Hint used to order tasks in the Bucket view of the Task Board. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="6a79f-133">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6a79f-133">Relationships</span></span>
<span data-ttu-id="6a79f-134">なし</span><span class="sxs-lookup"><span data-stu-id="6a79f-134">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="6a79f-135">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6a79f-135">JSON representation</span></span>
<span data-ttu-id="6a79f-136">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6a79f-136">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "plannerBucketTaskBoardTaskFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
