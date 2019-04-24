---
title: plannerProgressTaskBoardTaskFormat リソースの種類
description: '**plannerProgressTaskBoardTaskFormat**リソースは、タスクボードの進行状況ビュー (タスクオブジェクトの達成率フィールドの状態によって整理されたビュー、未開始の列) を表す情報を表します。、実行中、完了)。 各タスクには、1つの**plannerProgressTaskBoardTaskFormat**オブジェクトが関連付けられています。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 20a215b108ca1f1801702a532bda09eac67834c6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32522126"
---
# <a name="plannerprogresstaskboardtaskformat-resource-type"></a><span data-ttu-id="dabdc-104">plannerProgressTaskBoardTaskFormat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="dabdc-104">plannerProgressTaskBoardTaskFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dabdc-105">**plannerProgressTaskBoardTaskFormat**リソースは、タスクボードの進行状況ビュー (タスクオブジェクトの達成率フィールドの状態によって整理されたビュー、未開始の列) を表す情報を表します。、実行中、完了)。</span><span class="sxs-lookup"><span data-stu-id="dabdc-105">The **plannerProgressTaskBoardTaskFormat** resource represents the information used to render a task correctly in the Progress view of the Task Board (a view organized by the state of the PercentComplete field on the task object, with columns for Not Started, In Progress and Complete).</span></span> <span data-ttu-id="dabdc-106">各[タスク](plannertask.md)には、1つの**plannerProgressTaskBoardTaskFormat**オブジェクトが関連付けられています。</span><span class="sxs-lookup"><span data-stu-id="dabdc-106">Each [task](plannertask.md) will have one **plannerProgressTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="dabdc-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="dabdc-107">Methods</span></span>

| <span data-ttu-id="dabdc-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="dabdc-108">Method</span></span>           | <span data-ttu-id="dabdc-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="dabdc-109">Return Type</span></span>    |<span data-ttu-id="dabdc-110">説明</span><span class="sxs-lookup"><span data-stu-id="dabdc-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="dabdc-111">Get plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="dabdc-111">Get plannerProgressTaskBoardTaskFormat</span></span>](../api/plannerprogresstaskboardtaskformat-get.md) | [<span data-ttu-id="dabdc-112">plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="dabdc-112">plannerProgressTaskBoardTaskFormat</span></span>](plannerprogresstaskboardtaskformat.md) |<span data-ttu-id="dabdc-113">**plannerProgressTaskBoardTaskFormat**オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="dabdc-113">Read properties and relationships of **plannerProgressTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="dabdc-114">更新する</span><span class="sxs-lookup"><span data-stu-id="dabdc-114">Update</span></span>](../api/plannerprogresstaskboardtaskformat-update.md) | [<span data-ttu-id="dabdc-115">plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="dabdc-115">plannerProgressTaskBoardTaskFormat</span></span>](plannerprogresstaskboardtaskformat.md)    |<span data-ttu-id="dabdc-116">**plannerProgressTaskBoardTaskFormat**オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="dabdc-116">Update **plannerProgressTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="dabdc-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dabdc-117">Properties</span></span>
| <span data-ttu-id="dabdc-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dabdc-118">Property</span></span>     | <span data-ttu-id="dabdc-119">型</span><span class="sxs-lookup"><span data-stu-id="dabdc-119">Type</span></span>   |<span data-ttu-id="dabdc-120">説明</span><span class="sxs-lookup"><span data-stu-id="dabdc-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dabdc-121">id</span><span class="sxs-lookup"><span data-stu-id="dabdc-121">id</span></span>|<span data-ttu-id="dabdc-122">String</span><span class="sxs-lookup"><span data-stu-id="dabdc-122">String</span></span>| <span data-ttu-id="dabdc-123">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="dabdc-123">Read-only.</span></span> <span data-ttu-id="dabdc-124">リソースの ID。</span><span class="sxs-lookup"><span data-stu-id="dabdc-124">ID of the resource.</span></span> <span data-ttu-id="dabdc-125">28 文字長で、大文字と小文字の区別があります。</span><span class="sxs-lookup"><span data-stu-id="dabdc-125">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="dabdc-126">[書式検証](tasks-identifiers-disclaimer.md)はサービスによって行われます。</span><span class="sxs-lookup"><span data-stu-id="dabdc-126">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="dabdc-127">orderHint</span><span class="sxs-lookup"><span data-stu-id="dabdc-127">orderHint</span></span>|<span data-ttu-id="dabdc-128">String</span><span class="sxs-lookup"><span data-stu-id="dabdc-128">String</span></span>|<span data-ttu-id="dabdc-p104">タスク ボードの進行状況ビューでタスクの順序付けに使用するヒントの値。形式は[ここ](planner-order-hint-format.md)の説明に従って定義されます。</span><span class="sxs-lookup"><span data-stu-id="dabdc-p104">Hint value used to order the task on the Progress view of the Task Board. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="dabdc-131">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="dabdc-131">Relationships</span></span>
<span data-ttu-id="dabdc-132">なし</span><span class="sxs-lookup"><span data-stu-id="dabdc-132">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="dabdc-133">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="dabdc-133">JSON representation</span></span>
<span data-ttu-id="dabdc-134">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="dabdc-134">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "plannerProgressTaskBoardTaskFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerprogresstaskboardtaskformat.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
