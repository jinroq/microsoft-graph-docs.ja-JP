---
title: timeSlot リソースの種類
description: 期間です。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 7b09ae7f1c60a8348e9f22b856c65f326432e408
ms.sourcegitcommit: a90abf5b89dbbdfefb1b7794d1f12c6e2bfb0cda
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/28/2019
ms.locfileid: "30936242"
---
# <a name="timeslot-resource-type"></a><span data-ttu-id="9d4fe-103">timeSlot リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9d4fe-103">timeSlot resource type</span></span>

<span data-ttu-id="9d4fe-104">会議の時間帯を表します。</span><span class="sxs-lookup"><span data-stu-id="9d4fe-104">Represents a time slot for a meeting.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9d4fe-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9d4fe-105">JSON representation</span></span>

<span data-ttu-id="9d4fe-106">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="9d4fe-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeSlot"
}-->

```json
{
  "end": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "start": {"@odata.type": "microsoft.graph.dateTimeTimeZone"}
}

```
## <a name="properties"></a><span data-ttu-id="9d4fe-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9d4fe-107">Properties</span></span>
| <span data-ttu-id="9d4fe-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9d4fe-108">Property</span></span>     | <span data-ttu-id="9d4fe-109">型</span><span class="sxs-lookup"><span data-stu-id="9d4fe-109">Type</span></span>   |<span data-ttu-id="9d4fe-110">説明</span><span class="sxs-lookup"><span data-stu-id="9d4fe-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9d4fe-111">end</span><span class="sxs-lookup"><span data-stu-id="9d4fe-111">end</span></span>|[<span data-ttu-id="9d4fe-112">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="9d4fe-112">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="9d4fe-113">期間が始まる日付、時刻、タイムゾーン。</span><span class="sxs-lookup"><span data-stu-id="9d4fe-113">The date, time, and time zone that a period begins.</span></span> |
|<span data-ttu-id="9d4fe-114">start</span><span class="sxs-lookup"><span data-stu-id="9d4fe-114">start</span></span>|[<span data-ttu-id="9d4fe-115">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="9d4fe-115">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="9d4fe-116">期間が終了する日付、時刻、タイムゾーン。</span><span class="sxs-lookup"><span data-stu-id="9d4fe-116">The date, time, and time zone that a period ends.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeSlot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
