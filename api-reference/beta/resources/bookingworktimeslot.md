---
title: bookingWorkTimeSlot リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 33dd856d678d2cf1ba9da2a747c0bd46f2fd4932
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27968485"
---
# <a name="bookingworktimeslot-resource-type"></a><span data-ttu-id="26e06-104">bookingWorkTimeSlot リソースの種類</span><span class="sxs-lookup"><span data-stu-id="26e06-104">bookingWorkTimeSlot resource type</span></span>

 > <span data-ttu-id="26e06-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="26e06-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="26e06-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="26e06-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="26e06-107">作業の開始と終了時間です。</span><span class="sxs-lookup"><span data-stu-id="26e06-107">The start and end times for work.</span></span>


## <a name="properties"></a><span data-ttu-id="26e06-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="26e06-108">Properties</span></span>
| <span data-ttu-id="26e06-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="26e06-109">Property</span></span>     | <span data-ttu-id="26e06-110">種類</span><span class="sxs-lookup"><span data-stu-id="26e06-110">Type</span></span>   |<span data-ttu-id="26e06-111">説明</span><span class="sxs-lookup"><span data-stu-id="26e06-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="26e06-112">end</span><span class="sxs-lookup"><span data-stu-id="26e06-112">end</span></span>|<span data-ttu-id="26e06-113">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="26e06-113">TimeOfDay</span></span>|<span data-ttu-id="26e06-114">起動時に動作する 1 日の時間。</span><span class="sxs-lookup"><span data-stu-id="26e06-114">The time of the day that work starts.</span></span> <span data-ttu-id="26e06-115">たとえば、08:00:00.0000000 です。</span><span class="sxs-lookup"><span data-stu-id="26e06-115">For example, 08:00:00.0000000.</span></span>|
|<span data-ttu-id="26e06-116">開始</span><span class="sxs-lookup"><span data-stu-id="26e06-116">start</span></span>|<span data-ttu-id="26e06-117">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="26e06-117">TimeOfDay</span></span>|<span data-ttu-id="26e06-118">1 日の時間が停止するを作業です。</span><span class="sxs-lookup"><span data-stu-id="26e06-118">The time of the day that work stops.</span></span> <span data-ttu-id="26e06-119">たとえば、17:00:00.0000000 です。</span><span class="sxs-lookup"><span data-stu-id="26e06-119">For example, 17:00:00.0000000.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="26e06-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="26e06-120">JSON representation</span></span>

<span data-ttu-id="26e06-121">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="26e06-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingWorkTimeSlot"
}-->

```json
{
  "end": "String (timestamp)",
  "start": "String (timestamp)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "bookingWorkTimeSlot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
