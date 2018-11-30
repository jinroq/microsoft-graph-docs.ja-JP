---
title: standardTimeZoneOffset リソースの種類
description: タイム ゾーンが夏時間から標準時に切り替わるタイミングを指定します。
ms.openlocfilehash: 167ff45f4ccf1615c1560c3f2ba130cdc7747043
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069824"
---
# <a name="standardtimezoneoffset-resource-type"></a><span data-ttu-id="1f096-103">standardTimeZoneOffset リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1f096-103">standardTimeZoneOffset resource type</span></span>

> <span data-ttu-id="1f096-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1f096-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1f096-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1f096-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1f096-106">タイム ゾーンが夏時間から標準時に切り替わるタイミングを指定します。</span><span class="sxs-lookup"><span data-stu-id="1f096-106">Specifies when a time zone switches from daylight saving time to standard time.</span></span>

<span data-ttu-id="1f096-107">たとえば、タイム ゾーンに次のプロパティが指定されているとします。</span><span class="sxs-lookup"><span data-stu-id="1f096-107">For example, if a time zone is specified with the following properties:</span></span>

- <span data-ttu-id="1f096-108">**dayOccurrence**: 3</span><span class="sxs-lookup"><span data-stu-id="1f096-108">**dayOccurrence** is 3</span></span>
- <span data-ttu-id="1f096-109">**dayOfWeek**: "日曜日"</span><span class="sxs-lookup"><span data-stu-id="1f096-109">**dayOfWeek** is "Sunday"</span></span>
- <span data-ttu-id="1f096-110">**month**: 10</span><span class="sxs-lookup"><span data-stu-id="1f096-110">**month** is 10</span></span>
- <span data-ttu-id="1f096-111">**time** は 02:00:00 で、_ **year** は 0 です。つまり、夏時間から標準時への切り替えは、毎年 10 月の第 3 日曜日の午前 2 時に行われることを意味します。</span><span class="sxs-lookup"><span data-stu-id="1f096-111">**time** is 02:00:00 _ **year** is 0 That means the transition from daylight saving time to standard occurs at 2 AM on the third Sunday of October, every year.</span></span>

## <a name="properties"></a><span data-ttu-id="1f096-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1f096-112">Properties</span></span>
| <span data-ttu-id="1f096-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1f096-113">Property</span></span>     | <span data-ttu-id="1f096-114">型</span><span class="sxs-lookup"><span data-stu-id="1f096-114">Type</span></span>   |<span data-ttu-id="1f096-115">説明</span><span class="sxs-lookup"><span data-stu-id="1f096-115">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1f096-116">dayOccurrence</span><span class="sxs-lookup"><span data-stu-id="1f096-116">dayOccurrence</span></span> | <span data-ttu-id="1f096-117">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="1f096-117">Edm.Int32</span></span> | <span data-ttu-id="1f096-118">夏時間から標準時への切り替えが月の何番目の曜日に行われるかを表します。</span><span class="sxs-lookup"><span data-stu-id="1f096-118">Represents the nth occurrence of the day of week that the transition from daylight saving time to standard time occurs.</span></span> |
| <span data-ttu-id="1f096-119">dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="1f096-119">dayOfWeek</span></span> | <span data-ttu-id="1f096-120">文字列</span><span class="sxs-lookup"><span data-stu-id="1f096-120">string</span></span> | <span data-ttu-id="1f096-121">夏時間から標準時への切り替えが行われる曜日を表します。</span><span class="sxs-lookup"><span data-stu-id="1f096-121">Represents the day of the week when the transition from daylight saving time to standard time.</span></span> |
| <span data-ttu-id="1f096-122">month</span><span class="sxs-lookup"><span data-stu-id="1f096-122">month</span></span> | <span data-ttu-id="1f096-123">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="1f096-123">Edm.Int32</span></span> | <span data-ttu-id="1f096-124">夏時間から標準時への切り替えが行われる月を表します。</span><span class="sxs-lookup"><span data-stu-id="1f096-124">Represents the month of the year when the transition from daylight saving time to standard time occurs.</span></span> |
| <span data-ttu-id="1f096-125">time</span><span class="sxs-lookup"><span data-stu-id="1f096-125">time</span></span> | <span data-ttu-id="1f096-126">Edm.TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="1f096-126">Edm.TimeOfDay</span></span> | <span data-ttu-id="1f096-127">夏時間から標準時への切り替えが行われる時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="1f096-127">Represents the time of day when the transition from daylight saving time to standard time occurs.</span></span> |
| <span data-ttu-id="1f096-128">year</span><span class="sxs-lookup"><span data-stu-id="1f096-128">year</span></span> | <span data-ttu-id="1f096-129">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="1f096-129">Edm.Int32</span></span> | <span data-ttu-id="1f096-130">夏時間から標準時への切り替えが年に何回行われるかを表します。</span><span class="sxs-lookup"><span data-stu-id="1f096-130">Represents how frequently in terms of years the change from daylight saving time to standard time occurs.</span></span> <span data-ttu-id="1f096-131">たとえば、値 0 は年に 1 回を意味します。</span><span class="sxs-lookup"><span data-stu-id="1f096-131">For example, a value of 0 means every year.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="1f096-132">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1f096-132">JSON representation</span></span>

<span data-ttu-id="1f096-133">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1f096-133">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.standardTimeZoneOffset"
}-->

```json
{
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
  "description": "standardTimeZoneOffset resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->