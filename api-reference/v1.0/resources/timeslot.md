---
title: timeSlot リソースの種類
description: 期間です。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 5dbde12e63a5e48863f1353f4d4d22df5ba41091
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033594"
---
# <a name="timeslot-resource-type"></a><span data-ttu-id="31e1b-103">timeSlot リソースの種類</span><span class="sxs-lookup"><span data-stu-id="31e1b-103">timeSlot resource type</span></span>

<span data-ttu-id="31e1b-104">会議の時間帯を表します。</span><span class="sxs-lookup"><span data-stu-id="31e1b-104">Represents a time slot for a meeting.</span></span>

## <a name="json-representation"></a><span data-ttu-id="31e1b-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="31e1b-105">JSON representation</span></span>

<span data-ttu-id="31e1b-106">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="31e1b-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="31e1b-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="31e1b-107">Properties</span></span>
| <span data-ttu-id="31e1b-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="31e1b-108">Property</span></span>     | <span data-ttu-id="31e1b-109">型</span><span class="sxs-lookup"><span data-stu-id="31e1b-109">Type</span></span>   |<span data-ttu-id="31e1b-110">説明</span><span class="sxs-lookup"><span data-stu-id="31e1b-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="31e1b-111">end</span><span class="sxs-lookup"><span data-stu-id="31e1b-111">end</span></span>|[<span data-ttu-id="31e1b-112">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="31e1b-112">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="31e1b-113">期間が始まる日付、時刻、タイムゾーン。</span><span class="sxs-lookup"><span data-stu-id="31e1b-113">The date, time, and time zone that a period begins.</span></span> |
|<span data-ttu-id="31e1b-114">開始</span><span class="sxs-lookup"><span data-stu-id="31e1b-114">start</span></span>|[<span data-ttu-id="31e1b-115">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="31e1b-115">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="31e1b-116">期間が終了する日付、時刻、タイムゾーン。</span><span class="sxs-lookup"><span data-stu-id="31e1b-116">The date, time, and time zone that a period ends.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeSlot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
