---
title: plannerProgressTaskBoardTaskFormat リソースの種類
description: '**plannerProgressTaskBoardTaskFormat** リソースは、タスク ボードの進行状況ビューにタスクを正しく表示するための情報を示します (ビューはタスク オブジェクトの [未開始]、[処理中]、[完了] の列に示す PercentComplete フィールドの状態で整理されます)。各 task にはそれぞれ **plannerProgressTaskBoardTaskFormat** オブジェクトが 1 つ関連付けられています。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 5b6989751a5ad32a40530d568ae1e0e04f25f6d4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938470"
---
# <a name="plannerprogresstaskboardtaskformat-resource-type"></a><span data-ttu-id="93059-104">plannerProgressTaskBoardTaskFormat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="93059-104">plannerProgressTaskBoardTaskFormat resource type</span></span>

<span data-ttu-id="93059-p102">**plannerProgressTaskBoardTaskFormat** リソースは、タスク ボードの進行状況ビューにタスクを正しく表示するための情報を示します (ビューはタスク オブジェクトの [未開始]、[処理中]、[完了] の列に示す PercentComplete フィールドの状態で整理されます)。各 [task](plannertask.md) にはそれぞれ **plannerProgressTaskBoardTaskFormat** オブジェクトが 1 つ関連付けられています。</span><span class="sxs-lookup"><span data-stu-id="93059-p102">The **plannerProgressTaskBoardTaskFormat** resource represents the information used to render a task correctly in the Progress view of the Task Board (a view organized by the state of the PercentComplete field on the task object, with columns for Not Started, In Progress and Complete). Each [task](plannertask.md) will have one **plannerProgressTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="93059-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="93059-107">Methods</span></span>

| <span data-ttu-id="93059-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="93059-108">Method</span></span>           | <span data-ttu-id="93059-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="93059-109">Return Type</span></span>    |<span data-ttu-id="93059-110">説明</span><span class="sxs-lookup"><span data-stu-id="93059-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="93059-111">Get plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="93059-111">Get plannerProgressTaskBoardTaskFormat</span></span>](../api/plannerprogresstaskboardtaskformat-get.md) | [<span data-ttu-id="93059-112">plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="93059-112">plannerProgressTaskBoardTaskFormat</span></span>](plannerprogresstaskboardtaskformat.md) |<span data-ttu-id="93059-113">**plannerProgressTaskBoardTaskFormat** オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="93059-113">Read properties and relationships of **plannerProgressTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="93059-114">Update</span><span class="sxs-lookup"><span data-stu-id="93059-114">Update</span></span>](../api/plannerprogresstaskboardtaskformat-update.md) | [<span data-ttu-id="93059-115">plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="93059-115">plannerProgressTaskBoardTaskFormat</span></span>](plannerprogresstaskboardtaskformat.md)    |<span data-ttu-id="93059-116">**plannerProgressTaskBoardTaskFormat** オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="93059-116">Update **plannerProgressTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="93059-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="93059-117">Properties</span></span>
| <span data-ttu-id="93059-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="93059-118">Property</span></span>     | <span data-ttu-id="93059-119">種類</span><span class="sxs-lookup"><span data-stu-id="93059-119">Type</span></span>   |<span data-ttu-id="93059-120">説明</span><span class="sxs-lookup"><span data-stu-id="93059-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="93059-121">ID</span><span class="sxs-lookup"><span data-stu-id="93059-121">id</span></span>|<span data-ttu-id="93059-122">String</span><span class="sxs-lookup"><span data-stu-id="93059-122">String</span></span>| <span data-ttu-id="93059-123">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="93059-123">Read-only.</span></span> <span data-ttu-id="93059-124">リソースの ID です。</span><span class="sxs-lookup"><span data-stu-id="93059-124">ID of the resource.</span></span> <span data-ttu-id="93059-125">28 の文字、大文字小文字を区別することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="93059-125">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="93059-126">サービスの[フォーマットの検証](planner-identifiers-disclaimer.md)が行われます。</span><span class="sxs-lookup"><span data-stu-id="93059-126">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="93059-127">orderHint</span><span class="sxs-lookup"><span data-stu-id="93059-127">orderHint</span></span>|<span data-ttu-id="93059-128">String</span><span class="sxs-lookup"><span data-stu-id="93059-128">String</span></span>|<span data-ttu-id="93059-p104">タスク ボードの進行状況ビューでタスクの順序付けに使用するヒントの値。形式は[ここ](planner-order-hint-format.md)の説明に従って定義されます。</span><span class="sxs-lookup"><span data-stu-id="93059-p104">Hint value used to order the task on the Progress view of the Task Board. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="93059-131">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="93059-131">Relationships</span></span>
<span data-ttu-id="93059-132">なし</span><span class="sxs-lookup"><span data-stu-id="93059-132">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="93059-133">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="93059-133">JSON representation</span></span>
<span data-ttu-id="93059-134">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="93059-134">Here is a JSON representation of the resource.</span></span>

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
