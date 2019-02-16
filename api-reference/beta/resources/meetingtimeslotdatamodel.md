---
title: meetingTimeSlotDataModel リソースの種類
description: 期間。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: acbd08da5e15dd733c63c0141db5b58cee896666
ms.sourcegitcommit: 539ed08adf3b7ad3253c98636d4ab303ce00176e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/15/2019
ms.locfileid: "30057396"
---
# <a name="meetingtimeslotdatamodel-resource-type"></a><span data-ttu-id="6ee86-103">meetingTimeSlotDataModel リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6ee86-103">meetingTimeSlotDataModel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6ee86-104">会議の時間帯を表します。</span><span class="sxs-lookup"><span data-stu-id="6ee86-104">Represents a time slot for a meeting.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6ee86-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6ee86-105">JSON representation</span></span>

<span data-ttu-id="6ee86-106">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="6ee86-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingTimeSlotDataModel"
}-->

```json
{
  "end": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "start": {"@odata.type": "microsoft.graph.dateTimeTimeZone"}
}

```
## <a name="properties"></a><span data-ttu-id="6ee86-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6ee86-107">Properties</span></span>
| <span data-ttu-id="6ee86-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6ee86-108">Property</span></span>     | <span data-ttu-id="6ee86-109">型</span><span class="sxs-lookup"><span data-stu-id="6ee86-109">Type</span></span>   |<span data-ttu-id="6ee86-110">説明</span><span class="sxs-lookup"><span data-stu-id="6ee86-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6ee86-111">end</span><span class="sxs-lookup"><span data-stu-id="6ee86-111">end</span></span>|[<span data-ttu-id="6ee86-112">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="6ee86-112">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="6ee86-113">期間が始まる日付、時刻、タイムゾーン。</span><span class="sxs-lookup"><span data-stu-id="6ee86-113">The date, time, and time zone that a period begins.</span></span> |
|<span data-ttu-id="6ee86-114">start</span><span class="sxs-lookup"><span data-stu-id="6ee86-114">start</span></span>|[<span data-ttu-id="6ee86-115">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="6ee86-115">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="6ee86-116">期間が終了する日付、時刻、タイムゾーン。</span><span class="sxs-lookup"><span data-stu-id="6ee86-116">The date, time, and time zone that a period ends.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "meetingTimeSlotDataModel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/meetingtimeslotdatamodel.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->