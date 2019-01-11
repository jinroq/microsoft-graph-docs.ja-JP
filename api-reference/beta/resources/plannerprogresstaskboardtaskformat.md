---
title: plannerProgressTaskBoardTaskFormat リソースの種類
description: '**plannerProgressTaskBoardTaskFormat** リソースは、タスク ボードの進行状況ビューにタスクを正しく表示するための情報を示します (ビューはタスク オブジェクトの [未開始]、[処理中]、[完了] の列に示す PercentComplete フィールドの状態で整理されます)。各 task にはそれぞれ **plannerProgressTaskBoardTaskFormat** オブジェクトが 1 つ関連付けられています。'
localization_priority: Normal
ms.openlocfilehash: 2f3395e0b63d038b8c280e54a76afcc2ca864789
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845585"
---
# <a name="plannerprogresstaskboardtaskformat-resource-type"></a><span data-ttu-id="3c772-104">plannerProgressTaskBoardTaskFormat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3c772-104">plannerProgressTaskBoardTaskFormat resource type</span></span>

> <span data-ttu-id="3c772-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="3c772-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3c772-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3c772-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3c772-p103">**plannerProgressTaskBoardTaskFormat** リソースは、タスク ボードの進行状況ビューにタスクを正しく表示するための情報を示します (ビューはタスク オブジェクトの [未開始]、[処理中]、[完了] の列に示す PercentComplete フィールドの状態で整理されます)。各 [task](plannertask.md) にはそれぞれ **plannerProgressTaskBoardTaskFormat** オブジェクトが 1 つ関連付けられています。</span><span class="sxs-lookup"><span data-stu-id="3c772-p103">The **plannerProgressTaskBoardTaskFormat** resource represents the information used to render a task correctly in the Progress view of the Task Board (a view organized by the state of the PercentComplete field on the task object, with columns for Not Started, In Progress and Complete). Each [task](plannertask.md) will have one **plannerProgressTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="3c772-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="3c772-109">Methods</span></span>

| <span data-ttu-id="3c772-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="3c772-110">Method</span></span>           | <span data-ttu-id="3c772-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="3c772-111">Return Type</span></span>    |<span data-ttu-id="3c772-112">説明</span><span class="sxs-lookup"><span data-stu-id="3c772-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3c772-113">Get plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="3c772-113">Get plannerProgressTaskBoardTaskFormat</span></span>](../api/plannerprogresstaskboardtaskformat-get.md) | [<span data-ttu-id="3c772-114">plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="3c772-114">plannerProgressTaskBoardTaskFormat</span></span>](plannerprogresstaskboardtaskformat.md) |<span data-ttu-id="3c772-115">**plannerProgressTaskBoardTaskFormat** オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="3c772-115">Read properties and relationships of **plannerProgressTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="3c772-116">Update</span><span class="sxs-lookup"><span data-stu-id="3c772-116">Update</span></span>](../api/plannerprogresstaskboardtaskformat-update.md) | [<span data-ttu-id="3c772-117">plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="3c772-117">plannerProgressTaskBoardTaskFormat</span></span>](plannerprogresstaskboardtaskformat.md)    |<span data-ttu-id="3c772-118">**plannerProgressTaskBoardTaskFormat** オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="3c772-118">Update **plannerProgressTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="3c772-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3c772-119">Properties</span></span>
| <span data-ttu-id="3c772-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3c772-120">Property</span></span>     | <span data-ttu-id="3c772-121">種類</span><span class="sxs-lookup"><span data-stu-id="3c772-121">Type</span></span>   |<span data-ttu-id="3c772-122">説明</span><span class="sxs-lookup"><span data-stu-id="3c772-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3c772-123">ID</span><span class="sxs-lookup"><span data-stu-id="3c772-123">id</span></span>|<span data-ttu-id="3c772-124">String</span><span class="sxs-lookup"><span data-stu-id="3c772-124">String</span></span>| <span data-ttu-id="3c772-125">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="3c772-125">Read-only.</span></span> <span data-ttu-id="3c772-126">リソースの ID です。</span><span class="sxs-lookup"><span data-stu-id="3c772-126">ID of the resource.</span></span> <span data-ttu-id="3c772-127">28 の文字、大文字小文字を区別することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="3c772-127">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="3c772-128">サービスの[フォーマットの検証](tasks-identifiers-disclaimer.md)が行われます。</span><span class="sxs-lookup"><span data-stu-id="3c772-128">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="3c772-129">orderHint</span><span class="sxs-lookup"><span data-stu-id="3c772-129">orderHint</span></span>|<span data-ttu-id="3c772-130">String</span><span class="sxs-lookup"><span data-stu-id="3c772-130">String</span></span>|<span data-ttu-id="3c772-p105">タスク ボードの進行状況ビューでタスクの順序付けに使用するヒントの値。形式は[ここ](planner-order-hint-format.md)の説明に従って定義されます。</span><span class="sxs-lookup"><span data-stu-id="3c772-p105">Hint value used to order the task on the Progress view of the Task Board. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="3c772-133">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="3c772-133">Relationships</span></span>
<span data-ttu-id="3c772-134">なし</span><span class="sxs-lookup"><span data-stu-id="3c772-134">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="3c772-135">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3c772-135">JSON representation</span></span>
<span data-ttu-id="3c772-136">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3c772-136">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
