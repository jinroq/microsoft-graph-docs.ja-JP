---
title: timeConstraint リソースの種類
description: 指定されたアクティビティの性質および開いている時間帯に従って、会議時間の提案を特定の時間と曜日に制限します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 680ada778ea64f982e9ed5fac11c935a6cce55d5
ms.sourcegitcommit: a90abf5b89dbbdfefb1b7794d1f12c6e2bfb0cda
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/28/2019
ms.locfileid: "30937792"
---
# <a name="timeconstraint-resource-type"></a><span data-ttu-id="7dabc-103">timeConstraint リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7dabc-103">timeConstraint resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7dabc-104">指定されたアクティビティの性質および開いている時間帯に従って、会議時間の提案を特定の時間と曜日に制限します。</span><span class="sxs-lookup"><span data-stu-id="7dabc-104">Restricts meeting time suggestions to certain hours and days of the week according to the specified nature of activity and open time slots.</span></span>


## <a name="json-representation"></a><span data-ttu-id="7dabc-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7dabc-105">JSON representation</span></span>
<span data-ttu-id="7dabc-106">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="7dabc-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeConstraint"
}-->

```json
{
  "activityDomain": "String",
  "timeslots": [{"@odata.type": "microsoft.graph.timeSlot"}]
}
```

## <a name="properties"></a><span data-ttu-id="7dabc-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7dabc-107">Properties</span></span>
| <span data-ttu-id="7dabc-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7dabc-108">Property</span></span>     | <span data-ttu-id="7dabc-109">型</span><span class="sxs-lookup"><span data-stu-id="7dabc-109">Type</span></span>   |<span data-ttu-id="7dabc-110">説明</span><span class="sxs-lookup"><span data-stu-id="7dabc-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7dabc-111">activityDomain</span><span class="sxs-lookup"><span data-stu-id="7dabc-111">activityDomain</span></span>|<span data-ttu-id="7dabc-112">activityDomain</span><span class="sxs-lookup"><span data-stu-id="7dabc-112">activityDomain</span></span>|<span data-ttu-id="7dabc-113">活動の性質です (省略可能)。</span><span class="sxs-lookup"><span data-stu-id="7dabc-113">The nature of the activity, optional.</span></span> <span data-ttu-id="7dabc-114">可能な値は`work`、 `personal`、 `unrestricted`、、 `unknown`またはです。</span><span class="sxs-lookup"><span data-stu-id="7dabc-114">Possible values are: `work`, `personal`, `unrestricted`, or `unknown`.</span></span>|
|<span data-ttu-id="7dabc-115">timeslots</span><span class="sxs-lookup"><span data-stu-id="7dabc-115">timeslots</span></span>|<span data-ttu-id="7dabc-116">[timeSlot](timeslot.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="7dabc-116">[timeSlot](timeslot.md) collection</span></span>|<span data-ttu-id="7dabc-117">期間の配列。</span><span class="sxs-lookup"><span data-stu-id="7dabc-117">An array of time periods.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeConstraint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/timeconstraint.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->