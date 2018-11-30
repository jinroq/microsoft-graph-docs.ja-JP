---
title: bookingWorkTimeSlot リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。"
ms.openlocfilehash: 61436ca3e94ab15c44fc1898827a3de511c8ee94
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069418"
---
# <a name="bookingworktimeslot-resource-type"></a><span data-ttu-id="e761b-104">bookingWorkTimeSlot リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e761b-104">bookingWorkTimeSlot resource type</span></span>

 > <span data-ttu-id="e761b-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e761b-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e761b-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e761b-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="e761b-107">作業の開始と終了時間です。</span><span class="sxs-lookup"><span data-stu-id="e761b-107">The start and end times for work.</span></span>


## <a name="properties"></a><span data-ttu-id="e761b-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e761b-108">Properties</span></span>
| <span data-ttu-id="e761b-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e761b-109">Property</span></span>     | <span data-ttu-id="e761b-110">型</span><span class="sxs-lookup"><span data-stu-id="e761b-110">Type</span></span>   |<span data-ttu-id="e761b-111">説明</span><span class="sxs-lookup"><span data-stu-id="e761b-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e761b-112">end</span><span class="sxs-lookup"><span data-stu-id="e761b-112">end</span></span>|<span data-ttu-id="e761b-113">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="e761b-113">TimeOfDay</span></span>|<span data-ttu-id="e761b-114">起動時に動作する 1 日の時間。</span><span class="sxs-lookup"><span data-stu-id="e761b-114">The time of the day that work starts.</span></span> <span data-ttu-id="e761b-115">たとえば、08:00:00.0000000 です。</span><span class="sxs-lookup"><span data-stu-id="e761b-115">For example, 08:00:00.0000000.</span></span>|
|<span data-ttu-id="e761b-116">開始</span><span class="sxs-lookup"><span data-stu-id="e761b-116">start</span></span>|<span data-ttu-id="e761b-117">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="e761b-117">TimeOfDay</span></span>|<span data-ttu-id="e761b-118">1 日の時間が停止するを作業です。</span><span class="sxs-lookup"><span data-stu-id="e761b-118">The time of the day that work stops.</span></span> <span data-ttu-id="e761b-119">たとえば、17:00:00.0000000 です。</span><span class="sxs-lookup"><span data-stu-id="e761b-119">For example, 17:00:00.0000000.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e761b-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e761b-120">JSON representation</span></span>

<span data-ttu-id="e761b-121">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e761b-121">The following is a JSON representation of the resource.</span></span>

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