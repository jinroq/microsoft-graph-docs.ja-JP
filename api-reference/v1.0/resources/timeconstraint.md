---
title: timeConstraint リソースの種類
description: 指定したアクティビティの性質と空き時間帯に従って、会議の日時の候補を、特定の時間と曜日に限定します。
ms.openlocfilehash: 82ab18eb09201236f3227c7dd0660519092a3133
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020941"
---
# <a name="timeconstraint-resource-type"></a><span data-ttu-id="d2a06-103">timeConstraint リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d2a06-103">timeConstraint resource type</span></span>

<span data-ttu-id="d2a06-104">指定したアクティビティの性質と空き時間帯に従って、会議の日時の候補を、特定の時間と曜日に限定します。</span><span class="sxs-lookup"><span data-stu-id="d2a06-104">Restricts meeting time suggestions to certain hours and days of the week according to the specified nature of activity and open time slots.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d2a06-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d2a06-105">JSON representation</span></span>

<span data-ttu-id="d2a06-106">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="d2a06-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="d2a06-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d2a06-107">Properties</span></span>
| <span data-ttu-id="d2a06-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d2a06-108">Property</span></span>     | <span data-ttu-id="d2a06-109">型</span><span class="sxs-lookup"><span data-stu-id="d2a06-109">Type</span></span>   |<span data-ttu-id="d2a06-110">説明</span><span class="sxs-lookup"><span data-stu-id="d2a06-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d2a06-111">activityDomain</span><span class="sxs-lookup"><span data-stu-id="d2a06-111">activityDomain</span></span>|<span data-ttu-id="d2a06-112">activityDomain</span><span class="sxs-lookup"><span data-stu-id="d2a06-112">activityDomain</span></span>|<span data-ttu-id="d2a06-113">オプションは、アクティビティの性質です。</span><span class="sxs-lookup"><span data-stu-id="d2a06-113">The nature of the activity, optional.</span></span> <span data-ttu-id="d2a06-114">可能な値: `work`、 `personal`、 `unrestricted`、または`unknown`。</span><span class="sxs-lookup"><span data-stu-id="d2a06-114">The possible values are: `work`, `personal`, `unrestricted`, or `unknown`.</span></span>|
|<span data-ttu-id="d2a06-115">timeslots</span><span class="sxs-lookup"><span data-stu-id="d2a06-115">timeslots</span></span>|<span data-ttu-id="d2a06-116">[timeSlot](timeslot.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="d2a06-116">[timeSlot](timeslot.md) collection</span></span>|<span data-ttu-id="d2a06-117">期間の配列。</span><span class="sxs-lookup"><span data-stu-id="d2a06-117">An array of time periods.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeConstraint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
