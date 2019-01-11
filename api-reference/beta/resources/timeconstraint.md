---
title: timeConstraint リソースの種類
description: 指定したアクティビティの性質と空き時間帯に従って、会議の日時の候補を、特定の時間と曜日に限定します。
localization_priority: Normal
ms.openlocfilehash: 6e3cc56f1495eae60bb84c458caa25c79557e033
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27832908"
---
# <a name="timeconstraint-resource-type"></a><span data-ttu-id="9a9fe-103">timeConstraint リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9a9fe-103">timeConstraint resource type</span></span>

> <span data-ttu-id="9a9fe-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9a9fe-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9a9fe-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9a9fe-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9a9fe-106">指定したアクティビティの性質と空き時間帯に従って、会議の日時の候補を、特定の時間と曜日に限定します。</span><span class="sxs-lookup"><span data-stu-id="9a9fe-106">Restricts meeting time suggestions to certain hours and days of the week according to the specified nature of activity and open time slots.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9a9fe-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9a9fe-107">JSON representation</span></span>

<span data-ttu-id="9a9fe-108">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="9a9fe-108">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="9a9fe-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9a9fe-109">Properties</span></span>
| <span data-ttu-id="9a9fe-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9a9fe-110">Property</span></span>     | <span data-ttu-id="9a9fe-111">種類</span><span class="sxs-lookup"><span data-stu-id="9a9fe-111">Type</span></span>   |<span data-ttu-id="9a9fe-112">説明</span><span class="sxs-lookup"><span data-stu-id="9a9fe-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9a9fe-113">activityDomain</span><span class="sxs-lookup"><span data-stu-id="9a9fe-113">activityDomain</span></span>|<span data-ttu-id="9a9fe-114">String</span><span class="sxs-lookup"><span data-stu-id="9a9fe-114">String</span></span>|<span data-ttu-id="9a9fe-p102">アクティビティの性質です (省略可能)。使用可能な値: `work`、`personal`、`unrestricted`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="9a9fe-p102">The nature of the activity, optional. Possible values are: `work`, `personal`, `unrestricted`, or `unknown`.</span></span>|
|<span data-ttu-id="9a9fe-117">timeslots</span><span class="sxs-lookup"><span data-stu-id="9a9fe-117">timeslots</span></span>|<span data-ttu-id="9a9fe-118">[timeSlot](timeslot.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="9a9fe-118">[timeSlot](timeslot.md) collection</span></span>|<span data-ttu-id="9a9fe-119">期間の配列。</span><span class="sxs-lookup"><span data-stu-id="9a9fe-119">An array of time periods.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeConstraint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
