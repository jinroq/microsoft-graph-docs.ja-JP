---
title: daylightTimeZoneOffset リソースの種類
description: タイム ゾーンが標準時から夏時間に切り替わるタイミングを指定します。
localization_priority: Normal
ms.openlocfilehash: 160163d6f574eb75746fa751e383c06696006e43
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29507587"
---
# <a name="daylighttimezoneoffset-resource-type"></a><span data-ttu-id="6aa77-103">daylightTimeZoneOffset リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6aa77-103">daylightTimeZoneOffset resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6aa77-104">タイム ゾーンが標準時から夏時間に切り替わるタイミングを指定します。</span><span class="sxs-lookup"><span data-stu-id="6aa77-104">Specifies when a time zone switches from standard time to daylight saving time.</span></span>

<span data-ttu-id="6aa77-105">たとえば、タイム ゾーンに次のプロパティが指定されているとします。</span><span class="sxs-lookup"><span data-stu-id="6aa77-105">For example, if a time zone is specified with the following properties:</span></span>

- <span data-ttu-id="6aa77-106">**bias**: 300</span><span class="sxs-lookup"><span data-stu-id="6aa77-106">**bias** is 300</span></span>
- <span data-ttu-id="6aa77-107">**daylightBias**: -100</span><span class="sxs-lookup"><span data-stu-id="6aa77-107">**daylightBias** is -100</span></span>
- <span data-ttu-id="6aa77-108">**dayOccurrence**: 4</span><span class="sxs-lookup"><span data-stu-id="6aa77-108">**dayOccurrence** is 4</span></span>
- <span data-ttu-id="6aa77-109">**dayOfWeek**: "日曜日"</span><span class="sxs-lookup"><span data-stu-id="6aa77-109">**dayOfWeek** is "sunday"</span></span>
- <span data-ttu-id="6aa77-110">**month**: 5</span><span class="sxs-lookup"><span data-stu-id="6aa77-110">**month** is 5</span></span>
- <span data-ttu-id="6aa77-111">**time** は 02:00:00 で、_ **year** は 0 です。つまり、夏時間の間は、時刻が UTC より +300-100=200 分進んでいることを意味します。</span><span class="sxs-lookup"><span data-stu-id="6aa77-111">**time** is 02:00:00 _ **year** is 0 That means the time during daylight saving time is +300-100=200 minutes ahead of UTC.</span></span> <span data-ttu-id="6aa77-112">夏時間から標準時への切り替えは、毎年 5 月の第 4 日曜日の午前 2 時に行われます。</span><span class="sxs-lookup"><span data-stu-id="6aa77-112">The time zone transition from daylight saving time to standard occurs at 2 AM on the fourth Sunday of May, every year.</span></span>


## <a name="properties"></a><span data-ttu-id="6aa77-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6aa77-113">Properties</span></span>
| <span data-ttu-id="6aa77-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6aa77-114">Property</span></span>     | <span data-ttu-id="6aa77-115">型</span><span class="sxs-lookup"><span data-stu-id="6aa77-115">Type</span></span>   |<span data-ttu-id="6aa77-116">説明</span><span class="sxs-lookup"><span data-stu-id="6aa77-116">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6aa77-117">daylightBias</span><span class="sxs-lookup"><span data-stu-id="6aa77-117">daylightBias</span></span> | <span data-ttu-id="6aa77-118">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="6aa77-118">Edm.Int32</span></span> | <span data-ttu-id="6aa77-119">夏時間の協定世界時 (UTC) からの時間オフセットです。</span><span class="sxs-lookup"><span data-stu-id="6aa77-119">The time offset from Coordinated Universal Time (UTC) for daylight saving time.</span></span> <span data-ttu-id="6aa77-120">この値は分単位です。</span><span class="sxs-lookup"><span data-stu-id="6aa77-120">This value is in minutes.</span></span>  |
| <span data-ttu-id="6aa77-121">dayOccurrence</span><span class="sxs-lookup"><span data-stu-id="6aa77-121">dayOccurrence</span></span> | <span data-ttu-id="6aa77-122">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="6aa77-122">Edm.Int32</span></span> | <span data-ttu-id="6aa77-123">標準時から夏時間への切り替えが月の何番目の曜日に行われるかを表します。</span><span class="sxs-lookup"><span data-stu-id="6aa77-123">Represents the nth occurrence of the day of week that the transition from standard time to daylight saving time occurs.</span></span> |
| <span data-ttu-id="6aa77-124">dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="6aa77-124">dayOfWeek</span></span> | <span data-ttu-id="6aa77-125">string</span><span class="sxs-lookup"><span data-stu-id="6aa77-125">string</span></span> | <span data-ttu-id="6aa77-126">標準時から夏時間への切り替えが行われる曜日を表します。</span><span class="sxs-lookup"><span data-stu-id="6aa77-126">Represents the day of the week when the transition from standard time to daylight saving time occurs.</span></span> |
| <span data-ttu-id="6aa77-127">month</span><span class="sxs-lookup"><span data-stu-id="6aa77-127">month</span></span> | <span data-ttu-id="6aa77-128">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="6aa77-128">Edm.Int32</span></span> | <span data-ttu-id="6aa77-129">標準時から夏時間への切り替えが行われる月を表します。</span><span class="sxs-lookup"><span data-stu-id="6aa77-129">Represents the month of the year when the transition from standard time to daylight saving time occurs.</span></span> |
| <span data-ttu-id="6aa77-130">time</span><span class="sxs-lookup"><span data-stu-id="6aa77-130">time</span></span> | <span data-ttu-id="6aa77-131">Edm.TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="6aa77-131">Edm.TimeOfDay</span></span> | <span data-ttu-id="6aa77-132">標準時から夏時間への切り替えが行われる時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="6aa77-132">Represents the time of day when the transition from standard time to daylight saving time occurs.</span></span> |
| <span data-ttu-id="6aa77-133">year</span><span class="sxs-lookup"><span data-stu-id="6aa77-133">year</span></span> | <span data-ttu-id="6aa77-134">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="6aa77-134">Edm.Int32</span></span> | <span data-ttu-id="6aa77-135">標準時から夏時間への切り替えが年に何回行われるかを表します。</span><span class="sxs-lookup"><span data-stu-id="6aa77-135">Represents how frequently in terms of years the change from standard time to daylight saving time occurs.</span></span> <span data-ttu-id="6aa77-136">たとえば、値 0 は年に 1 回を意味します。</span><span class="sxs-lookup"><span data-stu-id="6aa77-136">For example, a value of 0 means every year.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="6aa77-137">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6aa77-137">JSON representation</span></span>

<span data-ttu-id="6aa77-138">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6aa77-138">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.daylightTimeZoneOffset"
}-->

```json
{
  "daylightBias": "Int32",
  "dayOccurrence": "Int32",
  "dayOfWeek": "string",
  "month": "Int32",
  "time": "TimeOfDay",
  "year": "Int32"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "daylightTimeZoneOffset resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/daylighttimezoneoffset.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
