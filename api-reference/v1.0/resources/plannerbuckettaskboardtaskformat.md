---
title: plannerBucketTaskBoardTaskFormat リソースの種類
description: '**plannerBucketTaskBoardTaskFormat** リソースは、タスク ボードのバケット ビューでタスクを正しく表示するための情報を示します (ビューは割り当てられているバケット内のタスクごとに整理されます)。各 task にはそれぞれ **plannerBucketTaskBoardTaskFormat** オブジェクトが 1 つ関連付けられています。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 4982b0b539412058d6d598893b698f12d88bd671
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986223"
---
# <a name="plannerbuckettaskboardtaskformat-resource-type"></a><span data-ttu-id="ae132-104">plannerBucketTaskBoardTaskFormat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ae132-104">plannerBucketTaskBoardTaskFormat resource type</span></span>

<span data-ttu-id="ae132-p102">**plannerBucketTaskBoardTaskFormat** リソースは、タスク ボードのバケット ビューでタスクを正しく表示するための情報を示します (ビューは割り当てられているバケット内のタスクごとに整理されます)。各 [task](plannertask.md) にはそれぞれ **plannerBucketTaskBoardTaskFormat** オブジェクトが 1 つ関連付けられています。</span><span class="sxs-lookup"><span data-stu-id="ae132-p102">The **plannerBucketTaskBoardTaskFormat** resource represents the information used to render a task correctly in the Buckets view of the Task Board (a view organized by tasks within the buckets they are assigned to). Each [task](plannertask.md) will have one **plannerBucketTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="ae132-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="ae132-107">Methods</span></span>

| <span data-ttu-id="ae132-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="ae132-108">Method</span></span>           | <span data-ttu-id="ae132-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ae132-109">Return Type</span></span>    |<span data-ttu-id="ae132-110">説明</span><span class="sxs-lookup"><span data-stu-id="ae132-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ae132-111">plannerBucketTaskBoardTaskFormat の取得</span><span class="sxs-lookup"><span data-stu-id="ae132-111">Get plannerBucketTaskBoardTaskFormat</span></span>](../api/plannerbuckettaskboardtaskformat-get.md) | [<span data-ttu-id="ae132-112">plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="ae132-112">plannerBucketTaskBoardTaskFormat</span></span>](plannerbuckettaskboardtaskformat.md) |<span data-ttu-id="ae132-113">**plannerBucketTaskBoardTaskFormat** オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="ae132-113">Read properties and relationships of **plannerBucketTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="ae132-114">Update</span><span class="sxs-lookup"><span data-stu-id="ae132-114">Update</span></span>](../api/plannerbuckettaskboardtaskformat-update.md) | [<span data-ttu-id="ae132-115">plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="ae132-115">plannerBucketTaskBoardTaskFormat</span></span>](plannerbuckettaskboardtaskformat.md)  |<span data-ttu-id="ae132-116">**plannerBucketTaskBoardTaskFormat** オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="ae132-116">Update **plannerBucketTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="ae132-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ae132-117">Properties</span></span>
| <span data-ttu-id="ae132-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ae132-118">Property</span></span>     | <span data-ttu-id="ae132-119">種類</span><span class="sxs-lookup"><span data-stu-id="ae132-119">Type</span></span>   |<span data-ttu-id="ae132-120">説明</span><span class="sxs-lookup"><span data-stu-id="ae132-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ae132-121">ID</span><span class="sxs-lookup"><span data-stu-id="ae132-121">id</span></span>|<span data-ttu-id="ae132-122">String</span><span class="sxs-lookup"><span data-stu-id="ae132-122">String</span></span>| <span data-ttu-id="ae132-123">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ae132-123">Read-only.</span></span> <span data-ttu-id="ae132-124">リソースの ID です。</span><span class="sxs-lookup"><span data-stu-id="ae132-124">ID of the resource.</span></span> <span data-ttu-id="ae132-125">28 の文字、大文字小文字を区別することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="ae132-125">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="ae132-126">サービスの[フォーマットの検証](planner-identifiers-disclaimer.md)が行われます。</span><span class="sxs-lookup"><span data-stu-id="ae132-126">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="ae132-127">orderHint</span><span class="sxs-lookup"><span data-stu-id="ae132-127">orderHint</span></span>|<span data-ttu-id="ae132-128">String</span><span class="sxs-lookup"><span data-stu-id="ae132-128">String</span></span>|<span data-ttu-id="ae132-p104">タスク ボードのバケット ビューでタスクの順序付けに使用するヒント。形式は[ここ](planner-order-hint-format.md)の説明に従って定義されます。</span><span class="sxs-lookup"><span data-stu-id="ae132-p104">Hint used to order tasks in the Bucket view of the Task Board. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="ae132-131">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ae132-131">Relationships</span></span>
<span data-ttu-id="ae132-132">なし</span><span class="sxs-lookup"><span data-stu-id="ae132-132">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="ae132-133">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ae132-133">JSON representation</span></span>
<span data-ttu-id="ae132-134">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ae132-134">Here is a JSON representation of the resource.</span></span>

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
