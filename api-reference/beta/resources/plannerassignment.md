---
title: Plan/Assignment リソースの種類
description: '[ **Plan] 割り当て**リソースは、ユーザーに対するタスクの割り当てを表します。 この型は、オープンタイププランの割り当てで使用されます。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 27b012374882e98da1669ac0921416bc1a9d1c63
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966042"
---
# <a name="plannerassignment-resource-type"></a><span data-ttu-id="88eed-104">Plan/Assignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="88eed-104">plannerAssignment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="88eed-105">[ **Plan] 割り当て**リソースは、ユーザーに対するタスクの割り当てを表します。</span><span class="sxs-lookup"><span data-stu-id="88eed-105">The **plannerAssignment** resource represents the assignment of a task to a user.</span></span> <span data-ttu-id="88eed-106">この型は、オープンタイププランの[割り当て](plannerassignments.md)で使用されます。</span><span class="sxs-lookup"><span data-stu-id="88eed-106">This type is used in the open type [plannerAssignments](plannerassignments.md).</span></span>


## <a name="properties"></a><span data-ttu-id="88eed-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="88eed-107">Properties</span></span>
| <span data-ttu-id="88eed-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="88eed-108">Property</span></span>     | <span data-ttu-id="88eed-109">型</span><span class="sxs-lookup"><span data-stu-id="88eed-109">Type</span></span>   |<span data-ttu-id="88eed-110">説明</span><span class="sxs-lookup"><span data-stu-id="88eed-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="88eed-111">assignedBy</span><span class="sxs-lookup"><span data-stu-id="88eed-111">assignedBy</span></span>|[<span data-ttu-id="88eed-112">identitySet</span><span class="sxs-lookup"><span data-stu-id="88eed-112">identitySet</span></span>](identityset.md)|<span data-ttu-id="88eed-113">タスクの割り当てを実行したユーザーの id。つまり、割り当てまたは。</span><span class="sxs-lookup"><span data-stu-id="88eed-113">The identity of the user that performed the assignment of the task, i.e. the assignor.</span></span>|
|<span data-ttu-id="88eed-114">assignedDateTime</span><span class="sxs-lookup"><span data-stu-id="88eed-114">assignedDateTime</span></span>|<span data-ttu-id="88eed-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="88eed-115">DateTimeOffset</span></span>|<span data-ttu-id="88eed-116">タスクが割り当てられた日時。</span><span class="sxs-lookup"><span data-stu-id="88eed-116">The time at which the task was assigned.</span></span> <span data-ttu-id="88eed-117">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="88eed-117">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="88eed-118">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="88eed-118">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="88eed-119">orderHint</span><span class="sxs-lookup"><span data-stu-id="88eed-119">orderHint</span></span>|<span data-ttu-id="88eed-120">String</span><span class="sxs-lookup"><span data-stu-id="88eed-120">String</span></span>|<span data-ttu-id="88eed-121">タスクの担当者を注文するために使用されるヒント。</span><span class="sxs-lookup"><span data-stu-id="88eed-121">Hint used to order assignees in a task.</span></span> <span data-ttu-id="88eed-122">この形式は、[ここで](planner-order-hint-format.md)説明するように定義されています。</span><span class="sxs-lookup"><span data-stu-id="88eed-122">The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="88eed-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="88eed-123">JSON representation</span></span>
<span data-ttu-id="88eed-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="88eed-124">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "plannerAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
