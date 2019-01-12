---
title: bookingWorkHours リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: af606cf8ea867c040c20db3b4082761b3de69052
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27958475"
---
# <a name="bookingworkhours-resource-type"></a><span data-ttu-id="7fdd0-104">bookingWorkHours リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7fdd0-104">bookingWorkHours resource type</span></span>

 > <span data-ttu-id="7fdd0-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7fdd0-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7fdd0-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7fdd0-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="7fdd0-107">[BookingBusiness](bookingbusiness.md)または[bookingStaffMember](bookingstaffmember.md)の週の 1 日の稼働時間のセットを表します。</span><span class="sxs-lookup"><span data-stu-id="7fdd0-107">Represents the set of working hours in a single day of the week, for a [bookingBusiness](bookingbusiness.md) or [bookingStaffMember](bookingstaffmember.md).</span></span>

## <a name="properties"></a><span data-ttu-id="7fdd0-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7fdd0-108">Properties</span></span>
| <span data-ttu-id="7fdd0-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7fdd0-109">Property</span></span>     | <span data-ttu-id="7fdd0-110">種類</span><span class="sxs-lookup"><span data-stu-id="7fdd0-110">Type</span></span>   |<span data-ttu-id="7fdd0-111">説明</span><span class="sxs-lookup"><span data-stu-id="7fdd0-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7fdd0-112">1 日</span><span class="sxs-lookup"><span data-stu-id="7fdd0-112">day</span></span>|<span data-ttu-id="7fdd0-113">String</span><span class="sxs-lookup"><span data-stu-id="7fdd0-113">String</span></span>| <span data-ttu-id="7fdd0-114">このインスタンスで表される曜日。</span><span class="sxs-lookup"><span data-stu-id="7fdd0-114">The day of the week represented by this instance.</span></span> <span data-ttu-id="7fdd0-115">可能な値は、`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday` です。</span><span class="sxs-lookup"><span data-stu-id="7fdd0-115">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="7fdd0-116">タイム スロット</span><span class="sxs-lookup"><span data-stu-id="7fdd0-116">timeSlots</span></span>|<span data-ttu-id="7fdd0-117">[bookingWorkTimeSlot](bookingworktimeslot.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="7fdd0-117">[bookingWorkTimeSlot](bookingworktimeslot.md) collection</span></span>|<span data-ttu-id="7fdd0-118">1 日中に開始/終了時刻の一覧です。</span><span class="sxs-lookup"><span data-stu-id="7fdd0-118">A list of start/end times during a day.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7fdd0-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7fdd0-119">JSON representation</span></span>

<span data-ttu-id="7fdd0-120">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7fdd0-120">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "bookingWorkHours resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
