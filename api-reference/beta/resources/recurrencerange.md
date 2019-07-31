---
title: recurrenceRange リソースの種類
description: '定期的なイベントを繰り返す期間について説明します。 '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: e3fba30268b2b0a6746e3bb116fc29c610a6d311
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965468"
---
# <a name="recurrencerange-resource-type"></a><span data-ttu-id="208eb-103">recurrenceRange リソースの種類</span><span class="sxs-lookup"><span data-stu-id="208eb-103">recurrenceRange resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="208eb-104">定期的な[イベント](event.md)を繰り返す期間について説明します。</span><span class="sxs-lookup"><span data-stu-id="208eb-104">Describes a date range over which a recurring [event](event.md) repeats.</span></span> 

<span data-ttu-id="208eb-105">シナリオに応じて、定期的なイベントの 3 通りの期間のいずれかを指定できます。</span><span class="sxs-lookup"><span data-stu-id="208eb-105">You can specify the date range for a recurring event in one of 3 ways depending on your scenario.</span></span> <span data-ttu-id="208eb-106">期間の **startDate** 値は必ず指定する必要がありますが、定期的なイベントの終了は、特定の日付までに終了する、終了しない、または特定の回数繰り返した後に終了する、など指定することができます。</span><span class="sxs-lookup"><span data-stu-id="208eb-106">While you must always specify a **startDate** value for the date range, you can specify a recurring event that ends by a specific date, or that doesn't end, or that ends after a specific number of occurrences.</span></span> <span data-ttu-id="208eb-107">イベントに対して指定した期間内の定期的なイベントは、必ずこの定期的なパターンに従って発生します。</span><span class="sxs-lookup"><span data-stu-id="208eb-107">Note that the actual occurrences within the date range always follow the recurrence pattern that you specify for the recurring event.</span></span> <span data-ttu-id="208eb-108">定期的なイベントは常に、[recurrencePattern](recurrencepattern.md) (イベントを繰り返す頻度)、および **recurrenceRange** (イベントを繰り返す期間) によって定義されます。</span><span class="sxs-lookup"><span data-stu-id="208eb-108">A recurring event is always defined by its [recurrencePattern](recurrencepattern.md) (how frequently the event repeats), and its **recurrenceRange** (for how long the event repeats).</span></span>


## <a name="properties"></a><span data-ttu-id="208eb-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="208eb-109">Properties</span></span>

| <span data-ttu-id="208eb-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="208eb-110">Property</span></span>     | <span data-ttu-id="208eb-111">型</span><span class="sxs-lookup"><span data-stu-id="208eb-111">Type</span></span>   |<span data-ttu-id="208eb-112">説明</span><span class="sxs-lookup"><span data-stu-id="208eb-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="208eb-113">endDate</span><span class="sxs-lookup"><span data-stu-id="208eb-113">endDate</span></span>|<span data-ttu-id="208eb-114">日付</span><span class="sxs-lookup"><span data-stu-id="208eb-114">Date</span></span>|<span data-ttu-id="208eb-115">定期的なパターンの適用を停止する日付。</span><span class="sxs-lookup"><span data-stu-id="208eb-115">The date to stop applying the recurrence pattern.</span></span> <span data-ttu-id="208eb-116">イベントの定期的なパターンによっては、最後に会議が発生するのは、この日付にならない可能性があります。</span><span class="sxs-lookup"><span data-stu-id="208eb-116">Depending on the recurrence pattern of the event, the last occurrence of the meeting may not be this date.</span></span> <span data-ttu-id="208eb-117">**type** が `endDate` の場合、必要です。</span><span class="sxs-lookup"><span data-stu-id="208eb-117">Required if **type** is `endDate`.</span></span>|
|<span data-ttu-id="208eb-118">numberOfOccurrences</span><span class="sxs-lookup"><span data-stu-id="208eb-118">numberOfOccurrences</span></span>|<span data-ttu-id="208eb-119">Int32</span><span class="sxs-lookup"><span data-stu-id="208eb-119">Int32</span></span>|<span data-ttu-id="208eb-120">イベントを繰り返す回数を指定します。</span><span class="sxs-lookup"><span data-stu-id="208eb-120">The number of times to repeat the event.</span></span> <span data-ttu-id="208eb-121">必須です。**type** が `numbered` の場合、正の値である必要があります。</span><span class="sxs-lookup"><span data-stu-id="208eb-121">Required and must be positive if **type** is `numbered`.</span></span>|
|<span data-ttu-id="208eb-122">recurrenceTimeZone</span><span class="sxs-lookup"><span data-stu-id="208eb-122">recurrenceTimeZone</span></span>|<span data-ttu-id="208eb-123">String</span><span class="sxs-lookup"><span data-stu-id="208eb-123">String</span></span> |<span data-ttu-id="208eb-124">**startDate** プロパティと **endDate** プロパティのタイム ゾーン。</span><span class="sxs-lookup"><span data-stu-id="208eb-124">Time zone for the **startDate** and **endDate** properties.</span></span> <span data-ttu-id="208eb-125">省略可能。</span><span class="sxs-lookup"><span data-stu-id="208eb-125">Optional.</span></span> <span data-ttu-id="208eb-126">指定されていない場合は、イベントのタイム ゾーンが使用されます。</span><span class="sxs-lookup"><span data-stu-id="208eb-126">If not specified, the time zone of the event is used.</span></span>|
|<span data-ttu-id="208eb-127">startDate</span><span class="sxs-lookup"><span data-stu-id="208eb-127">startDate</span></span>|<span data-ttu-id="208eb-128">Date</span><span class="sxs-lookup"><span data-stu-id="208eb-128">Date</span></span>|<span data-ttu-id="208eb-129">定期的なパターンの適用を開始する日付。</span><span class="sxs-lookup"><span data-stu-id="208eb-129">The date to start applying the recurrence pattern.</span></span> <span data-ttu-id="208eb-130">イベントの定期的なパターンによっては、最初に会議が発生するのは、この日付以降になる場合があります。</span><span class="sxs-lookup"><span data-stu-id="208eb-130">The first occurrence of the meeting may be this date or later, depending on the recurrence pattern of the event.</span></span> <span data-ttu-id="208eb-131">定期的な[イベント](event.md)の **start** プロパティと同じ値である必要があります。</span><span class="sxs-lookup"><span data-stu-id="208eb-131">Must be the same value as the **start** property of the recurring [event](event.md).</span></span> <span data-ttu-id="208eb-132">必須。</span><span class="sxs-lookup"><span data-stu-id="208eb-132">Required.</span></span>|
|<span data-ttu-id="208eb-133">type</span><span class="sxs-lookup"><span data-stu-id="208eb-133">type</span></span>|<span data-ttu-id="208eb-134">String</span><span class="sxs-lookup"><span data-stu-id="208eb-134">String</span></span>|<span data-ttu-id="208eb-135">繰り返す期間。</span><span class="sxs-lookup"><span data-stu-id="208eb-135">The recurrence range.</span></span> <span data-ttu-id="208eb-136">使用可能な値は、`endDate`、`noEnd`、`numbered` です。</span><span class="sxs-lookup"><span data-stu-id="208eb-136">Possible values are: `endDate`, `noEnd`, `numbered`.</span></span> <span data-ttu-id="208eb-137">必須。</span><span class="sxs-lookup"><span data-stu-id="208eb-137">Required.</span></span>|

<span data-ttu-id="208eb-138">**type** プロパティを使用して、**recurrenceRange** のさまざまな種類から期間を指定します。</span><span class="sxs-lookup"><span data-stu-id="208eb-138">Use the **type** property to specify the different types of **recurrenceRange**.</span></span> <span data-ttu-id="208eb-139">種類ごとに必要なプロパティについては、次の表の説明を参照してください。</span><span class="sxs-lookup"><span data-stu-id="208eb-139">Note the required properties for each type, as described in the following table.</span></span>

| <span data-ttu-id="208eb-140">type プロパティ</span><span class="sxs-lookup"><span data-stu-id="208eb-140">type property</span></span>  | <span data-ttu-id="208eb-141">繰り返す期間の種類</span><span class="sxs-lookup"><span data-stu-id="208eb-141">Type of recurrence range</span></span> | <span data-ttu-id="208eb-142">説明</span><span class="sxs-lookup"><span data-stu-id="208eb-142">Description</span></span> | <span data-ttu-id="208eb-143">例</span><span class="sxs-lookup"><span data-stu-id="208eb-143">Example</span></span> | <span data-ttu-id="208eb-144">必須のプロパティ</span><span class="sxs-lookup"><span data-stu-id="208eb-144">Required properties</span></span> |
|:-------|:---------------|:--------|:--------|:--------|
|`endDate` |<span data-ttu-id="208eb-145">終了日が指定された期間</span><span class="sxs-lookup"><span data-stu-id="208eb-145">Range with end date</span></span> | <span data-ttu-id="208eb-146">**startDate** と **endDate** の範囲内の、対応する定期的なパターンに適合するすべての日に、イベントが繰り返されます。</span><span class="sxs-lookup"><span data-stu-id="208eb-146">Event repeats on all the days that fit the corresponding recurrence pattern between the **startDate** and **endDate** inclusive.</span></span> | <span data-ttu-id="208eb-147">2017 年 6 月 1 日から 2017 年 6 月 15 日の期間で、イベントを繰り返します。</span><span class="sxs-lookup"><span data-stu-id="208eb-147">Repeat event in the date range between June 1, 2017 and June 15, 2017.</span></span> | <span data-ttu-id="208eb-148">**type**、**startDate**、**endDate**</span><span class="sxs-lookup"><span data-stu-id="208eb-148">**type**, **startDate**, **endDate**</span></span> | 
|`noEnd`   |<span data-ttu-id="208eb-149">終了日が指定されていない期間</span><span class="sxs-lookup"><span data-stu-id="208eb-149">Range without an end date</span></span> | <span data-ttu-id="208eb-150">**startDate** に始まる、対応する定期的なパターンに適合するすべての日に、イベントが繰り返されます。</span><span class="sxs-lookup"><span data-stu-id="208eb-150">Event repeats on all the days that fit the corresponding recurrence pattern beginning on the **startDate**.</span></span> | <span data-ttu-id="208eb-151">2017 年 6 月 1 日に始まる期間に、イベントを無期限に繰り返します。</span><span class="sxs-lookup"><span data-stu-id="208eb-151">Repeat event in the date range starting on June 1, 2017 indefinitely.</span></span> | <span data-ttu-id="208eb-152">**type**、**startDate**</span><span class="sxs-lookup"><span data-stu-id="208eb-152">**type**, **startDate**</span></span> |
|`numbered`|<span data-ttu-id="208eb-153">発生回数を指定した期間</span><span class="sxs-lookup"><span data-stu-id="208eb-153">Range with specific number of occurrences</span></span> | <span data-ttu-id="208eb-154">**startDate** に始まる定期的なパターンに基づいて、**numberOfOccurrences** で指定した回数、イベントが繰り返されます。</span><span class="sxs-lookup"><span data-stu-id="208eb-154">Event repeats for the **numberOfOccurrences** based on the recurrence pattern beginning on the **startDate**.</span></span> | <span data-ttu-id="208eb-155">2017 年 6 月 1 日に始まる期間に、イベントを 10 回繰り返します。</span><span class="sxs-lookup"><span data-stu-id="208eb-155">Repeat event in the date range starting on June 1, 2017, for 10 occurrences.</span></span>  | <span data-ttu-id="208eb-156">**type**、**startDate**、**numberOfOccurrences**</span><span class="sxs-lookup"><span data-stu-id="208eb-156">**type**, **startDate**, **numberOfOccurrences**</span></span> |

## <a name="json-representation"></a><span data-ttu-id="208eb-157">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="208eb-157">JSON representation</span></span>

<span data-ttu-id="208eb-158">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="208eb-158">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recurrenceRange"
}-->

```json
{
  "endDate": "String (timestamp)",
  "numberOfOccurrences": 1024,
  "recurrenceTimeZone": "string",
  "startDate": "String (timestamp)",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "recurrenceRange resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Warning: /api-reference/beta/resources/recurrencerange.md:\r\n      Failed to parse any rows out of table with headers: | type property  | Type of recurrence range | Description | Example | Required properties |"
  ]
}
-->
