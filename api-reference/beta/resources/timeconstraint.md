---
title: timeConstraint リソースの種類
description: 指定されたアクティビティの性質および開いている時間帯に従って、会議時間の提案を特定の時間と曜日に制限します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 8393e4b501815dcbd0195e04ca82cd639d1a84c8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964320"
---
# <a name="timeconstraint-resource-type"></a><span data-ttu-id="0b4cd-103">timeConstraint リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0b4cd-103">timeConstraint resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0b4cd-104">指定されたアクティビティの性質および開いている時間帯に従って、会議時間の提案を特定の時間と曜日に制限します。</span><span class="sxs-lookup"><span data-stu-id="0b4cd-104">Restricts meeting time suggestions to certain hours and days of the week according to the specified nature of activity and open time slots.</span></span>


## <a name="json-representation"></a><span data-ttu-id="0b4cd-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0b4cd-105">JSON representation</span></span>
<span data-ttu-id="0b4cd-106">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="0b4cd-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="0b4cd-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0b4cd-107">Properties</span></span>
| <span data-ttu-id="0b4cd-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0b4cd-108">Property</span></span>     | <span data-ttu-id="0b4cd-109">型</span><span class="sxs-lookup"><span data-stu-id="0b4cd-109">Type</span></span>   |<span data-ttu-id="0b4cd-110">説明</span><span class="sxs-lookup"><span data-stu-id="0b4cd-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0b4cd-111">activityDomain</span><span class="sxs-lookup"><span data-stu-id="0b4cd-111">activityDomain</span></span>|<span data-ttu-id="0b4cd-112">activityDomain</span><span class="sxs-lookup"><span data-stu-id="0b4cd-112">activityDomain</span></span>|<span data-ttu-id="0b4cd-113">活動の性質です (省略可能)。</span><span class="sxs-lookup"><span data-stu-id="0b4cd-113">The nature of the activity, optional.</span></span> <span data-ttu-id="0b4cd-114">可能な値は`work`、 `personal`、 `unrestricted`、、 `unknown`またはです。</span><span class="sxs-lookup"><span data-stu-id="0b4cd-114">Possible values are: `work`, `personal`, `unrestricted`, or `unknown`.</span></span>|
|<span data-ttu-id="0b4cd-115">timeslots</span><span class="sxs-lookup"><span data-stu-id="0b4cd-115">timeslots</span></span>|<span data-ttu-id="0b4cd-116">[timeSlot](timeslot.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="0b4cd-116">[timeSlot](timeslot.md) collection</span></span>|<span data-ttu-id="0b4cd-117">期間の配列。</span><span class="sxs-lookup"><span data-stu-id="0b4cd-117">An array of time periods.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeConstraint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
