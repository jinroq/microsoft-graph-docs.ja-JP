---
title: searchwindowtimeslot リソースの種類
description: 期間。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 393e6a87f35f4ea6da5e7c4a4ccf37f52d90a8de
ms.sourcegitcommit: 539ed08adf3b7ad3253c98636d4ab303ce00176e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/15/2019
ms.locfileid: "30057402"
---
# <a name="searchwindowtimeslot-resource-type"></a><span data-ttu-id="2485e-103">searchwindowtimeslot リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2485e-103">searchWindowTimeSlot resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2485e-104">検索対象の期間。</span><span class="sxs-lookup"><span data-stu-id="2485e-104">A time period to search within.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2485e-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2485e-105">JSON representation</span></span>

<span data-ttu-id="2485e-106">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="2485e-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchWindowTimeSlot"
}-->

```json
{
  "end": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "start": {"@odata.type": "microsoft.graph.dateTimeTimeZone"}
}

```
## <a name="properties"></a><span data-ttu-id="2485e-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2485e-107">Properties</span></span>
| <span data-ttu-id="2485e-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2485e-108">Property</span></span>     | <span data-ttu-id="2485e-109">型</span><span class="sxs-lookup"><span data-stu-id="2485e-109">Type</span></span>   |<span data-ttu-id="2485e-110">説明</span><span class="sxs-lookup"><span data-stu-id="2485e-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2485e-111">end</span><span class="sxs-lookup"><span data-stu-id="2485e-111">end</span></span>|[<span data-ttu-id="2485e-112">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="2485e-112">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="2485e-113">期間が始まる日付、時刻、タイムゾーン。</span><span class="sxs-lookup"><span data-stu-id="2485e-113">The date, time, and time zone that a period begins.</span></span> |
|<span data-ttu-id="2485e-114">start</span><span class="sxs-lookup"><span data-stu-id="2485e-114">start</span></span>|[<span data-ttu-id="2485e-115">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="2485e-115">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="2485e-116">期間が終了する日付、時刻、タイムゾーン。</span><span class="sxs-lookup"><span data-stu-id="2485e-116">The date, time, and time zone that a period ends.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "searchWindowTimeSlot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/searchwindowtimeslot.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->