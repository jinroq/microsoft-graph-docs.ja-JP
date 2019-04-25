---
title: plan/assignment リソースの種類
description: '[ **plan] 割り当て**リソースは、ユーザーに対するタスクの割り当てを表します。 この型は、オープンタイププランの割り当てで使用されます。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 054cd42eedd27a7fe11abc2e5578a56da667e05d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32541361"
---
# <a name="plannerassignment-resource-type"></a><span data-ttu-id="4cdd2-104">plan/assignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4cdd2-104">plannerAssignment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4cdd2-105">[ **plan] 割り当て**リソースは、ユーザーに対するタスクの割り当てを表します。</span><span class="sxs-lookup"><span data-stu-id="4cdd2-105">The **plannerAssignment** resource represents the assignment of a task to a user.</span></span> <span data-ttu-id="4cdd2-106">この型は、オープンタイププランの[割り当て](plannerassignments.md)で使用されます。</span><span class="sxs-lookup"><span data-stu-id="4cdd2-106">This type is used in the open type [plannerAssignments](plannerassignments.md).</span></span>


## <a name="properties"></a><span data-ttu-id="4cdd2-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4cdd2-107">Properties</span></span>
| <span data-ttu-id="4cdd2-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4cdd2-108">Property</span></span>     | <span data-ttu-id="4cdd2-109">型</span><span class="sxs-lookup"><span data-stu-id="4cdd2-109">Type</span></span>   |<span data-ttu-id="4cdd2-110">説明</span><span class="sxs-lookup"><span data-stu-id="4cdd2-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4cdd2-111">assignedBy</span><span class="sxs-lookup"><span data-stu-id="4cdd2-111">assignedBy</span></span>|[<span data-ttu-id="4cdd2-112">identitySet</span><span class="sxs-lookup"><span data-stu-id="4cdd2-112">identitySet</span></span>](identityset.md)|<span data-ttu-id="4cdd2-113">タスクの割り当てを実行したユーザーの id。つまり、割り当てまたは。</span><span class="sxs-lookup"><span data-stu-id="4cdd2-113">The identity of the user that performed the assignment of the task, i.e. the assignor.</span></span>|
|<span data-ttu-id="4cdd2-114">assignedDateTime</span><span class="sxs-lookup"><span data-stu-id="4cdd2-114">assignedDateTime</span></span>|<span data-ttu-id="4cdd2-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4cdd2-115">DateTimeOffset</span></span>|<span data-ttu-id="4cdd2-116">タスクが割り当てられた日時。</span><span class="sxs-lookup"><span data-stu-id="4cdd2-116">The time at which the task was assigned.</span></span> <span data-ttu-id="4cdd2-117">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="4cdd2-117">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="4cdd2-118">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="4cdd2-118">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="4cdd2-119">orderHint</span><span class="sxs-lookup"><span data-stu-id="4cdd2-119">orderHint</span></span>|<span data-ttu-id="4cdd2-120">String</span><span class="sxs-lookup"><span data-stu-id="4cdd2-120">String</span></span>|<span data-ttu-id="4cdd2-121">タスクの担当者を注文するために使用されるヒント。</span><span class="sxs-lookup"><span data-stu-id="4cdd2-121">Hint used to order assignees in a task.</span></span> <span data-ttu-id="4cdd2-122">この形式は、[ここで](planner-order-hint-format.md)説明するように定義されています。</span><span class="sxs-lookup"><span data-stu-id="4cdd2-122">The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4cdd2-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4cdd2-123">JSON representation</span></span>
<span data-ttu-id="4cdd2-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4cdd2-124">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerassignment.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
