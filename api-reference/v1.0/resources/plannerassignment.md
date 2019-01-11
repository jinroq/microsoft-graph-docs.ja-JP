---
title: plannerAssignment リソースの種類
description: '**PlannerAssignment**リソースでは、ユーザーにタスクの割り当てを表します。 この型がオープン型の plannerAssignments で使用されます。'
localization_priority: Normal
ms.openlocfilehash: a2766653fdd7fe29c40529e77bbff2c72e8e6be7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27875685"
---
# <a name="plannerassignment-resource-type"></a><span data-ttu-id="6efc3-104">plannerAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6efc3-104">plannerAssignment resource type</span></span>

<span data-ttu-id="6efc3-p102">**PlannerAssignment** リソースは、ユーザーに対するタスクの割り当てを表します。この種類は、オープン型の [plannerAssignments](plannerassignments.md) で使用されます。</span><span class="sxs-lookup"><span data-stu-id="6efc3-p102">The **plannerAssignment** resource represents the assignment of a task to a user. This type is used in the open type [plannerAssignments](plannerassignments.md).</span></span>


## <a name="properties"></a><span data-ttu-id="6efc3-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6efc3-107">Properties</span></span>
| <span data-ttu-id="6efc3-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6efc3-108">Property</span></span>     | <span data-ttu-id="6efc3-109">種類</span><span class="sxs-lookup"><span data-stu-id="6efc3-109">Type</span></span>   |<span data-ttu-id="6efc3-110">説明</span><span class="sxs-lookup"><span data-stu-id="6efc3-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6efc3-111">assignedBy</span><span class="sxs-lookup"><span data-stu-id="6efc3-111">assignedBy</span></span>|[<span data-ttu-id="6efc3-112">identitySet</span><span class="sxs-lookup"><span data-stu-id="6efc3-112">identitySet</span></span>](identityset.md)|<span data-ttu-id="6efc3-113">assignor など、タスクの割り当てを実行したユーザーの ID。</span><span class="sxs-lookup"><span data-stu-id="6efc3-113">The identity of the user that performed the assignment of the task, i.e. the assignor.</span></span>|
|<span data-ttu-id="6efc3-114">assignedDateTime</span><span class="sxs-lookup"><span data-stu-id="6efc3-114">assignedDateTime</span></span>|<span data-ttu-id="6efc3-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6efc3-115">DateTimeOffset</span></span>|<span data-ttu-id="6efc3-p103">タスクが割り当てられた時間。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="6efc3-p103">The time at which the task was assigned. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="6efc3-119">orderHint</span><span class="sxs-lookup"><span data-stu-id="6efc3-119">orderHint</span></span>|<span data-ttu-id="6efc3-120">String</span><span class="sxs-lookup"><span data-stu-id="6efc3-120">String</span></span>|<span data-ttu-id="6efc3-p104">タスクの担当者を並べ替えるために使用するヒント。形式は[ここ](planner-order-hint-format.md)の説明に従って定義されます。</span><span class="sxs-lookup"><span data-stu-id="6efc3-p104">Hint used to order assignees in a task. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6efc3-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6efc3-123">JSON representation</span></span>
<span data-ttu-id="6efc3-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6efc3-124">Here is a JSON representation of the resource.</span></span>

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
