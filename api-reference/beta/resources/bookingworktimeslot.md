---
title: bookingwork timesロットリソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: a193843617d5acc7e18d8a06993a1629b80762be
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543713"
---
# <a name="bookingworktimeslot-resource-type"></a><span data-ttu-id="40b64-104">bookingwork timesロットリソースの種類</span><span class="sxs-lookup"><span data-stu-id="40b64-104">bookingWorkTimeSlot resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="40b64-105">作業の開始時刻と終了時刻。</span><span class="sxs-lookup"><span data-stu-id="40b64-105">The start and end times for work.</span></span>


## <a name="properties"></a><span data-ttu-id="40b64-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="40b64-106">Properties</span></span>
| <span data-ttu-id="40b64-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="40b64-107">Property</span></span>     | <span data-ttu-id="40b64-108">型</span><span class="sxs-lookup"><span data-stu-id="40b64-108">Type</span></span>   |<span data-ttu-id="40b64-109">説明</span><span class="sxs-lookup"><span data-stu-id="40b64-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="40b64-110">end</span><span class="sxs-lookup"><span data-stu-id="40b64-110">end</span></span>|<span data-ttu-id="40b64-111">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="40b64-111">TimeOfDay</span></span>|<span data-ttu-id="40b64-112">作業を開始する時刻。</span><span class="sxs-lookup"><span data-stu-id="40b64-112">The time of the day that work starts.</span></span> <span data-ttu-id="40b64-113">たとえば、08:00: 00.0000000 のようになります。</span><span class="sxs-lookup"><span data-stu-id="40b64-113">For example, 08:00:00.0000000.</span></span>|
|<span data-ttu-id="40b64-114">開始</span><span class="sxs-lookup"><span data-stu-id="40b64-114">start</span></span>|<span data-ttu-id="40b64-115">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="40b64-115">TimeOfDay</span></span>|<span data-ttu-id="40b64-116">作業が停止する時間。</span><span class="sxs-lookup"><span data-stu-id="40b64-116">The time of the day that work stops.</span></span> <span data-ttu-id="40b64-117">たとえば、17:00: 00.0000000 となります。</span><span class="sxs-lookup"><span data-stu-id="40b64-117">For example, 17:00:00.0000000.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="40b64-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="40b64-118">JSON representation</span></span>

<span data-ttu-id="40b64-119">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="40b64-119">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/bookingworktimeslot.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
