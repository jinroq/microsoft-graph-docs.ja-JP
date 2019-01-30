---
title: timeConstraint リソースの種類
description: 指定したアクティビティの性質と空き時間帯に従って、会議の日時の候補を、特定の時間と曜日に限定します。
localization_priority: Normal
ms.openlocfilehash: 88035d0617523c51bb01ee0a467e8c84785ad6aa
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643567"
---
# <a name="timeconstraint-resource-type"></a><span data-ttu-id="f6177-103">timeConstraint リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f6177-103">timeConstraint resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f6177-104">指定したアクティビティの性質と空き時間帯に従って、会議の日時の候補を、特定の時間と曜日に限定します。</span><span class="sxs-lookup"><span data-stu-id="f6177-104">Restricts meeting time suggestions to certain hours and days of the week according to the specified nature of activity and open time slots.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f6177-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f6177-105">JSON representation</span></span>

<span data-ttu-id="f6177-106">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="f6177-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeconstraint"
}-->

```json
{
  "activityDomain": "String",
  "timeslots": [{"@odata.type": "microsoft.graph.timeSlot"}]
}

```
## <a name="properties"></a><span data-ttu-id="f6177-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f6177-107">Properties</span></span>
| <span data-ttu-id="f6177-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f6177-108">Property</span></span>     | <span data-ttu-id="f6177-109">型</span><span class="sxs-lookup"><span data-stu-id="f6177-109">Type</span></span>   |<span data-ttu-id="f6177-110">説明</span><span class="sxs-lookup"><span data-stu-id="f6177-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f6177-111">activityDomain</span><span class="sxs-lookup"><span data-stu-id="f6177-111">activityDomain</span></span>|<span data-ttu-id="f6177-112">String</span><span class="sxs-lookup"><span data-stu-id="f6177-112">String</span></span>|<span data-ttu-id="f6177-p101">アクティビティの性質です (省略可能)。使用可能な値: `work`、`personal`、`unrestricted`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="f6177-p101">The nature of the activity, optional. Possible values are: `work`, `personal`, `unrestricted`, or `unknown`.</span></span>|
|<span data-ttu-id="f6177-115">timeslots</span><span class="sxs-lookup"><span data-stu-id="f6177-115">timeslots</span></span>|<span data-ttu-id="f6177-116">[timeSlot](timeslot.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="f6177-116">[timeSlot](timeslot.md) collection</span></span>|<span data-ttu-id="f6177-117">期間の配列。</span><span class="sxs-lookup"><span data-stu-id="f6177-117">An array of time periods.</span></span>|

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
