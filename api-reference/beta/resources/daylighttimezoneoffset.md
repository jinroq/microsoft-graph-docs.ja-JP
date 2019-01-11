---
title: daylightTimeZoneOffset リソースの種類
description: タイム ゾーンが標準時から夏時間に切り替わるタイミングを指定します。
localization_priority: Normal
ms.openlocfilehash: 37e08ec0e695fd245678510ac4a40bc978b1a93e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27825607"
---
# <a name="daylighttimezoneoffset-resource-type"></a><span data-ttu-id="386cf-103">daylightTimeZoneOffset リソースの種類</span><span class="sxs-lookup"><span data-stu-id="386cf-103">daylightTimeZoneOffset resource type</span></span>

> <span data-ttu-id="386cf-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="386cf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="386cf-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="386cf-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="386cf-106">タイム ゾーンが標準時から夏時間に切り替わるタイミングを指定します。</span><span class="sxs-lookup"><span data-stu-id="386cf-106">Specifies when a time zone switches from standard time to daylight saving time.</span></span>

<span data-ttu-id="386cf-107">たとえば、タイム ゾーンに次のプロパティが指定されているとします。</span><span class="sxs-lookup"><span data-stu-id="386cf-107">For example, if a time zone is specified with the following properties:</span></span>

- <span data-ttu-id="386cf-108">**bias**: 300</span><span class="sxs-lookup"><span data-stu-id="386cf-108">**bias** is 300</span></span>
- <span data-ttu-id="386cf-109">**daylightBias**: -100</span><span class="sxs-lookup"><span data-stu-id="386cf-109">**daylightBias** is -100</span></span>
- <span data-ttu-id="386cf-110">**dayOccurrence**: 4</span><span class="sxs-lookup"><span data-stu-id="386cf-110">**dayOccurrence** is 4</span></span>
- <span data-ttu-id="386cf-111">**dayOfWeek**: "日曜日"</span><span class="sxs-lookup"><span data-stu-id="386cf-111">**dayOfWeek** is "sunday"</span></span>
- <span data-ttu-id="386cf-112">**month**: 5</span><span class="sxs-lookup"><span data-stu-id="386cf-112">**month** is 5</span></span>
- <span data-ttu-id="386cf-113">**time** は 02:00:00 で、_ **year** は 0 です。つまり、夏時間の間は、時刻が UTC より +300-100=200 分進んでいることを意味します。</span><span class="sxs-lookup"><span data-stu-id="386cf-113">**time** is 02:00:00 _ **year** is 0 That means the time during daylight saving time is +300-100=200 minutes ahead of UTC.</span></span> <span data-ttu-id="386cf-114">夏時間から標準時への切り替えは、毎年 5 月の第 4 日曜日の午前 2 時に行われます。</span><span class="sxs-lookup"><span data-stu-id="386cf-114">The time zone transition from daylight saving time to standard occurs at 2 AM on the fourth Sunday of May, every year.</span></span>


## <a name="properties"></a><span data-ttu-id="386cf-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="386cf-115">Properties</span></span>
| <span data-ttu-id="386cf-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="386cf-116">Property</span></span>     | <span data-ttu-id="386cf-117">種類</span><span class="sxs-lookup"><span data-stu-id="386cf-117">Type</span></span>   |<span data-ttu-id="386cf-118">説明</span><span class="sxs-lookup"><span data-stu-id="386cf-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="386cf-119">daylightBias</span><span class="sxs-lookup"><span data-stu-id="386cf-119">daylightBias</span></span> | <span data-ttu-id="386cf-120">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="386cf-120">Edm.Int32</span></span> | <span data-ttu-id="386cf-121">夏時間の協定世界時 (UTC) からの時間オフセットです。</span><span class="sxs-lookup"><span data-stu-id="386cf-121">The time offset from Coordinated Universal Time (UTC) for daylight saving time.</span></span> <span data-ttu-id="386cf-122">この値は分単位です。</span><span class="sxs-lookup"><span data-stu-id="386cf-122">This value is in minutes.</span></span>  |
| <span data-ttu-id="386cf-123">dayOccurrence</span><span class="sxs-lookup"><span data-stu-id="386cf-123">dayOccurrence</span></span> | <span data-ttu-id="386cf-124">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="386cf-124">Edm.Int32</span></span> | <span data-ttu-id="386cf-125">標準時から夏時間への切り替えが月の何番目の曜日に行われるかを表します。</span><span class="sxs-lookup"><span data-stu-id="386cf-125">Represents the nth occurrence of the day of week that the transition from standard time to daylight saving time occurs.</span></span> |
| <span data-ttu-id="386cf-126">dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="386cf-126">dayOfWeek</span></span> | <span data-ttu-id="386cf-127">文字列</span><span class="sxs-lookup"><span data-stu-id="386cf-127">string</span></span> | <span data-ttu-id="386cf-128">標準時から夏時間への切り替えが行われる曜日を表します。</span><span class="sxs-lookup"><span data-stu-id="386cf-128">Represents the day of the week when the transition from standard time to daylight saving time occurs.</span></span> |
| <span data-ttu-id="386cf-129">month</span><span class="sxs-lookup"><span data-stu-id="386cf-129">month</span></span> | <span data-ttu-id="386cf-130">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="386cf-130">Edm.Int32</span></span> | <span data-ttu-id="386cf-131">標準時から夏時間への切り替えが行われる月を表します。</span><span class="sxs-lookup"><span data-stu-id="386cf-131">Represents the month of the year when the transition from standard time to daylight saving time occurs.</span></span> |
| <span data-ttu-id="386cf-132">time</span><span class="sxs-lookup"><span data-stu-id="386cf-132">time</span></span> | <span data-ttu-id="386cf-133">Edm.TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="386cf-133">Edm.TimeOfDay</span></span> | <span data-ttu-id="386cf-134">標準時から夏時間への切り替えが行われる時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="386cf-134">Represents the time of day when the transition from standard time to daylight saving time occurs.</span></span> |
| <span data-ttu-id="386cf-135">year</span><span class="sxs-lookup"><span data-stu-id="386cf-135">year</span></span> | <span data-ttu-id="386cf-136">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="386cf-136">Edm.Int32</span></span> | <span data-ttu-id="386cf-137">標準時から夏時間への切り替えが年に何回行われるかを表します。</span><span class="sxs-lookup"><span data-stu-id="386cf-137">Represents how frequently in terms of years the change from standard time to daylight saving time occurs.</span></span> <span data-ttu-id="386cf-138">たとえば、値 0 は年に 1 回を意味します。</span><span class="sxs-lookup"><span data-stu-id="386cf-138">For example, a value of 0 means every year.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="386cf-139">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="386cf-139">JSON representation</span></span>

<span data-ttu-id="386cf-140">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="386cf-140">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "daylightTimeZoneOffset resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
