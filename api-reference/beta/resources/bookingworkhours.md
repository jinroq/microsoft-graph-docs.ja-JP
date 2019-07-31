---
title: Bookingwork Hours リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでは、これらの API の使用はサポートされていません。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 4011dd7f5f363afc4d0017d5b8931cc26e9f20e8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974119"
---
# <a name="bookingworkhours-resource-type"></a><span data-ttu-id="67876-104">Bookingwork Hours リソースの種類</span><span class="sxs-lookup"><span data-stu-id="67876-104">bookingWorkHours resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="67876-105">1週間の稼働時間のセットを表します。これは、 [Bookingbusiness](bookingbusiness.md)または[bookingStaffMember](bookingstaffmember.md)に対して使用されます。</span><span class="sxs-lookup"><span data-stu-id="67876-105">Represents the set of working hours in a single day of the week, for a [bookingBusiness](bookingbusiness.md) or [bookingStaffMember](bookingstaffmember.md).</span></span>

## <a name="properties"></a><span data-ttu-id="67876-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="67876-106">Properties</span></span>
| <span data-ttu-id="67876-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="67876-107">Property</span></span>     | <span data-ttu-id="67876-108">型</span><span class="sxs-lookup"><span data-stu-id="67876-108">Type</span></span>   |<span data-ttu-id="67876-109">説明</span><span class="sxs-lookup"><span data-stu-id="67876-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="67876-110">日勤</span><span class="sxs-lookup"><span data-stu-id="67876-110">day</span></span>|<span data-ttu-id="67876-111">String</span><span class="sxs-lookup"><span data-stu-id="67876-111">String</span></span>| <span data-ttu-id="67876-112">このインスタンスで表される曜日。</span><span class="sxs-lookup"><span data-stu-id="67876-112">The day of the week represented by this instance.</span></span> <span data-ttu-id="67876-113">可能な値は、`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday` です。</span><span class="sxs-lookup"><span data-stu-id="67876-113">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="67876-114">timeSlots</span><span class="sxs-lookup"><span data-stu-id="67876-114">timeSlots</span></span>|<span data-ttu-id="67876-115">[Bookingwork timesロット](bookingworktimeslot.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="67876-115">[bookingWorkTimeSlot](bookingworktimeslot.md) collection</span></span>|<span data-ttu-id="67876-116">1日の開始/終了時刻のリスト。</span><span class="sxs-lookup"><span data-stu-id="67876-116">A list of start/end times during a day.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="67876-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="67876-117">JSON representation</span></span>

<span data-ttu-id="67876-118">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="67876-118">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
