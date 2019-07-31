---
title: standardTimeZoneOffset リソースの種類
description: タイム ゾーンが夏時間から標準時に切り替わるタイミングを指定します。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 545ed2aed08be31aad09e33d8db7e0bd669bfcb8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008097"
---
# <a name="standardtimezoneoffset-resource-type"></a><span data-ttu-id="6603c-103">standardTimeZoneOffset リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6603c-103">standardTimeZoneOffset resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6603c-104">タイム ゾーンが夏時間から標準時に切り替わるタイミングを指定します。</span><span class="sxs-lookup"><span data-stu-id="6603c-104">Specifies when a time zone switches from daylight saving time to standard time.</span></span>

<span data-ttu-id="6603c-105">たとえば、タイム ゾーンに次のプロパティが指定されているとします。</span><span class="sxs-lookup"><span data-stu-id="6603c-105">For example, if a time zone is specified with the following properties:</span></span>

- <span data-ttu-id="6603c-106">**dayOccurrence**: 3</span><span class="sxs-lookup"><span data-stu-id="6603c-106">**dayOccurrence** is 3</span></span>
- <span data-ttu-id="6603c-107">**dayOfWeek**: "日曜日"</span><span class="sxs-lookup"><span data-stu-id="6603c-107">**dayOfWeek** is "Sunday"</span></span>
- <span data-ttu-id="6603c-108">**month**: 10</span><span class="sxs-lookup"><span data-stu-id="6603c-108">**month** is 10</span></span>
- <span data-ttu-id="6603c-109">**time** は 02:00:00 で、_ **year** は 0 です。つまり、夏時間から標準時への切り替えは、毎年 10 月の第 3 日曜日の午前 2 時に行われることを意味します。</span><span class="sxs-lookup"><span data-stu-id="6603c-109">**time** is 02:00:00 _ **year** is 0 That means the transition from daylight saving time to standard occurs at 2 AM on the third Sunday of October, every year.</span></span>

## <a name="properties"></a><span data-ttu-id="6603c-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6603c-110">Properties</span></span>
| <span data-ttu-id="6603c-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6603c-111">Property</span></span>     | <span data-ttu-id="6603c-112">型</span><span class="sxs-lookup"><span data-stu-id="6603c-112">Type</span></span>   |<span data-ttu-id="6603c-113">説明</span><span class="sxs-lookup"><span data-stu-id="6603c-113">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6603c-114">dayOccurrence</span><span class="sxs-lookup"><span data-stu-id="6603c-114">dayOccurrence</span></span> | <span data-ttu-id="6603c-115">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="6603c-115">Edm.Int32</span></span> | <span data-ttu-id="6603c-116">夏時間から標準時への切り替えが月の何番目の曜日に行われるかを表します。</span><span class="sxs-lookup"><span data-stu-id="6603c-116">Represents the nth occurrence of the day of week that the transition from daylight saving time to standard time occurs.</span></span> |
| <span data-ttu-id="6603c-117">dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="6603c-117">dayOfWeek</span></span> | <span data-ttu-id="6603c-118">string</span><span class="sxs-lookup"><span data-stu-id="6603c-118">string</span></span> | <span data-ttu-id="6603c-119">夏時間から標準時への切り替えが行われる曜日を表します。</span><span class="sxs-lookup"><span data-stu-id="6603c-119">Represents the day of the week when the transition from daylight saving time to standard time.</span></span> |
| <span data-ttu-id="6603c-120">month</span><span class="sxs-lookup"><span data-stu-id="6603c-120">month</span></span> | <span data-ttu-id="6603c-121">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="6603c-121">Edm.Int32</span></span> | <span data-ttu-id="6603c-122">夏時間から標準時への切り替えが行われる月を表します。</span><span class="sxs-lookup"><span data-stu-id="6603c-122">Represents the month of the year when the transition from daylight saving time to standard time occurs.</span></span> |
| <span data-ttu-id="6603c-123">time</span><span class="sxs-lookup"><span data-stu-id="6603c-123">time</span></span> | <span data-ttu-id="6603c-124">Edm.TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="6603c-124">Edm.TimeOfDay</span></span> | <span data-ttu-id="6603c-125">夏時間から標準時への切り替えが行われる時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="6603c-125">Represents the time of day when the transition from daylight saving time to standard time occurs.</span></span> |
| <span data-ttu-id="6603c-126">year</span><span class="sxs-lookup"><span data-stu-id="6603c-126">year</span></span> | <span data-ttu-id="6603c-127">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="6603c-127">Edm.Int32</span></span> | <span data-ttu-id="6603c-128">夏時間から標準時への切り替えが年に何回行われるかを表します。</span><span class="sxs-lookup"><span data-stu-id="6603c-128">Represents how frequently in terms of years the change from daylight saving time to standard time occurs.</span></span> <span data-ttu-id="6603c-129">たとえば、値 0 は年に 1 回を意味します。</span><span class="sxs-lookup"><span data-stu-id="6603c-129">For example, a value of 0 means every year.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="6603c-130">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6603c-130">JSON representation</span></span>

<span data-ttu-id="6603c-131">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6603c-131">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "standardTimeZoneOffset resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
