---
title: recurrencePattern リソースの種類
description: 定期的なイベントを繰り返す頻度について説明します。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 48fca7295d7305fd915cf40a32c227f1fbf08c5c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008741"
---
# <a name="recurrencepattern-resource-type"></a><span data-ttu-id="0593d-103">recurrencePattern リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0593d-103">recurrencePattern resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0593d-104">定期的な[イベント](event.md)を繰り返す頻度について説明します。</span><span class="sxs-lookup"><span data-stu-id="0593d-104">Describes the frequency by which a recurring [event](event.md) repeats.</span></span>

<span data-ttu-id="0593d-105">シナリオに応じて、定期的なイベントの 6 通りの繰り返しパターンのいずれかを指定できます。</span><span class="sxs-lookup"><span data-stu-id="0593d-105">You can specify the recurrence pattern of a recurring event in one of 6 ways depending on your scenario.</span></span> <span data-ttu-id="0593d-106">パターンの種類ごとに、次のイベント発生までの期間を指定します。</span><span class="sxs-lookup"><span data-stu-id="0593d-106">For each pattern type, specify the amount of time between occurrences.</span></span> <span data-ttu-id="0593d-107">イベントに対して指定した期間内に発生する定期的なイベントは、必ずこのパターンに従って発生します。</span><span class="sxs-lookup"><span data-stu-id="0593d-107">The actual occurrences of the recurring event always follow this pattern falling within the date range that you specify for the event.</span></span> <span data-ttu-id="0593d-108">定期的なイベントは常に、**recurrencePattern** (イベントを繰り返す頻度)、および [recurrenceRange](recurrencerange.md) (イベントを繰り返す期間) によって定義されます。</span><span class="sxs-lookup"><span data-stu-id="0593d-108">A recurring event is always defined by its **recurrencePattern** (how frequently the event repeats), and its [recurrenceRange](recurrencerange.md) (over how long the event repeats).</span></span>

<span data-ttu-id="0593d-109">**type** プロパティを使用して **recurrencePattern** のさまざまな種類からパターンを指定し、**interval** プロパティを使用してイベント発生までの期間を指定します。**type** によって、その期間は数日、数週間、数か月、数年になる可能性があります。</span><span class="sxs-lookup"><span data-stu-id="0593d-109">Use the **type** property to specify the different types of **recurrencePattern**, and the **interval** property to specify the time between occurrences, which can be in number of days, weeks, months, or years, depending on the **type**.</span></span> <span data-ttu-id="0593d-110">種類ごとに必要なプロパティについては、次の表の説明を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0593d-110">Note which properties are required for each type, as described in the following table.</span></span>

> <span data-ttu-id="0593d-111">**注** 定期的なパターンに必要なプロパティのみを含めます。</span><span class="sxs-lookup"><span data-stu-id="0593d-111">**Note** Include only the properties that you need for a recurrence pattern.</span></span> <span data-ttu-id="0593d-112">含めたプロパティにサポートされている値がない場合、エラーになる可能性があります。</span><span class="sxs-lookup"><span data-stu-id="0593d-112">Any property that you include that does not have a supported value would result in an error.</span></span>

| <span data-ttu-id="0593d-113">定期的なパターンの種類</span><span class="sxs-lookup"><span data-stu-id="0593d-113">Type of recurrence pattern</span></span> | <span data-ttu-id="0593d-114">type プロパティの値</span><span class="sxs-lookup"><span data-stu-id="0593d-114">Value of type property</span></span> | <span data-ttu-id="0593d-115">説明</span><span class="sxs-lookup"><span data-stu-id="0593d-115">Description</span></span> | <span data-ttu-id="0593d-116">例</span><span class="sxs-lookup"><span data-stu-id="0593d-116">Example</span></span> | <span data-ttu-id="0593d-117">必須のプロパティ</span><span class="sxs-lookup"><span data-stu-id="0593d-117">Required properties</span></span> |
|:---------------|:--------|:--------|:--------|:----------|
| <span data-ttu-id="0593d-118">Daily (日単位)</span><span class="sxs-lookup"><span data-stu-id="0593d-118">Daily</span></span> | `daily` | <span data-ttu-id="0593d-119">**interval** で指定された、次のイベント発生までの日数に基づいて、イベントが繰り返されます。</span><span class="sxs-lookup"><span data-stu-id="0593d-119">Event repeats based on the number of days specified by **interval** between occurrences.</span></span> | <span data-ttu-id="0593d-120">イベントを 3 日ごとに繰り返します。</span><span class="sxs-lookup"><span data-stu-id="0593d-120">Repeat event every 3 days.</span></span> | <span data-ttu-id="0593d-121">**type**、**interval**</span><span class="sxs-lookup"><span data-stu-id="0593d-121">**type**, **interval**</span></span> |
| <span data-ttu-id="0593d-122">Weekly (週単位)</span><span class="sxs-lookup"><span data-stu-id="0593d-122">Weekly</span></span> | `weekly` | <span data-ttu-id="0593d-123">次の一連のイベント発生までの週数に基づいて、同じ曜日 (複数の曜日も可) にイベントが繰り返されます。</span><span class="sxs-lookup"><span data-stu-id="0593d-123">Event repeats on the same day or days of the week, based on the number of weeks between each set of occurrences.</span></span> | <span data-ttu-id="0593d-124">イベントを隔週の月曜日と火曜日に繰り返します。</span><span class="sxs-lookup"><span data-stu-id="0593d-124">Repeat event Monday and Tuesday of every other week.</span></span> | <span data-ttu-id="0593d-125">**type**、**interval**、**daysOfWeek**、**firstDayOfWeek**</span><span class="sxs-lookup"><span data-stu-id="0593d-125">**type**, **interval**, **daysOfWeek**, **firstDayOfWeek**</span></span> |
| <span data-ttu-id="0593d-126">絶対月</span><span class="sxs-lookup"><span data-stu-id="0593d-126">Absolute monthly</span></span> | `absoluteMonthly` | <span data-ttu-id="0593d-127">次のイベント発生までの月数に基づいて、該当月の指定日 (例: 15 日) にイベントが繰り返されます。</span><span class="sxs-lookup"><span data-stu-id="0593d-127">Event repeats on the specified day of the month (e.g. the 15th), based on the number of months between occurrences.</span></span> | <span data-ttu-id="0593d-128">四半期 (3 か月ごと) の 15 日にイベントを繰り返します。</span><span class="sxs-lookup"><span data-stu-id="0593d-128">Repeat event quarterly (every 3 months) on the 15th.</span></span> | <span data-ttu-id="0593d-129">**type**、**interval**、**dayOfMonth**</span><span class="sxs-lookup"><span data-stu-id="0593d-129">**type**, **interval**, **dayOfMonth**</span></span> |
| <span data-ttu-id="0593d-130">相対月</span><span class="sxs-lookup"><span data-stu-id="0593d-130">Relative monthly</span></span> | `relativeMonthly` | <span data-ttu-id="0593d-131">次のイベント発生までの月数に基づいて、該当月の同じ相対位置にある指定した曜日 (複数の曜日も可) にイベントが繰り返されます。</span><span class="sxs-lookup"><span data-stu-id="0593d-131">Event repeats on the specified day or days of the week, in the same relative position in the month, based on the number of months between occurrences.</span></span> | <span data-ttu-id="0593d-132">3 か月ごとに、第 2 木曜日または金曜日にイベントを繰り返します。</span><span class="sxs-lookup"><span data-stu-id="0593d-132">Repeat event on the second Thursday or Friday every three months.</span></span> | <span data-ttu-id="0593d-133">**type**、**interval**、**daysOfWeek**</span><span class="sxs-lookup"><span data-stu-id="0593d-133">**type**, **interval**, **daysOfWeek**</span></span> |
| <span data-ttu-id="0593d-134">絶対年</span><span class="sxs-lookup"><span data-stu-id="0593d-134">Absolute yearly</span></span> | `absoluteYearly` | <span data-ttu-id="0593d-135">次のイベント発生までの年数に基づいて、指定した日付にイベントが繰り返されます。</span><span class="sxs-lookup"><span data-stu-id="0593d-135">Event repeats on the specified day and month, based on the number of years between occurrences.</span></span> | <span data-ttu-id="0593d-136">3 年ごとに、3 月 15 日にイベントを繰り返します。</span><span class="sxs-lookup"><span data-stu-id="0593d-136">Repeat event on the 15th of March every 3 years.</span></span> | <span data-ttu-id="0593d-137">**type**、**interval**、**dayOfMonth**、**month**</span><span class="sxs-lookup"><span data-stu-id="0593d-137">**type**, **interval**, **dayOfMonth**, **month**</span></span> |
| <span data-ttu-id="0593d-138">相対年</span><span class="sxs-lookup"><span data-stu-id="0593d-138">Relative yearly</span></span> | `relativeYearly` | <span data-ttu-id="0593d-139">次のイベント発生までの年数に基づいて、該当年の特定の月の同じ相対位置にある指定した曜日 (複数の曜日も可) にイベントが繰り返されます。</span><span class="sxs-lookup"><span data-stu-id="0593d-139">Event repeats on the specified day or days of the week, in the same relative position in a specific month of the year, based on the number of years between occurrences.</span></span> | <span data-ttu-id="0593d-140">3 年ごとに、11 月の第 2 木曜日または金曜日にイベントを繰り返します。</span><span class="sxs-lookup"><span data-stu-id="0593d-140">Repeat event on the second Thursday or Friday of every November every 3 years.</span></span> | <span data-ttu-id="0593d-141">**type**、**interval**、**daysOfWeek**、**month**</span><span class="sxs-lookup"><span data-stu-id="0593d-141">**type**, **interval**, **daysOfWeek**, **month**</span></span> |


## <a name="properties"></a><span data-ttu-id="0593d-142">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0593d-142">Properties</span></span>
| <span data-ttu-id="0593d-143">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0593d-143">Property</span></span>     | <span data-ttu-id="0593d-144">型</span><span class="sxs-lookup"><span data-stu-id="0593d-144">Type</span></span>   |<span data-ttu-id="0593d-145">説明</span><span class="sxs-lookup"><span data-stu-id="0593d-145">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0593d-146">dayOfMonth</span><span class="sxs-lookup"><span data-stu-id="0593d-146">dayOfMonth</span></span>|<span data-ttu-id="0593d-147">Int32</span><span class="sxs-lookup"><span data-stu-id="0593d-147">Int32</span></span>|<span data-ttu-id="0593d-148">イベントが発生する月の日付。</span><span class="sxs-lookup"><span data-stu-id="0593d-148">The day of the month on which the event occurs.</span></span> <span data-ttu-id="0593d-149">**type** が、`absoluteMonthly` または `absoluteYearly` の場合、必要です。</span><span class="sxs-lookup"><span data-stu-id="0593d-149">Required if **type** is `absoluteMonthly` or `absoluteYearly`.</span></span> |
|<span data-ttu-id="0593d-150">daysOfWeek</span><span class="sxs-lookup"><span data-stu-id="0593d-150">daysOfWeek</span></span>|<span data-ttu-id="0593d-151">String collection</span><span class="sxs-lookup"><span data-stu-id="0593d-151">String collection</span></span>|<span data-ttu-id="0593d-152">イベントが発生する曜日のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="0593d-152">A collection of the days of the week on which the event occurs.</span></span> <span data-ttu-id="0593d-153">可能な値は、`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday` です。</span><span class="sxs-lookup"><span data-stu-id="0593d-153">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span> <br><span data-ttu-id="0593d-154">**type** が `relativeMonthly` または `relativeYearly` であり、**daysOfWeek** で 1 日以上を指定する場合、パターンを満たす最初の日にイベントが発生します。</span><span class="sxs-lookup"><span data-stu-id="0593d-154">If **type** is `relativeMonthly` or `relativeYearly`, and **daysOfWeek** specifies more than one day, the event falls on the first day that satisfies the pattern.</span></span> <br> <span data-ttu-id="0593d-155">**type** が `weekly`、`relativeMonthly`、`relativeYearly` の場合、必要です。</span><span class="sxs-lookup"><span data-stu-id="0593d-155">Required if **type** is `weekly`, `relativeMonthly`, or `relativeYearly`.</span></span>|
|<span data-ttu-id="0593d-156">firstDayOfWeek</span><span class="sxs-lookup"><span data-stu-id="0593d-156">firstDayOfWeek</span></span>|<span data-ttu-id="0593d-157">String</span><span class="sxs-lookup"><span data-stu-id="0593d-157">String</span></span>|<span data-ttu-id="0593d-158">週の最初の曜日。</span><span class="sxs-lookup"><span data-stu-id="0593d-158">The first day of the week.</span></span> <span data-ttu-id="0593d-159">使用可能な値は、`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday` です。</span><span class="sxs-lookup"><span data-stu-id="0593d-159">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span> <span data-ttu-id="0593d-160">既定値は `sunday` です。</span><span class="sxs-lookup"><span data-stu-id="0593d-160">Default is `sunday`.</span></span> <span data-ttu-id="0593d-161">**type** が `weekly` の場合、必要です。</span><span class="sxs-lookup"><span data-stu-id="0593d-161">Required if **type** is `weekly`.</span></span> |
|<span data-ttu-id="0593d-162">index</span><span class="sxs-lookup"><span data-stu-id="0593d-162">index</span></span>|<span data-ttu-id="0593d-163">String</span><span class="sxs-lookup"><span data-stu-id="0593d-163">String</span></span>|<span data-ttu-id="0593d-164">月の最初のインスタンスから数えて、**daysOfsWeek** で指定された許可日数のどのインスタンスでイベントが発生するか指定します。</span><span class="sxs-lookup"><span data-stu-id="0593d-164">Specifies on which instance of the allowed days specified in **daysOfsWeek** the event occurs, counted from the first instance in the month.</span></span> <span data-ttu-id="0593d-165">使用可能な値は、`first`、`second`、`third`、`fourth`、`last` です。</span><span class="sxs-lookup"><span data-stu-id="0593d-165">Possible values are: `first`, `second`, `third`, `fourth`, `last`.</span></span> <span data-ttu-id="0593d-166">既定値は `first` です。</span><span class="sxs-lookup"><span data-stu-id="0593d-166">Default is `first`.</span></span> <span data-ttu-id="0593d-167">オプションです。**type** が `relativeMonthly` か `relativeYearly` の場合、使用します。</span><span class="sxs-lookup"><span data-stu-id="0593d-167">Optional and used if **type** is `relativeMonthly` or `relativeYearly`.</span></span> |
|<span data-ttu-id="0593d-168">interval</span><span class="sxs-lookup"><span data-stu-id="0593d-168">interval</span></span>|<span data-ttu-id="0593d-169">Int32</span><span class="sxs-lookup"><span data-stu-id="0593d-169">Int32</span></span>|<span data-ttu-id="0593d-170">次のイベント発生までの単位数。**type** によって、単位は、日、週、月、年などになります。</span><span class="sxs-lookup"><span data-stu-id="0593d-170">The number of units between occurrences, where units can be in days, weeks, months, or years, depending on the **type**.</span></span> <span data-ttu-id="0593d-171">必須です。</span><span class="sxs-lookup"><span data-stu-id="0593d-171">Required.</span></span> |
|<span data-ttu-id="0593d-172">month</span><span class="sxs-lookup"><span data-stu-id="0593d-172">month</span></span>|<span data-ttu-id="0593d-173">Int32</span><span class="sxs-lookup"><span data-stu-id="0593d-173">Int32</span></span>|<span data-ttu-id="0593d-174">イベントが発生する月。</span><span class="sxs-lookup"><span data-stu-id="0593d-174">The month in which the event occurs.</span></span>  <span data-ttu-id="0593d-175">これは、1 から 12 までの数字です。</span><span class="sxs-lookup"><span data-stu-id="0593d-175">This is a number from 1 to 12.</span></span>|
|<span data-ttu-id="0593d-176">type</span><span class="sxs-lookup"><span data-stu-id="0593d-176">type</span></span>|<span data-ttu-id="0593d-177">String</span><span class="sxs-lookup"><span data-stu-id="0593d-177">String</span></span>|<span data-ttu-id="0593d-178">定期的なパターンの種類は、`daily`、`weekly`、`absoluteMonthly`、`relativeMonthly`、`absoluteYearly`、`relativeYearly` です。</span><span class="sxs-lookup"><span data-stu-id="0593d-178">The recurrence pattern type: `daily`, `weekly`, `absoluteMonthly`, `relativeMonthly`, `absoluteYearly`, `relativeYearly`.</span></span> <span data-ttu-id="0593d-179">必須。</span><span class="sxs-lookup"><span data-stu-id="0593d-179">Required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0593d-180">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0593d-180">JSON representation</span></span>

<span data-ttu-id="0593d-181">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="0593d-181">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recurrencePattern"
}-->

```json
{
  "dayOfMonth": 1024,
  "daysOfWeek": ["String"],
  "firstDayOfWeek": "String",
  "index": "String",
  "interval": 1024,
  "month": 1024,
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "recurrencePattern resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
