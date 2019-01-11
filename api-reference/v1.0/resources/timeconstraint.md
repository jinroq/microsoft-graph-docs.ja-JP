---
title: timeConstraint リソースの種類
description: 指定したアクティビティの性質と空き時間帯に従って、会議の日時の候補を、特定の時間と曜日に限定します。
localization_priority: Normal
ms.openlocfilehash: b6e239abbd0d9f7b4f83df4a60625a2f88131476
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815093"
---
# <a name="timeconstraint-resource-type"></a><span data-ttu-id="7f3f0-103">timeConstraint リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7f3f0-103">timeConstraint resource type</span></span>

<span data-ttu-id="7f3f0-104">指定したアクティビティの性質と空き時間帯に従って、会議の日時の候補を、特定の時間と曜日に限定します。</span><span class="sxs-lookup"><span data-stu-id="7f3f0-104">Restricts meeting time suggestions to certain hours and days of the week according to the specified nature of activity and open time slots.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7f3f0-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7f3f0-105">JSON representation</span></span>

<span data-ttu-id="7f3f0-106">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="7f3f0-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="7f3f0-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7f3f0-107">Properties</span></span>
| <span data-ttu-id="7f3f0-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7f3f0-108">Property</span></span>     | <span data-ttu-id="7f3f0-109">種類</span><span class="sxs-lookup"><span data-stu-id="7f3f0-109">Type</span></span>   |<span data-ttu-id="7f3f0-110">説明</span><span class="sxs-lookup"><span data-stu-id="7f3f0-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7f3f0-111">activityDomain</span><span class="sxs-lookup"><span data-stu-id="7f3f0-111">activityDomain</span></span>|<span data-ttu-id="7f3f0-112">activityDomain</span><span class="sxs-lookup"><span data-stu-id="7f3f0-112">activityDomain</span></span>|<span data-ttu-id="7f3f0-113">オプションは、アクティビティの性質です。</span><span class="sxs-lookup"><span data-stu-id="7f3f0-113">The nature of the activity, optional.</span></span> <span data-ttu-id="7f3f0-114">可能な値: `work`、 `personal`、 `unrestricted`、または`unknown`。</span><span class="sxs-lookup"><span data-stu-id="7f3f0-114">The possible values are: `work`, `personal`, `unrestricted`, or `unknown`.</span></span>|
|<span data-ttu-id="7f3f0-115">timeslots</span><span class="sxs-lookup"><span data-stu-id="7f3f0-115">timeslots</span></span>|<span data-ttu-id="7f3f0-116">[timeSlot](timeslot.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="7f3f0-116">[timeSlot](timeslot.md) collection</span></span>|<span data-ttu-id="7f3f0-117">期間の配列。</span><span class="sxs-lookup"><span data-stu-id="7f3f0-117">An array of time periods.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeConstraint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
