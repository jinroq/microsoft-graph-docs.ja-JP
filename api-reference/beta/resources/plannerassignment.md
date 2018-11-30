---
title: plannerAssignment リソースの種類
description: '**PlannerAssignment**リソースでは、ユーザーにタスクの割り当てを表します。 この型がオープン型の plannerAssignments で使用されます。'
ms.openlocfilehash: 1efe7c3f2d3229bcce1d2c35e375cc636dadc51f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072582"
---
# <a name="plannerassignment-resource-type"></a><span data-ttu-id="2d2d7-104">plannerAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2d2d7-104">plannerAssignment resource type</span></span>

> <span data-ttu-id="2d2d7-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2d2d7-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2d2d7-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2d2d7-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2d2d7-p103">**PlannerAssignment** リソースは、ユーザーに対するタスクの割り当てを表します。この種類は、オープン型の [plannerAssignments](plannerassignments.md) で使用されます。</span><span class="sxs-lookup"><span data-stu-id="2d2d7-p103">The **plannerAssignment** resource represents the assignment of a task to a user. This type is used in the open type [plannerAssignments](plannerassignments.md).</span></span>


## <a name="properties"></a><span data-ttu-id="2d2d7-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2d2d7-109">Properties</span></span>
| <span data-ttu-id="2d2d7-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2d2d7-110">Property</span></span>     | <span data-ttu-id="2d2d7-111">型</span><span class="sxs-lookup"><span data-stu-id="2d2d7-111">Type</span></span>   |<span data-ttu-id="2d2d7-112">説明</span><span class="sxs-lookup"><span data-stu-id="2d2d7-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2d2d7-113">assignedBy</span><span class="sxs-lookup"><span data-stu-id="2d2d7-113">assignedBy</span></span>|[<span data-ttu-id="2d2d7-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="2d2d7-114">identitySet</span></span>](identityset.md)|<span data-ttu-id="2d2d7-115">assignor など、タスクの割り当てを実行したユーザーの ID。</span><span class="sxs-lookup"><span data-stu-id="2d2d7-115">The identity of the user that performed the assignment of the task, i.e. the assignor.</span></span>|
|<span data-ttu-id="2d2d7-116">assignedDateTime</span><span class="sxs-lookup"><span data-stu-id="2d2d7-116">assignedDateTime</span></span>|<span data-ttu-id="2d2d7-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2d2d7-117">DateTimeOffset</span></span>|<span data-ttu-id="2d2d7-p104">タスクが割り当てられた時間。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="2d2d7-p104">The time at which the task was assigned. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="2d2d7-121">orderHint</span><span class="sxs-lookup"><span data-stu-id="2d2d7-121">orderHint</span></span>|<span data-ttu-id="2d2d7-122">String</span><span class="sxs-lookup"><span data-stu-id="2d2d7-122">String</span></span>|<span data-ttu-id="2d2d7-p105">タスクの担当者を並べ替えるために使用するヒント。形式は[ここ](planner-order-hint-format.md)の説明に従って定義されます。</span><span class="sxs-lookup"><span data-stu-id="2d2d7-p105">Hint used to order assignees in a task. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2d2d7-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2d2d7-125">JSON representation</span></span>
<span data-ttu-id="2d2d7-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2d2d7-126">Here is a JSON representation of the resource.</span></span>

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