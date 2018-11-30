---
title: plannerBucketTaskBoardTaskFormat リソースの種類
description: '**plannerBucketTaskBoardTaskFormat** リソースは、タスク ボードのバケット ビューでタスクを正しく表示するための情報を示します (ビューは割り当てられているバケット内のタスクごとに整理されます)。各 task にはそれぞれ **plannerBucketTaskBoardTaskFormat** オブジェクトが 1 つ関連付けられています。'
ms.openlocfilehash: 2fa91a4900a12f4c7433049c8ee4be94cdaa7b06
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072589"
---
# <a name="plannerbuckettaskboardtaskformat-resource-type"></a><span data-ttu-id="1144d-104">plannerBucketTaskBoardTaskFormat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1144d-104">plannerBucketTaskBoardTaskFormat resource type</span></span>

> <span data-ttu-id="1144d-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1144d-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1144d-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1144d-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1144d-p103">**plannerBucketTaskBoardTaskFormat** リソースは、タスク ボードのバケット ビューでタスクを正しく表示するための情報を示します (ビューは割り当てられているバケット内のタスクごとに整理されます)。各 [task](plannertask.md) にはそれぞれ **plannerBucketTaskBoardTaskFormat** オブジェクトが 1 つ関連付けられています。</span><span class="sxs-lookup"><span data-stu-id="1144d-p103">The **plannerBucketTaskBoardTaskFormat** resource represents the information used to render a task correctly in the Buckets view of the Task Board (a view organized by tasks within the buckets they are assigned to). Each [task](plannertask.md) will have one **plannerBucketTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="1144d-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="1144d-109">Methods</span></span>

| <span data-ttu-id="1144d-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="1144d-110">Method</span></span>           | <span data-ttu-id="1144d-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="1144d-111">Return Type</span></span>    |<span data-ttu-id="1144d-112">説明</span><span class="sxs-lookup"><span data-stu-id="1144d-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1144d-113">plannerBucketTaskBoardTaskFormat の取得</span><span class="sxs-lookup"><span data-stu-id="1144d-113">Get plannerBucketTaskBoardTaskFormat</span></span>](../api/plannerbuckettaskboardtaskformat-get.md) | [<span data-ttu-id="1144d-114">plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="1144d-114">plannerBucketTaskBoardTaskFormat</span></span>](plannerbuckettaskboardtaskformat.md) |<span data-ttu-id="1144d-115">**plannerBucketTaskBoardTaskFormat** オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="1144d-115">Read properties and relationships of **plannerBucketTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="1144d-116">Update</span><span class="sxs-lookup"><span data-stu-id="1144d-116">Update</span></span>](../api/plannerbuckettaskboardtaskformat-update.md) | [<span data-ttu-id="1144d-117">plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="1144d-117">plannerBucketTaskBoardTaskFormat</span></span>](plannerbuckettaskboardtaskformat.md)  |<span data-ttu-id="1144d-118">**plannerBucketTaskBoardTaskFormat** オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="1144d-118">Update **plannerBucketTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="1144d-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1144d-119">Properties</span></span>
| <span data-ttu-id="1144d-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1144d-120">Property</span></span>     | <span data-ttu-id="1144d-121">型</span><span class="sxs-lookup"><span data-stu-id="1144d-121">Type</span></span>   |<span data-ttu-id="1144d-122">説明</span><span class="sxs-lookup"><span data-stu-id="1144d-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1144d-123">id</span><span class="sxs-lookup"><span data-stu-id="1144d-123">id</span></span>|<span data-ttu-id="1144d-124">String</span><span class="sxs-lookup"><span data-stu-id="1144d-124">String</span></span>| <span data-ttu-id="1144d-125">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="1144d-125">Read-only.</span></span> <span data-ttu-id="1144d-126">リソースの ID です。</span><span class="sxs-lookup"><span data-stu-id="1144d-126">ID of the resource.</span></span> <span data-ttu-id="1144d-127">28 の文字、大文字小文字を区別することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="1144d-127">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="1144d-128">サービスの[フォーマットの検証](tasks-identifiers-disclaimer.md)が行われます。</span><span class="sxs-lookup"><span data-stu-id="1144d-128">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="1144d-129">orderHint</span><span class="sxs-lookup"><span data-stu-id="1144d-129">orderHint</span></span>|<span data-ttu-id="1144d-130">String</span><span class="sxs-lookup"><span data-stu-id="1144d-130">String</span></span>|<span data-ttu-id="1144d-p105">タスク ボードのバケット ビューでタスクの順序付けに使用するヒント。形式は[ここ](planner-order-hint-format.md)の説明に従って定義されます。</span><span class="sxs-lookup"><span data-stu-id="1144d-p105">Hint used to order tasks in the Bucket view of the Task Board. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="1144d-133">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1144d-133">Relationships</span></span>
<span data-ttu-id="1144d-134">なし</span><span class="sxs-lookup"><span data-stu-id="1144d-134">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="1144d-135">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1144d-135">JSON representation</span></span>
<span data-ttu-id="1144d-136">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1144d-136">Here is a JSON representation of the resource.</span></span>

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