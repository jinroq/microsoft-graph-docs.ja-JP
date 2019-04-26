---
title: bookingwork timesロットリソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでは、これらの API の使用はサポートされていません。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: a6063b8ee5c1c40476f676c3a9846fa7d7aab421
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33338803"
---
# <a name="bookingworktimeslot-resource-type"></a><span data-ttu-id="f85ea-104">bookingwork timesロットリソースの種類</span><span class="sxs-lookup"><span data-stu-id="f85ea-104">bookingWorkTimeSlot resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="f85ea-105">作業の開始時刻と終了時刻。</span><span class="sxs-lookup"><span data-stu-id="f85ea-105">The start and end times for work.</span></span>


## <a name="properties"></a><span data-ttu-id="f85ea-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f85ea-106">Properties</span></span>
| <span data-ttu-id="f85ea-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f85ea-107">Property</span></span>     | <span data-ttu-id="f85ea-108">型</span><span class="sxs-lookup"><span data-stu-id="f85ea-108">Type</span></span>   |<span data-ttu-id="f85ea-109">説明</span><span class="sxs-lookup"><span data-stu-id="f85ea-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f85ea-110">end</span><span class="sxs-lookup"><span data-stu-id="f85ea-110">end</span></span>|<span data-ttu-id="f85ea-111">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="f85ea-111">TimeOfDay</span></span>|<span data-ttu-id="f85ea-112">作業を開始する時刻。</span><span class="sxs-lookup"><span data-stu-id="f85ea-112">The time of the day that work starts.</span></span> <span data-ttu-id="f85ea-113">たとえば、08:00: 00.0000000 のようになります。</span><span class="sxs-lookup"><span data-stu-id="f85ea-113">For example, 08:00:00.0000000.</span></span>|
|<span data-ttu-id="f85ea-114">開始</span><span class="sxs-lookup"><span data-stu-id="f85ea-114">start</span></span>|<span data-ttu-id="f85ea-115">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="f85ea-115">TimeOfDay</span></span>|<span data-ttu-id="f85ea-116">作業が停止する時間。</span><span class="sxs-lookup"><span data-stu-id="f85ea-116">The time of the day that work stops.</span></span> <span data-ttu-id="f85ea-117">たとえば、17:00: 00.0000000 となります。</span><span class="sxs-lookup"><span data-stu-id="f85ea-117">For example, 17:00:00.0000000.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f85ea-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f85ea-118">JSON representation</span></span>

<span data-ttu-id="f85ea-119">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f85ea-119">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "bookingWorkTimeSlot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
