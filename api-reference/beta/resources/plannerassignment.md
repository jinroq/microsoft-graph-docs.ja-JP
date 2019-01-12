---
title: plannerAssignment リソースの種類
description: '**PlannerAssignment**リソースでは、ユーザーにタスクの割り当てを表します。 この型がオープン型の plannerAssignments で使用されます。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 5eaeb00abf7446db1085a7c0d0916b0a7b5b2434
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27963963"
---
# <a name="plannerassignment-resource-type"></a><span data-ttu-id="1c185-104">plannerAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1c185-104">plannerAssignment resource type</span></span>

> <span data-ttu-id="1c185-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1c185-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1c185-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1c185-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1c185-p103">**PlannerAssignment** リソースは、ユーザーに対するタスクの割り当てを表します。この種類は、オープン型の [plannerAssignments](plannerassignments.md) で使用されます。</span><span class="sxs-lookup"><span data-stu-id="1c185-p103">The **plannerAssignment** resource represents the assignment of a task to a user. This type is used in the open type [plannerAssignments](plannerassignments.md).</span></span>


## <a name="properties"></a><span data-ttu-id="1c185-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1c185-109">Properties</span></span>
| <span data-ttu-id="1c185-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1c185-110">Property</span></span>     | <span data-ttu-id="1c185-111">種類</span><span class="sxs-lookup"><span data-stu-id="1c185-111">Type</span></span>   |<span data-ttu-id="1c185-112">説明</span><span class="sxs-lookup"><span data-stu-id="1c185-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1c185-113">assignedBy</span><span class="sxs-lookup"><span data-stu-id="1c185-113">assignedBy</span></span>|[<span data-ttu-id="1c185-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="1c185-114">identitySet</span></span>](identityset.md)|<span data-ttu-id="1c185-115">assignor など、タスクの割り当てを実行したユーザーの ID。</span><span class="sxs-lookup"><span data-stu-id="1c185-115">The identity of the user that performed the assignment of the task, i.e. the assignor.</span></span>|
|<span data-ttu-id="1c185-116">assignedDateTime</span><span class="sxs-lookup"><span data-stu-id="1c185-116">assignedDateTime</span></span>|<span data-ttu-id="1c185-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1c185-117">DateTimeOffset</span></span>|<span data-ttu-id="1c185-p104">タスクが割り当てられた時間。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="1c185-p104">The time at which the task was assigned. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="1c185-121">orderHint</span><span class="sxs-lookup"><span data-stu-id="1c185-121">orderHint</span></span>|<span data-ttu-id="1c185-122">String</span><span class="sxs-lookup"><span data-stu-id="1c185-122">String</span></span>|<span data-ttu-id="1c185-p105">タスクの担当者を並べ替えるために使用するヒント。形式は[ここ](planner-order-hint-format.md)の説明に従って定義されます。</span><span class="sxs-lookup"><span data-stu-id="1c185-p105">Hint used to order assignees in a task. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1c185-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1c185-125">JSON representation</span></span>
<span data-ttu-id="1c185-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1c185-126">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerAssignment"
}-->

```json
{
  "assignedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "assignedDateTime": "String (timestamp)",
  "orderHint": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
