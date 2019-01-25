---
title: plannerBucketTaskBoardTaskFormat リソースの種類
description: '**plannerBucketTaskBoardTaskFormat** リソースは、タスク ボードのバケット ビューでタスクを正しく表示するための情報を示します (ビューは割り当てられているバケット内のタスクごとに整理されます)。各 **task** にはそれぞれ plannerBucketTaskBoardTaskFormat オブジェクトが 1 つ関連付けられています。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: eca8865e54d68fb7b403364b065e642ad61e9276
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526950"
---
# <a name="plannerbuckettaskboardtaskformat-resource-type"></a><span data-ttu-id="17a78-104">plannerBucketTaskBoardTaskFormat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="17a78-104">plannerBucketTaskBoardTaskFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="17a78-p102">**plannerBucketTaskBoardTaskFormat** リソースは、タスク ボードのバケット ビューでタスクを正しく表示するための情報を示します (ビューは割り当てられているバケット内のタスクごとに整理されます)。各 [task](plannertask.md) にはそれぞれ **plannerBucketTaskBoardTaskFormat** オブジェクトが 1 つ関連付けられています。</span><span class="sxs-lookup"><span data-stu-id="17a78-p102">The **plannerBucketTaskBoardTaskFormat** resource represents the information used to render a task correctly in the Buckets view of the Task Board (a view organized by tasks within the buckets they are assigned to). Each [task](plannertask.md) will have one **plannerBucketTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="17a78-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="17a78-107">Methods</span></span>

| <span data-ttu-id="17a78-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="17a78-108">Method</span></span>           | <span data-ttu-id="17a78-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="17a78-109">Return Type</span></span>    |<span data-ttu-id="17a78-110">説明</span><span class="sxs-lookup"><span data-stu-id="17a78-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="17a78-111">plannerBucketTaskBoardTaskFormat の取得</span><span class="sxs-lookup"><span data-stu-id="17a78-111">Get plannerBucketTaskBoardTaskFormat</span></span>](../api/plannerbuckettaskboardtaskformat-get.md) | [<span data-ttu-id="17a78-112">plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="17a78-112">plannerBucketTaskBoardTaskFormat</span></span>](plannerbuckettaskboardtaskformat.md) |<span data-ttu-id="17a78-113">**plannerBucketTaskBoardTaskFormat** オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="17a78-113">Read properties and relationships of **plannerBucketTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="17a78-114">Update</span><span class="sxs-lookup"><span data-stu-id="17a78-114">Update</span></span>](../api/plannerbuckettaskboardtaskformat-update.md) | [<span data-ttu-id="17a78-115">plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="17a78-115">plannerBucketTaskBoardTaskFormat</span></span>](plannerbuckettaskboardtaskformat.md)  |<span data-ttu-id="17a78-116">**plannerBucketTaskBoardTaskFormat** オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="17a78-116">Update **plannerBucketTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="17a78-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="17a78-117">Properties</span></span>
| <span data-ttu-id="17a78-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="17a78-118">Property</span></span>     | <span data-ttu-id="17a78-119">型</span><span class="sxs-lookup"><span data-stu-id="17a78-119">Type</span></span>   |<span data-ttu-id="17a78-120">説明</span><span class="sxs-lookup"><span data-stu-id="17a78-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="17a78-121">id</span><span class="sxs-lookup"><span data-stu-id="17a78-121">id</span></span>|<span data-ttu-id="17a78-122">String</span><span class="sxs-lookup"><span data-stu-id="17a78-122">String</span></span>| <span data-ttu-id="17a78-123">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="17a78-123">Read-only.</span></span> <span data-ttu-id="17a78-124">リソースの ID です。</span><span class="sxs-lookup"><span data-stu-id="17a78-124">ID of the resource.</span></span> <span data-ttu-id="17a78-125">28 の文字、大文字小文字を区別することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="17a78-125">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="17a78-126">サービスの[フォーマットの検証](tasks-identifiers-disclaimer.md)が行われます。</span><span class="sxs-lookup"><span data-stu-id="17a78-126">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="17a78-127">orderHint</span><span class="sxs-lookup"><span data-stu-id="17a78-127">orderHint</span></span>|<span data-ttu-id="17a78-128">String</span><span class="sxs-lookup"><span data-stu-id="17a78-128">String</span></span>|<span data-ttu-id="17a78-p104">タスク ボードのバケット ビューでタスクの順序付けに使用するヒント。形式は[ここ](planner-order-hint-format.md)の説明に従って定義されます。</span><span class="sxs-lookup"><span data-stu-id="17a78-p104">Hint used to order tasks in the Bucket view of the Task Board. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="17a78-131">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="17a78-131">Relationships</span></span>
<span data-ttu-id="17a78-132">なし</span><span class="sxs-lookup"><span data-stu-id="17a78-132">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="17a78-133">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="17a78-133">JSON representation</span></span>
<span data-ttu-id="17a78-134">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="17a78-134">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerbuckettaskboardtaskformat.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
