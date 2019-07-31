---
title: timeSlot リソースの種類
description: 期間です。
localization_priority: Normal
doc_type: resourcePageType
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 8843b8418bff068564e5716d715a9ad11579f01b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007537"
---
# <a name="timeslot-resource-type"></a><span data-ttu-id="d35a2-103">timeSlot リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d35a2-103">timeSlot resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d35a2-104">会議の時間帯を表します。</span><span class="sxs-lookup"><span data-stu-id="d35a2-104">Represents a time slot for a meeting.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d35a2-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d35a2-105">JSON representation</span></span>

<span data-ttu-id="d35a2-106">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="d35a2-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="d35a2-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d35a2-107">Properties</span></span>
| <span data-ttu-id="d35a2-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d35a2-108">Property</span></span>     | <span data-ttu-id="d35a2-109">型</span><span class="sxs-lookup"><span data-stu-id="d35a2-109">Type</span></span>   |<span data-ttu-id="d35a2-110">説明</span><span class="sxs-lookup"><span data-stu-id="d35a2-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d35a2-111">end</span><span class="sxs-lookup"><span data-stu-id="d35a2-111">end</span></span>|[<span data-ttu-id="d35a2-112">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="d35a2-112">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="d35a2-113">期間が始まる日付、時刻、タイムゾーン。</span><span class="sxs-lookup"><span data-stu-id="d35a2-113">The date, time, and time zone that a period begins.</span></span> |
|<span data-ttu-id="d35a2-114">開始</span><span class="sxs-lookup"><span data-stu-id="d35a2-114">start</span></span>|[<span data-ttu-id="d35a2-115">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="d35a2-115">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="d35a2-116">期間が終了する日付、時刻、タイムゾーン。</span><span class="sxs-lookup"><span data-stu-id="d35a2-116">The date, time, and time zone that a period ends.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeSlot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
