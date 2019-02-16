---
title: findMeetingTimesTimeConstraints リソースの種類
description: 指定したアクティビティの性質と空き時間帯に従って、会議の日時の候補を、特定の時間と曜日に限定します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: e5790faf49fea03040dca05d457fededf5fdd683
ms.sourcegitcommit: 539ed08adf3b7ad3253c98636d4ab303ce00176e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/15/2019
ms.locfileid: "30057404"
---
# <a name="findmeetingtimestimeconstraints-resource-type"></a><span data-ttu-id="50607-103">findMeetingTimesTimeConstraints リソースの種類</span><span class="sxs-lookup"><span data-stu-id="50607-103">findMeetingTimesTimeConstraints resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="50607-104">会議時間の提案を、活動の性質と特定の範囲の時間に制限します。 |</span><span class="sxs-lookup"><span data-stu-id="50607-104">Restricts meeting time suggestions to the nature of activity and certain ranges of time.|</span></span>

## <a name="json-representation"></a><span data-ttu-id="50607-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="50607-105">JSON representation</span></span>

<span data-ttu-id="50607-106">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="50607-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.findMeetingTimesTimeConstraints"
}-->

```json
{
  "activityDomain": "String",
  "timeslots": [{"@odata.type": "microsoft.graph.timeSlot"}]
}

```
## <a name="properties"></a><span data-ttu-id="50607-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="50607-107">Properties</span></span>
| <span data-ttu-id="50607-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="50607-108">Property</span></span>     | <span data-ttu-id="50607-109">型</span><span class="sxs-lookup"><span data-stu-id="50607-109">Type</span></span>   |<span data-ttu-id="50607-110">説明</span><span class="sxs-lookup"><span data-stu-id="50607-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="50607-111">activityDomain</span><span class="sxs-lookup"><span data-stu-id="50607-111">activityDomain</span></span>|<span data-ttu-id="50607-112">activityDomain</span><span class="sxs-lookup"><span data-stu-id="50607-112">activityDomain</span></span>|<span data-ttu-id="50607-p101">アクティビティの性質です (省略可能)。使用可能な値: `work`、`personal`、`unrestricted`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="50607-p101">The nature of the activity, optional. Possible values are: `work`, `personal`, `unrestricted`, or `unknown`.</span></span>|
|<span data-ttu-id="50607-115">timeslots</span><span class="sxs-lookup"><span data-stu-id="50607-115">timeslots</span></span>|<span data-ttu-id="50607-116">[searchwindowtimeslot](searchwindowtimeslot.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="50607-116">[searchWindowTimeSlot](searchwindowtimeslot.md) collection</span></span>|<span data-ttu-id="50607-117">可能な会議時間を検索する時間範囲の配列。</span><span class="sxs-lookup"><span data-stu-id="50607-117">An array of time ranges to look into for possible meeting times.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "findMeetingTimesTimeConstraints resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/findmeetingtimestimeconstraints.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->