---
title: plannerProgressTaskBoardTaskFormat リソースの種類
description: '**plannerProgressTaskBoardTaskFormat**リソースは、タスクボードの進行状況ビュー (タスクオブジェクトの達成率フィールドの状態によって整理されたビュー、未開始の列) を表す情報を表します。、実行中、完了)。 各タスクには、1つの**plannerProgressTaskBoardTaskFormat**オブジェクトが関連付けられています。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 5b6989751a5ad32a40530d568ae1e0e04f25f6d4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462383"
---
# <a name="plannerprogresstaskboardtaskformat-resource-type"></a><span data-ttu-id="86576-104">plannerProgressTaskBoardTaskFormat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="86576-104">plannerProgressTaskBoardTaskFormat resource type</span></span>

<span data-ttu-id="86576-105">**plannerProgressTaskBoardTaskFormat**リソースは、タスクボードの進行状況ビュー (タスクオブジェクトの達成率フィールドの状態によって整理されたビュー、未開始の列) を表す情報を表します。、実行中、完了)。</span><span class="sxs-lookup"><span data-stu-id="86576-105">The **plannerProgressTaskBoardTaskFormat** resource represents the information used to render a task correctly in the Progress view of the Task Board (a view organized by the state of the PercentComplete field on the task object, with columns for Not Started, In Progress and Complete).</span></span> <span data-ttu-id="86576-106">各[タスク](plannertask.md)には、1つの**plannerProgressTaskBoardTaskFormat**オブジェクトが関連付けられています。</span><span class="sxs-lookup"><span data-stu-id="86576-106">Each [task](plannertask.md) will have one **plannerProgressTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="86576-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="86576-107">Methods</span></span>

| <span data-ttu-id="86576-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="86576-108">Method</span></span>           | <span data-ttu-id="86576-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="86576-109">Return Type</span></span>    |<span data-ttu-id="86576-110">説明</span><span class="sxs-lookup"><span data-stu-id="86576-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="86576-111">Get plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="86576-111">Get plannerProgressTaskBoardTaskFormat</span></span>](../api/plannerprogresstaskboardtaskformat-get.md) | [<span data-ttu-id="86576-112">plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="86576-112">plannerProgressTaskBoardTaskFormat</span></span>](plannerprogresstaskboardtaskformat.md) |<span data-ttu-id="86576-113">**plannerProgressTaskBoardTaskFormat**オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="86576-113">Read properties and relationships of **plannerProgressTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="86576-114">Update</span><span class="sxs-lookup"><span data-stu-id="86576-114">Update</span></span>](../api/plannerprogresstaskboardtaskformat-update.md) | [<span data-ttu-id="86576-115">plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="86576-115">plannerProgressTaskBoardTaskFormat</span></span>](plannerprogresstaskboardtaskformat.md)    |<span data-ttu-id="86576-116">**plannerProgressTaskBoardTaskFormat**オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="86576-116">Update **plannerProgressTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="86576-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="86576-117">Properties</span></span>
| <span data-ttu-id="86576-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="86576-118">Property</span></span>     | <span data-ttu-id="86576-119">型</span><span class="sxs-lookup"><span data-stu-id="86576-119">Type</span></span>   |<span data-ttu-id="86576-120">説明</span><span class="sxs-lookup"><span data-stu-id="86576-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="86576-121">id</span><span class="sxs-lookup"><span data-stu-id="86576-121">id</span></span>|<span data-ttu-id="86576-122">String</span><span class="sxs-lookup"><span data-stu-id="86576-122">String</span></span>| <span data-ttu-id="86576-123">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="86576-123">Read-only.</span></span> <span data-ttu-id="86576-124">リソースの ID。</span><span class="sxs-lookup"><span data-stu-id="86576-124">ID of the resource.</span></span> <span data-ttu-id="86576-125">28 文字長で、大文字と小文字の区別があります。</span><span class="sxs-lookup"><span data-stu-id="86576-125">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="86576-126">[書式検証](planner-identifiers-disclaimer.md)はサービスによって行われます。</span><span class="sxs-lookup"><span data-stu-id="86576-126">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="86576-127">orderHint</span><span class="sxs-lookup"><span data-stu-id="86576-127">orderHint</span></span>|<span data-ttu-id="86576-128">String</span><span class="sxs-lookup"><span data-stu-id="86576-128">String</span></span>|<span data-ttu-id="86576-p104">タスク ボードの進行状況ビューでタスクの順序付けに使用するヒントの値。形式は[ここ](planner-order-hint-format.md)の説明に従って定義されます。</span><span class="sxs-lookup"><span data-stu-id="86576-p104">Hint value used to order the task on the Progress view of the Task Board. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="86576-131">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="86576-131">Relationships</span></span>
<span data-ttu-id="86576-132">なし</span><span class="sxs-lookup"><span data-stu-id="86576-132">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="86576-133">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="86576-133">JSON representation</span></span>
<span data-ttu-id="86576-134">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="86576-134">Here is a JSON representation of the resource.</span></span>

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
