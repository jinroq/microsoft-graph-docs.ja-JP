---
title: bookingwork hours リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 9a51fb9d4f97dde2e3b50d9a19481eeab31483d1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535492"
---
# <a name="bookingworkhours-resource-type"></a><span data-ttu-id="2df66-104">bookingwork hours リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2df66-104">bookingWorkHours resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="2df66-105">1週間の稼働時間のセットを表します。これは、 [bookingbusiness](bookingbusiness.md)または[bookingStaffMember](bookingstaffmember.md)に対して使用されます。</span><span class="sxs-lookup"><span data-stu-id="2df66-105">Represents the set of working hours in a single day of the week, for a [bookingBusiness](bookingbusiness.md) or [bookingStaffMember](bookingstaffmember.md).</span></span>

## <a name="properties"></a><span data-ttu-id="2df66-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2df66-106">Properties</span></span>
| <span data-ttu-id="2df66-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2df66-107">Property</span></span>     | <span data-ttu-id="2df66-108">型</span><span class="sxs-lookup"><span data-stu-id="2df66-108">Type</span></span>   |<span data-ttu-id="2df66-109">説明</span><span class="sxs-lookup"><span data-stu-id="2df66-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2df66-110">日勤</span><span class="sxs-lookup"><span data-stu-id="2df66-110">day</span></span>|<span data-ttu-id="2df66-111">String</span><span class="sxs-lookup"><span data-stu-id="2df66-111">String</span></span>| <span data-ttu-id="2df66-112">このインスタンスで表される曜日。</span><span class="sxs-lookup"><span data-stu-id="2df66-112">The day of the week represented by this instance.</span></span> <span data-ttu-id="2df66-113">可能な値は、`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday` です。</span><span class="sxs-lookup"><span data-stu-id="2df66-113">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="2df66-114">timeSlots</span><span class="sxs-lookup"><span data-stu-id="2df66-114">timeSlots</span></span>|<span data-ttu-id="2df66-115">[bookingwork timesロット](bookingworktimeslot.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="2df66-115">[bookingWorkTimeSlot](bookingworktimeslot.md) collection</span></span>|<span data-ttu-id="2df66-116">1日の開始/終了時刻のリスト。</span><span class="sxs-lookup"><span data-stu-id="2df66-116">A list of start/end times during a day.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2df66-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2df66-117">JSON representation</span></span>

<span data-ttu-id="2df66-118">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2df66-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingWorkHours"
}-->

```json
{
  "day": "String",
  "timeSlots": [{"@odata.type": "microsoft.graph.bookingWorkTimeSlot"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingWorkHours resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/bookingworkhours.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
