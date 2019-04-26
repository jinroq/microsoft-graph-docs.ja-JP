---
title: 定期的に繰り返される予定を、Outlook で定期的なイベントとして設定する
description: 繰り返しイベントは、Outlook カレンダーの重要な部分です。 毎週行う上司との個別の打ち合わせや毎月第 2 火曜日に行われる部門全体のレビュー会議などの繰り返しイベントでは、イベントを一度作成するだけで、シリーズの残りの部分はサーバーによって入力されます。
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: 9cdd7e7170dc48c2739514674786893efeae1b4e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32570349"
---
# <a name="schedule-repeating-appointments-as-recurring-events-in-outlook"></a><span data-ttu-id="23da3-104">定期的に繰り返される予定を、Outlook で定期的なイベントとして設定する</span><span class="sxs-lookup"><span data-stu-id="23da3-104">Schedule repeating appointments as recurring events in Outlook</span></span>

<span data-ttu-id="23da3-105">繰り返しイベントは、Outlook カレンダーの重要な部分です。</span><span class="sxs-lookup"><span data-stu-id="23da3-105">Recurring events are an important part of Outlook calendaring.</span></span> <span data-ttu-id="23da3-106">毎週行う上司との個別の打ち合わせや毎月第 2 火曜日に行われる部門全体のレビュー会議などの繰り返しイベントでは、イベントを一度作成するだけで、シリーズの残りの部分はサーバーによって入力されます。</span><span class="sxs-lookup"><span data-stu-id="23da3-106">Whether it's a weekly one-on-one meeting with your manager, or a division-wide review meeting that happens on the second Tuesday of each month, recurring events make it easy to create the event once, and let the server fill in the rest of the series.</span></span>

<span data-ttu-id="23da3-107">繰り返しイベントを個々の予定に「拡張」するための情報のキー ビットとなるものが繰り返しルールです。</span><span class="sxs-lookup"><span data-stu-id="23da3-107">The key bit of information that allows recurring events to "expand" into individual occurrences is the recurrence rule.</span></span> <span data-ttu-id="23da3-108">このルールは、イベントを繰り返す頻度と期間の両方を指定します。</span><span class="sxs-lookup"><span data-stu-id="23da3-108">The rule specifies both how often an event repeats, and for how long.</span></span> <span data-ttu-id="23da3-109">Outlook REST API は、[イベント リソース](/graph/api/resources/event?view=graph-rest-1.0)の**recurrence**プロパティで繰り返しルールをモデル化します。</span><span class="sxs-lookup"><span data-stu-id="23da3-109">The Outlook REST APIs model recurrence rules in the **recurrence** property of the [event resource](/graph/api/resources/event?view=graph-rest-1.0).</span></span> 

<span data-ttu-id="23da3-110">それぞれのパターンは、繰り返しパターン (頻度) と繰り返し範囲 (期間) の 2 つの部分で構成されます。</span><span class="sxs-lookup"><span data-stu-id="23da3-110">Each recurrence is made up of two parts: the recurrence pattern (how often), and the recurrence range (for how long).</span></span>

## <a name="recurrence-patterns"></a><span data-ttu-id="23da3-111">繰り返しパターン</span><span class="sxs-lookup"><span data-stu-id="23da3-111">Recurrence patterns</span></span>

<span data-ttu-id="23da3-112">繰り返しの第 1 の部分は、パターンです。</span><span class="sxs-lookup"><span data-stu-id="23da3-112">The first part of a recurrence is the pattern.</span></span> <span data-ttu-id="23da3-113">これは、イベントを繰り返す頻度を指定します。</span><span class="sxs-lookup"><span data-stu-id="23da3-113">This specifies how often the event repeats.</span></span> <span data-ttu-id="23da3-114">たとえば、イベントを「3 日ごと」、「毎週木曜日」、または「毎年 7 月 22 日」に繰り返すことができます。</span><span class="sxs-lookup"><span data-stu-id="23da3-114">For example, an event could repeat "every 3 days," "every Thursday," or "on July 22 every year."</span></span> <span data-ttu-id="23da3-115">パターンは、API の [recurrencePattern リソース](/graph/api/resources/recurrencepattern?view=graph-rest-1.0)で表されます。</span><span class="sxs-lookup"><span data-stu-id="23da3-115">A pattern is represented in the API by the [recurrencePattern resource](/graph/api/resources/recurrencepattern?view=graph-rest-1.0).</span></span>

<span data-ttu-id="23da3-116">パターンの種類に応じて、**recurrencePattern**の特定のフィールドは、必須、オプションになるか、または無視されます。</span><span class="sxs-lookup"><span data-stu-id="23da3-116">Depending on the type of pattern, certain fields of the **recurrencePattern** are required, optional, or ignored.</span></span>

> <span data-ttu-id="23da3-117">**注**: フィールドが無視される場合でも、検証は行われます。</span><span class="sxs-lookup"><span data-stu-id="23da3-117">**Note**: Even if a field is ignored, it is still validated.</span></span> <span data-ttu-id="23da3-118">使用可能な値のセット リストがフィールドに含まれる場合、そのフィールドが無視されても、許可されたセットの範囲外の値を使用するとエラーが発生します。</span><span class="sxs-lookup"><span data-stu-id="23da3-118">If a field has a set list of possible values, using a value outside the allowed set causes an error, even if that field is ignored.</span></span>

<span data-ttu-id="23da3-119">使用可能なパターンの種類を見てみましょう。</span><span class="sxs-lookup"><span data-stu-id="23da3-119">Let's take a look at each of the possible pattern types.</span></span>

### <a name="daily"></a><span data-ttu-id="23da3-120">Daily (日単位)</span><span class="sxs-lookup"><span data-stu-id="23da3-120">Daily</span></span>

<span data-ttu-id="23da3-121">Daily (日単位) の繰り返しパターンでは、次の予定までの日数に基づいてイベントが繰り返されます。</span><span class="sxs-lookup"><span data-stu-id="23da3-121">The daily recurrence pattern causes an event to repeat based on a number of days between each occurrence.</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="23da3-122">関連するプロパティ</span><span class="sxs-lookup"><span data-stu-id="23da3-122">Relevant properties</span></span>

| <span data-ttu-id="23da3-123">プロパティ</span><span class="sxs-lookup"><span data-stu-id="23da3-123">Property</span></span> | <span data-ttu-id="23da3-124">関連性</span><span class="sxs-lookup"><span data-stu-id="23da3-124">Relevance</span></span> | <span data-ttu-id="23da3-125">説明</span><span class="sxs-lookup"><span data-stu-id="23da3-125">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="23da3-126">**interval**</span><span class="sxs-lookup"><span data-stu-id="23da3-126">**interval**</span></span> | <span data-ttu-id="23da3-127">必須</span><span class="sxs-lookup"><span data-stu-id="23da3-127">Required</span></span> | <span data-ttu-id="23da3-128">次の予定までの日数を指定します。</span><span class="sxs-lookup"><span data-stu-id="23da3-128">Specifies the number of days between each occurrence.</span></span> |
| <span data-ttu-id="23da3-129">**type**</span><span class="sxs-lookup"><span data-stu-id="23da3-129">**type**</span></span> | <span data-ttu-id="23da3-130">必須</span><span class="sxs-lookup"><span data-stu-id="23da3-130">Required</span></span> | <span data-ttu-id="23da3-131">`daily` に設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="23da3-131">Must be set to `daily`.</span></span> |

#### <a name="examples"></a><span data-ttu-id="23da3-132">例</span><span class="sxs-lookup"><span data-stu-id="23da3-132">Examples</span></span>

- <span data-ttu-id="23da3-133">このイベントを毎日繰り返す</span><span class="sxs-lookup"><span data-stu-id="23da3-133">Repeat this event every day</span></span>

  ```json
    "pattern": {
      "type": "daily",
      "interval": 1
    }
  ```
- <span data-ttu-id="23da3-134">このイベントを 3 日おきに繰り返す</span><span class="sxs-lookup"><span data-stu-id="23da3-134">Repeat this event every three days</span></span>

  ```json
    "pattern": {
      "type": "daily",
      "interval": 3
    }
  ```

### <a name="weekly"></a><span data-ttu-id="23da3-135">Weekly (週単位)</span><span class="sxs-lookup"><span data-stu-id="23da3-135">Weekly</span></span>

<span data-ttu-id="23da3-136">Weekly (週単位) の定期的なパターンでは、次の予定セットまでの週数に基づいて、同じ曜日 (複数の曜日も可) にイベントが繰り返されます。</span><span class="sxs-lookup"><span data-stu-id="23da3-136">The weekly recurrence pattern causes an event to repeat on the same day or days of the week, based on the number of weeks between each set of occurrences.</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="23da3-137">関連するプロパティ</span><span class="sxs-lookup"><span data-stu-id="23da3-137">Relevant properties</span></span>

| <span data-ttu-id="23da3-138">プロパティ</span><span class="sxs-lookup"><span data-stu-id="23da3-138">Property</span></span> | <span data-ttu-id="23da3-139">関連性</span><span class="sxs-lookup"><span data-stu-id="23da3-139">Relevance</span></span> | <span data-ttu-id="23da3-140">説明</span><span class="sxs-lookup"><span data-stu-id="23da3-140">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="23da3-141">**daysOfWeek**</span><span class="sxs-lookup"><span data-stu-id="23da3-141">**daysOfWeek**</span></span> | <span data-ttu-id="23da3-142">必須</span><span class="sxs-lookup"><span data-stu-id="23da3-142">Required</span></span> | <span data-ttu-id="23da3-143">イベントが発生する曜日 (複数可) を指定します。</span><span class="sxs-lookup"><span data-stu-id="23da3-143">Specifies on which day(s) of the week the event occurs.</span></span> |
| <span data-ttu-id="23da3-144">**firstDayOfWeek**</span><span class="sxs-lookup"><span data-stu-id="23da3-144">**firstDayOfWeek**</span></span> | <span data-ttu-id="23da3-145">省略可能</span><span class="sxs-lookup"><span data-stu-id="23da3-145">Optional</span></span> | <span data-ttu-id="23da3-146">週の最初の曜日となる日を指定します。</span><span class="sxs-lookup"><span data-stu-id="23da3-146">Specifies which day is considered the first day of the week.</span></span> <span data-ttu-id="23da3-147">既定値: `Sunday`。</span><span class="sxs-lookup"><span data-stu-id="23da3-147">Default value: `Sunday`.</span></span> |
| <span data-ttu-id="23da3-148">**interval**</span><span class="sxs-lookup"><span data-stu-id="23da3-148">**interval**</span></span> | <span data-ttu-id="23da3-149">必須</span><span class="sxs-lookup"><span data-stu-id="23da3-149">Required</span></span> | <span data-ttu-id="23da3-150">次の予定までの週数を指定します。</span><span class="sxs-lookup"><span data-stu-id="23da3-150">Specifies the number of weeks between each set of occurrences.</span></span> |
| <span data-ttu-id="23da3-151">**type**</span><span class="sxs-lookup"><span data-stu-id="23da3-151">**type**</span></span> | <span data-ttu-id="23da3-152">必須</span><span class="sxs-lookup"><span data-stu-id="23da3-152">Required</span></span> | <span data-ttu-id="23da3-153">`weekly` に設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="23da3-153">Must be set to `weekly`.</span></span> |

#### <a name="examples"></a><span data-ttu-id="23da3-154">例</span><span class="sxs-lookup"><span data-stu-id="23da3-154">Examples</span></span>

- <span data-ttu-id="23da3-155">このイベントを毎週木曜日に繰り返す</span><span class="sxs-lookup"><span data-stu-id="23da3-155">Repeat this event every Thursday</span></span>

  ```json
    "pattern": {
      "type": "weekly",
      "interval": 1,
      "daysOfWeek": [ "Thursday" ]
    }
  ```
- <span data-ttu-id="23da3-156">このイベントを隔週の月曜日と火曜日に繰り返す</span><span class="sxs-lookup"><span data-stu-id="23da3-156">Repeat this event every other Monday and Tuesday</span></span>

  ```json
    "pattern": {
      "type": "weekly",
      "interval": 2,
      "daysOfWeek": [
        "Monday",
        "Tuesday"
      ]
    }
  ```

### <a name="absolute-monthly"></a><span data-ttu-id="23da3-157">絶対月</span><span class="sxs-lookup"><span data-stu-id="23da3-157">Absolute monthly</span></span>

<span data-ttu-id="23da3-158">絶対月というパターンでは、次の予定までの月数に基づいて月の同じ日 (たとえば、15 日) にイベントが繰り返されます。</span><span class="sxs-lookup"><span data-stu-id="23da3-158">The absolute monthly pattern causes an event to repeat on the same day of the month (for example, the 15th), based on the number of months between each occurrence.</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="23da3-159">関連するプロパティ</span><span class="sxs-lookup"><span data-stu-id="23da3-159">Relevant properties</span></span>

| <span data-ttu-id="23da3-160">プロパティ</span><span class="sxs-lookup"><span data-stu-id="23da3-160">Property</span></span> | <span data-ttu-id="23da3-161">関連性</span><span class="sxs-lookup"><span data-stu-id="23da3-161">Relevance</span></span> | <span data-ttu-id="23da3-162">説明</span><span class="sxs-lookup"><span data-stu-id="23da3-162">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="23da3-163">**dayOfMonth**</span><span class="sxs-lookup"><span data-stu-id="23da3-163">**dayOfMonth**</span></span> | <span data-ttu-id="23da3-164">必須</span><span class="sxs-lookup"><span data-stu-id="23da3-164">Required</span></span> | <span data-ttu-id="23da3-165">イベントが発生する月の日付を指定します。</span><span class="sxs-lookup"><span data-stu-id="23da3-165">Specifies on which day of the month the event occurs.</span></span> |
| <span data-ttu-id="23da3-166">**interval**</span><span class="sxs-lookup"><span data-stu-id="23da3-166">**interval**</span></span> | <span data-ttu-id="23da3-167">必須</span><span class="sxs-lookup"><span data-stu-id="23da3-167">Required</span></span> | <span data-ttu-id="23da3-168">次の予定までの月数を指定します。</span><span class="sxs-lookup"><span data-stu-id="23da3-168">Specifies the number of months between each occurrence.</span></span> |
| <span data-ttu-id="23da3-169">**type**</span><span class="sxs-lookup"><span data-stu-id="23da3-169">**type**</span></span> | <span data-ttu-id="23da3-170">必須</span><span class="sxs-lookup"><span data-stu-id="23da3-170">Required</span></span> | <span data-ttu-id="23da3-171">`absoluteMonthly` に設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="23da3-171">Must be set to `absoluteMonthly`.</span></span> |

#### <a name="examples"></a><span data-ttu-id="23da3-172">例</span><span class="sxs-lookup"><span data-stu-id="23da3-172">Examples</span></span>

- <span data-ttu-id="23da3-173">毎月 15 日にこのイベントを繰り返す</span><span class="sxs-lookup"><span data-stu-id="23da3-173">Repeat this event on the 15th of every month</span></span>

  ```json
    "pattern": {
      "type": "absoluteMonthly",
      "interval": 1,
      "dayOfMonth": 15
    }
  ```
- <span data-ttu-id="23da3-174">四半期 (3 か月ごと) の 7 日にこのイベントを繰り返す</span><span class="sxs-lookup"><span data-stu-id="23da3-174">Repeat this event quarterly (every 3 months) on the 7th</span></span>

  ```json
    "pattern": {
      "type": "absoluteMonthly",
      "interval": 3,
      "dayOfMonth": 7
    }
  ```

### <a name="relative-monthly"></a><span data-ttu-id="23da3-175">相対月</span><span class="sxs-lookup"><span data-stu-id="23da3-175">Relative monthly</span></span>

<span data-ttu-id="23da3-176">相対月というパターンでは、次の予定までの月数に基づいて、月の同じ相対位置にある同じ曜日にイベントが繰り返されます。</span><span class="sxs-lookup"><span data-stu-id="23da3-176">The relative monthly pattern causes an event to repeat on the same day of the week in the same relative position in the month, based on the number of months between each occurrence.</span></span> <span data-ttu-id="23da3-177">たとえば、「毎月第 2 水曜日」です。</span><span class="sxs-lookup"><span data-stu-id="23da3-177">For example, "every second Wednesday of the month."</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="23da3-178">関連するプロパティ</span><span class="sxs-lookup"><span data-stu-id="23da3-178">Relevant properties</span></span>

| <span data-ttu-id="23da3-179">プロパティ</span><span class="sxs-lookup"><span data-stu-id="23da3-179">Property</span></span> | <span data-ttu-id="23da3-180">関連性</span><span class="sxs-lookup"><span data-stu-id="23da3-180">Relevance</span></span> | <span data-ttu-id="23da3-181">説明</span><span class="sxs-lookup"><span data-stu-id="23da3-181">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="23da3-182">**daysOfWeek**</span><span class="sxs-lookup"><span data-stu-id="23da3-182">**daysOfWeek**</span></span> | <span data-ttu-id="23da3-183">必須</span><span class="sxs-lookup"><span data-stu-id="23da3-183">Required</span></span> | <span data-ttu-id="23da3-184">イベントが発生することができる曜日を指定します。</span><span class="sxs-lookup"><span data-stu-id="23da3-184">Specifies on which day(s) of the week the event can occur.</span></span> <span data-ttu-id="23da3-185">相対月のイベントは、1 か月に一度発生するため、複数の値が指定されている場合、イベントはパターンを満たす最初の日にあたります。</span><span class="sxs-lookup"><span data-stu-id="23da3-185">Relative monthly events only occur once per month, so if more than one value is specified, the event falls on the first day that satisfies the pattern.</span></span> |
| <span data-ttu-id="23da3-186">**index**</span><span class="sxs-lookup"><span data-stu-id="23da3-186">**index**</span></span> | <span data-ttu-id="23da3-187">省略可能</span><span class="sxs-lookup"><span data-stu-id="23da3-187">Optional</span></span> | <span data-ttu-id="23da3-188">月の最初のインスタンスから数えて、**daysOfsWeek** で指定された許可日数のどのインスタンスでイベントが発生するか指定します。</span><span class="sxs-lookup"><span data-stu-id="23da3-188">Specifies on which instance of the allowed days specified in **daysOfsWeek** the event occurs, counted from the first instance in the month.</span></span> <span data-ttu-id="23da3-189">使用可能な値: `first`、`second`、`third`、`fourth`、`last`。</span><span class="sxs-lookup"><span data-stu-id="23da3-189">Possible values: `first`, `second`, `third`, `fourth`, and `last`.</span></span> <span data-ttu-id="23da3-190">既定値: `first`。</span><span class="sxs-lookup"><span data-stu-id="23da3-190">Default value: `first`.</span></span> |
| <span data-ttu-id="23da3-191">**interval**</span><span class="sxs-lookup"><span data-stu-id="23da3-191">**interval**</span></span> | <span data-ttu-id="23da3-192">必須</span><span class="sxs-lookup"><span data-stu-id="23da3-192">Required</span></span> | <span data-ttu-id="23da3-193">次の予定までの月数を指定します。</span><span class="sxs-lookup"><span data-stu-id="23da3-193">Specifies the number of months between each occurrence.</span></span> |
| <span data-ttu-id="23da3-194">**type**</span><span class="sxs-lookup"><span data-stu-id="23da3-194">**type**</span></span> | <span data-ttu-id="23da3-195">必須</span><span class="sxs-lookup"><span data-stu-id="23da3-195">Required</span></span> | <span data-ttu-id="23da3-196">`relativeMonthly` に設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="23da3-196">Must be set to `relativeMonthly`.</span></span> |

#### <a name="examples"></a><span data-ttu-id="23da3-197">例</span><span class="sxs-lookup"><span data-stu-id="23da3-197">Examples</span></span>

- <span data-ttu-id="23da3-198">毎月第 2 水曜日にこのイベントを繰り返す</span><span class="sxs-lookup"><span data-stu-id="23da3-198">Repeat this event on the second Wednesday of every month</span></span>

  ```json
    "pattern": {
      "type": "relativeMonthly",
      "interval": 1,
      "daysOfWeek": [ "Wednesday" ],
      "index": "second"
    }
  ```
- <span data-ttu-id="23da3-199">毎月第 1 木曜日または第 1 金曜日にこのイベントを繰り返す</span><span class="sxs-lookup"><span data-stu-id="23da3-199">Repeat this event on the first Thursday or Friday of every month</span></span>

  ```json
    "pattern": {
      "type": "relativeMonthly",
      "interval": 1,
      "daysOfWeek": [ "Thursday", "Friday" ],
      "index": "first"
    }
  ```

### <a name="absolute-yearly"></a><span data-ttu-id="23da3-200">絶対年</span><span class="sxs-lookup"><span data-stu-id="23da3-200">Absolute yearly</span></span>

<span data-ttu-id="23da3-201">絶対年というパターンでは、次の予定までの年数に基づいて同じ月の同じ日 (たとえば、4 月 15 日) にイベントが繰り返されます。</span><span class="sxs-lookup"><span data-stu-id="23da3-201">The absolute yearly pattern causes an event to repeat on the same month and day (for example, April 15), based on the number of years between each occurrence.</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="23da3-202">関連するプロパティ</span><span class="sxs-lookup"><span data-stu-id="23da3-202">Relevant properties</span></span>

| <span data-ttu-id="23da3-203">プロパティ</span><span class="sxs-lookup"><span data-stu-id="23da3-203">Property</span></span> | <span data-ttu-id="23da3-204">関連性</span><span class="sxs-lookup"><span data-stu-id="23da3-204">Relevance</span></span> | <span data-ttu-id="23da3-205">説明</span><span class="sxs-lookup"><span data-stu-id="23da3-205">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="23da3-206">**dayOfMonth**</span><span class="sxs-lookup"><span data-stu-id="23da3-206">**dayOfMonth**</span></span> | <span data-ttu-id="23da3-207">必須</span><span class="sxs-lookup"><span data-stu-id="23da3-207">Required</span></span> | <span data-ttu-id="23da3-208">イベントが発生する月の日付を指定します。</span><span class="sxs-lookup"><span data-stu-id="23da3-208">Specifies on which day of the month the event occurs.</span></span> |
| <span data-ttu-id="23da3-209">**month**</span><span class="sxs-lookup"><span data-stu-id="23da3-209">**month**</span></span> | <span data-ttu-id="23da3-210">必須</span><span class="sxs-lookup"><span data-stu-id="23da3-210">Required</span></span> | <span data-ttu-id="23da3-211">イベントが発生する月を指定します。</span><span class="sxs-lookup"><span data-stu-id="23da3-211">Specifies in which month the event occurs.</span></span> |
| <span data-ttu-id="23da3-212">**interval**</span><span class="sxs-lookup"><span data-stu-id="23da3-212">**interval**</span></span> | <span data-ttu-id="23da3-213">必須</span><span class="sxs-lookup"><span data-stu-id="23da3-213">Required</span></span> | <span data-ttu-id="23da3-214">次の予定までの年数を指定します。</span><span class="sxs-lookup"><span data-stu-id="23da3-214">Specifies the number of years between each occurrence.</span></span> |
| <span data-ttu-id="23da3-215">**type**</span><span class="sxs-lookup"><span data-stu-id="23da3-215">**type**</span></span> | <span data-ttu-id="23da3-216">必須</span><span class="sxs-lookup"><span data-stu-id="23da3-216">Required</span></span> | <span data-ttu-id="23da3-217">`absoluteYearly` に設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="23da3-217">Must be set to `absoluteYearly`.</span></span> |

#### <a name="example"></a><span data-ttu-id="23da3-218">例</span><span class="sxs-lookup"><span data-stu-id="23da3-218">Example</span></span>

- <span data-ttu-id="23da3-219">毎年 4 月 15 日にこのイベントを繰り返す</span><span class="sxs-lookup"><span data-stu-id="23da3-219">Repeat this event on April 15 every year</span></span>

  ```json
    "pattern": {
      "type": "absoluteYearly",
      "interval": 1,
      "dayOfMonth": 15,
      "month": 4
    }
  ```

### <a name="relative-yearly"></a><span data-ttu-id="23da3-220">相対年</span><span class="sxs-lookup"><span data-stu-id="23da3-220">Relative yearly</span></span>

<span data-ttu-id="23da3-221">相対年というパターンでは、次の予定までの年数に基づいて、特定の月の同じ相対位置にある同じ曜日にイベントが繰り返されます。</span><span class="sxs-lookup"><span data-stu-id="23da3-221">The relative yearly pattern causes an event to repeat on the same day of the week in the same relative position in a specific month, based on the number of years between each occurrence.</span></span> <span data-ttu-id="23da3-222">たとえば、「11 月の最後の水曜日」です。</span><span class="sxs-lookup"><span data-stu-id="23da3-222">For example, "every last Wednesday of November."</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="23da3-223">関連するプロパティ</span><span class="sxs-lookup"><span data-stu-id="23da3-223">Relevant properties</span></span>

| <span data-ttu-id="23da3-224">プロパティ</span><span class="sxs-lookup"><span data-stu-id="23da3-224">Property</span></span> | <span data-ttu-id="23da3-225">関連性</span><span class="sxs-lookup"><span data-stu-id="23da3-225">Relevance</span></span> | <span data-ttu-id="23da3-226">説明</span><span class="sxs-lookup"><span data-stu-id="23da3-226">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="23da3-227">**daysOfWeek**</span><span class="sxs-lookup"><span data-stu-id="23da3-227">**daysOfWeek**</span></span> | <span data-ttu-id="23da3-228">必須</span><span class="sxs-lookup"><span data-stu-id="23da3-228">Required</span></span> | <span data-ttu-id="23da3-229">イベントが発生することができる曜日を指定します。</span><span class="sxs-lookup"><span data-stu-id="23da3-229">Specifies on which day(s) of the week the event can occur.</span></span> <span data-ttu-id="23da3-230">相対年のイベントは、1 年に一度発生するため、複数の値が指定されている場合、イベントはパターンを満たす最初の日にあたります。</span><span class="sxs-lookup"><span data-stu-id="23da3-230">Relative yearly events only occur once per year, so if more than one value is specified, the event falls on the first day that satisfies the pattern.</span></span> |
| <span data-ttu-id="23da3-231">**index**</span><span class="sxs-lookup"><span data-stu-id="23da3-231">**index**</span></span> | <span data-ttu-id="23da3-232">省略可能</span><span class="sxs-lookup"><span data-stu-id="23da3-232">Optional</span></span> | <span data-ttu-id="23da3-233">月の最初のインスタンスから数えて、**daysOfsWeek** で指定された許可日数のどのインスタンスでイベントが発生するか指定します。</span><span class="sxs-lookup"><span data-stu-id="23da3-233">Specifies on which instance of the allowed days specified in **daysOfsWeek** the event occurs, counted from the first instance in the month.</span></span> <span data-ttu-id="23da3-234">使用可能な値: `first`、`second`、`third`、`fourth`、`last`。</span><span class="sxs-lookup"><span data-stu-id="23da3-234">Possible values: `first`, `second`, `third`, `fourth`, and `last`.</span></span> <span data-ttu-id="23da3-235">既定値: `first`。</span><span class="sxs-lookup"><span data-stu-id="23da3-235">Default value: `first`.</span></span> |
| <span data-ttu-id="23da3-236">**month**</span><span class="sxs-lookup"><span data-stu-id="23da3-236">**month**</span></span> | <span data-ttu-id="23da3-237">必須</span><span class="sxs-lookup"><span data-stu-id="23da3-237">Required</span></span> | <span data-ttu-id="23da3-238">イベントが発生する月を指定します。</span><span class="sxs-lookup"><span data-stu-id="23da3-238">Specifies in which month the event occurs.</span></span> |
| <span data-ttu-id="23da3-239">**interval**</span><span class="sxs-lookup"><span data-stu-id="23da3-239">**interval**</span></span> | <span data-ttu-id="23da3-240">必須</span><span class="sxs-lookup"><span data-stu-id="23da3-240">Required</span></span> | <span data-ttu-id="23da3-241">次の予定までの年数を指定します。</span><span class="sxs-lookup"><span data-stu-id="23da3-241">Specifies the number of years between each occurrence.</span></span> |
| <span data-ttu-id="23da3-242">**type**</span><span class="sxs-lookup"><span data-stu-id="23da3-242">**type**</span></span> | <span data-ttu-id="23da3-243">必須</span><span class="sxs-lookup"><span data-stu-id="23da3-243">Required</span></span> | <span data-ttu-id="23da3-244">`relativeYearly` に設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="23da3-244">Must be set to `relativeYearly`.</span></span> |

#### <a name="examples"></a><span data-ttu-id="23da3-245">例</span><span class="sxs-lookup"><span data-stu-id="23da3-245">Examples</span></span>

- <span data-ttu-id="23da3-246">毎年 11 月の最後の水曜日にこのイベントを繰り返す</span><span class="sxs-lookup"><span data-stu-id="23da3-246">Repeat this event on the last Wednesday of November every year</span></span>

  ```json
    "pattern": {
      "type": "relativeYearly",
      "interval": 1,
      "daysOfWeek": [ "Wednesday" ],
      "index": "last",
      "month": 11
    }
  ```

## <a name="recurrence-ranges"></a><span data-ttu-id="23da3-247">繰り返し範囲</span><span class="sxs-lookup"><span data-stu-id="23da3-247">Recurrence ranges</span></span>

<span data-ttu-id="23da3-248">繰り返しの第 2 の部分は範囲です。</span><span class="sxs-lookup"><span data-stu-id="23da3-248">The second part of a recurrence is the range.</span></span> <span data-ttu-id="23da3-249">パターンが繰り返される期間を指定します。</span><span class="sxs-lookup"><span data-stu-id="23da3-249">This specifies how long the pattern repeats.</span></span> <span data-ttu-id="23da3-250">たとえば、イベントは、10 回出現したら終了する、特定の日付で終了する、または終了しないというように設定できます。</span><span class="sxs-lookup"><span data-stu-id="23da3-250">For example, an event could end after 10 occurrences, by a specific date, or could have no end.</span></span> <span data-ttu-id="23da3-251">範囲は、API の [recurrenceRange リソース](/graph/api/resources/recurrencepattern?view=graph-rest-1.0)で表されます。</span><span class="sxs-lookup"><span data-stu-id="23da3-251">A range is represented in the API by the [recurrenceRange resource](/graph/api/resources/recurrencepattern?view=graph-rest-1.0).</span></span>

<span data-ttu-id="23da3-252">範囲の種類に応じて、**recurrenceRange** の特定のフィールドは、必須になるか、または無視されます。</span><span class="sxs-lookup"><span data-stu-id="23da3-252">Depending on the type of range, certain fields of **recurrenceRange** are required or ignored.</span></span>

> <span data-ttu-id="23da3-253">**注**: フィールドが無視される場合でも、検証は行われます。</span><span class="sxs-lookup"><span data-stu-id="23da3-253">**Note**: Even if a field is ignored, it is still validated.</span></span> <span data-ttu-id="23da3-254">使用可能な値のセット リストがフィールドに含まれる場合、そのフィールドが無視されても、許可されたセットの範囲外の値を使用するとエラーが発生します。</span><span class="sxs-lookup"><span data-stu-id="23da3-254">If a field has a set list of possible values, using a value outside the allowed set causes an error, even if that field is ignored.</span></span>

<span data-ttu-id="23da3-255">使用可能な範囲の種類を見てみましょう。</span><span class="sxs-lookup"><span data-stu-id="23da3-255">Let's take a look at each of the possible range types.</span></span>

### <a name="numbered-range"></a><span data-ttu-id="23da3-256">番号付き範囲</span><span class="sxs-lookup"><span data-stu-id="23da3-256">Numbered range</span></span>

<span data-ttu-id="23da3-257">番号付き範囲により、イベントは開始日から固定した回数、パターンに基づいて発生します。</span><span class="sxs-lookup"><span data-stu-id="23da3-257">The numbered range causes an event to occur a fixed number of times (based on the pattern) from a start date.</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="23da3-258">関連するプロパティ</span><span class="sxs-lookup"><span data-stu-id="23da3-258">Relevant properties</span></span>

| <span data-ttu-id="23da3-259">プロパティ</span><span class="sxs-lookup"><span data-stu-id="23da3-259">Property</span></span> | <span data-ttu-id="23da3-260">関連性</span><span class="sxs-lookup"><span data-stu-id="23da3-260">Relevance</span></span> | <span data-ttu-id="23da3-261">説明</span><span class="sxs-lookup"><span data-stu-id="23da3-261">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="23da3-262">**numberOfOccurences**</span><span class="sxs-lookup"><span data-stu-id="23da3-262">**numberOfOccurences**</span></span> | <span data-ttu-id="23da3-263">必須</span><span class="sxs-lookup"><span data-stu-id="23da3-263">Required</span></span> | <span data-ttu-id="23da3-264">発生回数を指定します。</span><span class="sxs-lookup"><span data-stu-id="23da3-264">Specifies the number of occurrences.</span></span> <span data-ttu-id="23da3-265">正の整数であることが必要です。</span><span class="sxs-lookup"><span data-stu-id="23da3-265">Must be a positive integer.</span></span> |
| <span data-ttu-id="23da3-266">**recurrenceTimeZone**</span><span class="sxs-lookup"><span data-stu-id="23da3-266">**recurrenceTimeZone**</span></span> | <span data-ttu-id="23da3-267">省略可能</span><span class="sxs-lookup"><span data-stu-id="23da3-267">Optional</span></span> | <span data-ttu-id="23da3-268">**startDate** プロパティのタイム ゾーンを指定します。</span><span class="sxs-lookup"><span data-stu-id="23da3-268">Specifies the time zone for the **startDate** property.</span></span> <span data-ttu-id="23da3-269">指定しない場合は、イベントのタイム ゾーンが使用されます。</span><span class="sxs-lookup"><span data-stu-id="23da3-269">If not specified, the time zone of the event is used.</span></span> |
| <span data-ttu-id="23da3-270">**startDate**</span><span class="sxs-lookup"><span data-stu-id="23da3-270">**startDate**</span></span> | <span data-ttu-id="23da3-271">必須</span><span class="sxs-lookup"><span data-stu-id="23da3-271">Required</span></span> | <span data-ttu-id="23da3-272">パターンの適用を開始する日付を指定します。</span><span class="sxs-lookup"><span data-stu-id="23da3-272">Specifies the date to start applying the pattern.</span></span> <span data-ttu-id="23da3-273">**startDate** の値は、[イベント リソース](/graph/api/resources/event?view=graph-rest-1.0)の **start** プロパティの日付値に対応している必要があります。</span><span class="sxs-lookup"><span data-stu-id="23da3-273">The value of **startDate** MUST correspond to the date value of the **start** property on the [event resource](/graph/api/resources/event?view=graph-rest-1.0).</span></span> <span data-ttu-id="23da3-274">パターンと一致しない場合、会議の最初の回はこの日付には発生しないことにご注意ください。</span><span class="sxs-lookup"><span data-stu-id="23da3-274">Note that the first occurrence of the meeting may not occur on this date if it does not fit the pattern.</span></span> |
| <span data-ttu-id="23da3-275">**type**</span><span class="sxs-lookup"><span data-stu-id="23da3-275">**type**</span></span> | <span data-ttu-id="23da3-276">必須</span><span class="sxs-lookup"><span data-stu-id="23da3-276">Required</span></span> | <span data-ttu-id="23da3-277">`numbered` に設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="23da3-277">Must be set to `numbered`.</span></span> |

#### <a name="examples"></a><span data-ttu-id="23da3-278">例</span><span class="sxs-lookup"><span data-stu-id="23da3-278">Examples</span></span>

- <span data-ttu-id="23da3-279">このイベントを 10 回繰り返す</span><span class="sxs-lookup"><span data-stu-id="23da3-279">Repeat this event 10 times</span></span>

  ```json
    "range": {
      "type": "numbered",
      "startDate": "2017-04-02",
      "numberOfOccurrences": 10
    }
  ```

### <a name="end-date-range"></a><span data-ttu-id="23da3-280">終了日の範囲</span><span class="sxs-lookup"><span data-stu-id="23da3-280">End date range</span></span>

<span data-ttu-id="23da3-281">終了日の範囲を設定すると、開始日から終了日まで適用可能なパターンに適合するすべての日でイベントが発生します。</span><span class="sxs-lookup"><span data-stu-id="23da3-281">The end date range causes an event to occur on all days that fit the applicable pattern between a start date and an end date.</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="23da3-282">関連するプロパティ</span><span class="sxs-lookup"><span data-stu-id="23da3-282">Relevant properties</span></span>

| <span data-ttu-id="23da3-283">プロパティ</span><span class="sxs-lookup"><span data-stu-id="23da3-283">Property</span></span> | <span data-ttu-id="23da3-284">関連性</span><span class="sxs-lookup"><span data-stu-id="23da3-284">Relevance</span></span> | <span data-ttu-id="23da3-285">説明</span><span class="sxs-lookup"><span data-stu-id="23da3-285">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="23da3-286">**endDate**</span><span class="sxs-lookup"><span data-stu-id="23da3-286">**endDate**</span></span> | <span data-ttu-id="23da3-287">必須</span><span class="sxs-lookup"><span data-stu-id="23da3-287">Required</span></span> | <span data-ttu-id="23da3-288">パターンの適用を停止する日付を指定します。</span><span class="sxs-lookup"><span data-stu-id="23da3-288">Specifies the date to stop applying the pattern.</span></span> <span data-ttu-id="23da3-289">パターンと一致しない場合、会議の最後の回はこの日付には発生しないことにご注意ください。</span><span class="sxs-lookup"><span data-stu-id="23da3-289">Note that the last occurrence of the meeting may not occur on this date if it does not fit the pattern.</span></span> |
| <span data-ttu-id="23da3-290">**recurrenceTimeZone**</span><span class="sxs-lookup"><span data-stu-id="23da3-290">**recurrenceTimeZone**</span></span> | <span data-ttu-id="23da3-291">省略可能</span><span class="sxs-lookup"><span data-stu-id="23da3-291">Optional</span></span> | <span data-ttu-id="23da3-292">**startDate** プロパティと **endDate** プロパティのタイム ゾーンを指定します。</span><span class="sxs-lookup"><span data-stu-id="23da3-292">Specifies the time zone for the **startDate** and **endDate** properties.</span></span> <span data-ttu-id="23da3-293">指定しない場合は、イベントのタイム ゾーンが使用されます。</span><span class="sxs-lookup"><span data-stu-id="23da3-293">If not specified, the time zone of the event is used.</span></span> |
| <span data-ttu-id="23da3-294">**startDate**</span><span class="sxs-lookup"><span data-stu-id="23da3-294">**startDate**</span></span> | <span data-ttu-id="23da3-295">必須</span><span class="sxs-lookup"><span data-stu-id="23da3-295">Required</span></span> | <span data-ttu-id="23da3-296">パターンの適用を開始する日付を指定します。</span><span class="sxs-lookup"><span data-stu-id="23da3-296">Specifies the date to start applying the pattern.</span></span> <span data-ttu-id="23da3-297">**startDate** の値は、[イベント リソース](/graph/api/resources/event?view=graph-rest-1.0)の **start** プロパティの日付値に対応している必要があります。</span><span class="sxs-lookup"><span data-stu-id="23da3-297">The value of **startDate** MUST correspond to the date value of the **start** property on the [event resource](/graph/api/resources/event?view=graph-rest-1.0).</span></span> <span data-ttu-id="23da3-298">パターンと一致しない場合、会議の最初の回はこの日付には発生しないことにご注意ください。</span><span class="sxs-lookup"><span data-stu-id="23da3-298">Note that the first occurrence of the meeting may not occur on this date if it does not fit the pattern.</span></span> |
| <span data-ttu-id="23da3-299">**type**</span><span class="sxs-lookup"><span data-stu-id="23da3-299">**type**</span></span> | <span data-ttu-id="23da3-300">必須</span><span class="sxs-lookup"><span data-stu-id="23da3-300">Required</span></span> | <span data-ttu-id="23da3-301">**endDate** に設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="23da3-301">Must be set to **endDate**.</span></span> |

#### <a name="examples"></a><span data-ttu-id="23da3-302">例</span><span class="sxs-lookup"><span data-stu-id="23da3-302">Examples</span></span>

- <span data-ttu-id="23da3-303">2017 年 7 月 1 日から 2017 年 7 月 31 日までこのイベントを繰り返す</span><span class="sxs-lookup"><span data-stu-id="23da3-303">Repeat this event from July 1, 2017, to July 31, 2017</span></span>

  ```json
    "range": {
      "type": "endDate",
      "startDate": "2017-07-01",
      "endDate": "2017-07-31"
    }
  ```

### <a name="no-end-range"></a><span data-ttu-id="23da3-304">終了範囲なし</span><span class="sxs-lookup"><span data-stu-id="23da3-304">No end range</span></span>

<span data-ttu-id="23da3-305">終了範囲なしに設定すると、開始日以降の適用可能なパターンに適合するすべての日でイベントが発生します。</span><span class="sxs-lookup"><span data-stu-id="23da3-305">The no end range causes an event to occur on all days that fit the applicable pattern after a start date.</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="23da3-306">関連するプロパティ</span><span class="sxs-lookup"><span data-stu-id="23da3-306">Relevant properties</span></span>

| <span data-ttu-id="23da3-307">プロパティ</span><span class="sxs-lookup"><span data-stu-id="23da3-307">Property</span></span> | <span data-ttu-id="23da3-308">関連性</span><span class="sxs-lookup"><span data-stu-id="23da3-308">Relevance</span></span> | <span data-ttu-id="23da3-309">説明</span><span class="sxs-lookup"><span data-stu-id="23da3-309">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="23da3-310">**recurrenceTimeZone**</span><span class="sxs-lookup"><span data-stu-id="23da3-310">**recurrenceTimeZone**</span></span> | <span data-ttu-id="23da3-311">省略可能</span><span class="sxs-lookup"><span data-stu-id="23da3-311">Optional</span></span> | <span data-ttu-id="23da3-312">**startDate** プロパティのタイム ゾーンを指定します。</span><span class="sxs-lookup"><span data-stu-id="23da3-312">Specifies the time zone for the **startDate** property.</span></span> <span data-ttu-id="23da3-313">指定しない場合は、イベントのタイム ゾーンが使用されます。</span><span class="sxs-lookup"><span data-stu-id="23da3-313">If not specified, the time zone of the event is used.</span></span> |
| <span data-ttu-id="23da3-314">**startDate**</span><span class="sxs-lookup"><span data-stu-id="23da3-314">**startDate**</span></span> | <span data-ttu-id="23da3-315">必須</span><span class="sxs-lookup"><span data-stu-id="23da3-315">Required</span></span> | <span data-ttu-id="23da3-316">パターンの適用を開始する日付を指定します。</span><span class="sxs-lookup"><span data-stu-id="23da3-316">Specifies the date to start applying the pattern.</span></span> <span data-ttu-id="23da3-317">**startDate** の値は、[イベント リソース](/graph/api/resources/event?view=graph-rest-1.0)の **start** プロパティの日付値に対応している必要があります。</span><span class="sxs-lookup"><span data-stu-id="23da3-317">The value of **startDate** MUST correspond to the date value of the **start** property on the [event resource](/graph/api/resources/event?view=graph-rest-1.0).</span></span> <span data-ttu-id="23da3-318">パターンと一致しない場合、会議の最初の回はこの日付には発生しないことにご注意ください。</span><span class="sxs-lookup"><span data-stu-id="23da3-318">Note that the first occurrence of the meeting may not occur on this date if it does not fit the pattern.</span></span> |
| <span data-ttu-id="23da3-319">**type**</span><span class="sxs-lookup"><span data-stu-id="23da3-319">**type**</span></span> | <span data-ttu-id="23da3-320">必須</span><span class="sxs-lookup"><span data-stu-id="23da3-320">Required</span></span> | <span data-ttu-id="23da3-321">`noEnd` に設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="23da3-321">Must be set to `noEnd`.</span></span> |

#### <a name="examples"></a><span data-ttu-id="23da3-322">例</span><span class="sxs-lookup"><span data-stu-id="23da3-322">Examples</span></span>

- <span data-ttu-id="23da3-323">2017 年 5 月 15 日から永遠にこのイベントを繰り返す</span><span class="sxs-lookup"><span data-stu-id="23da3-323">Repeat this event from May 15, 2017, forever</span></span>

  ```json
    "range": {
      "type": "noEnd",
      "startDate": "2017-05-15"
    }
  ```

## <a name="using-patterns-and-ranges-to-create-recurring-events"></a><span data-ttu-id="23da3-324">パターンおよび範囲を使用して繰り返しイベントを作成する</span><span class="sxs-lookup"><span data-stu-id="23da3-324">Using patterns and ranges to create recurring events</span></span>

<span data-ttu-id="23da3-325">これまでは、パターンと範囲について別々に考えてきました。次に、パターンと範囲がどのように連携し、イベントの **start** プロパティおよび **end** プロパティとどのようにやり取りするかを見てみましょう。</span><span class="sxs-lookup"><span data-stu-id="23da3-325">Now that we've looked at patterns and ranges separately, let's look at how they work together and how they interact with the **start** and **end** properties on the event.</span></span>

### <a name="creating-a-recurrence-rule"></a><span data-ttu-id="23da3-326">繰り返しルールの作成</span><span class="sxs-lookup"><span data-stu-id="23da3-326">Creating a recurrence rule</span></span>

<span data-ttu-id="23da3-327">繰り返しルールを作成するには、パターンと範囲の両方を指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="23da3-327">To create a recurrence rule, you must specify both a pattern and a range.</span></span> <span data-ttu-id="23da3-328">どのパターンの種類も、任意の範囲の種類で使用できます。</span><span class="sxs-lookup"><span data-stu-id="23da3-328">Any pattern type can work with any range type.</span></span> <span data-ttu-id="23da3-329">次にいくつかの例を示します。</span><span class="sxs-lookup"><span data-stu-id="23da3-329">Here are a few examples.</span></span>

#### <a name="examples"></a><span data-ttu-id="23da3-330">例</span><span class="sxs-lookup"><span data-stu-id="23da3-330">Examples</span></span>

- <span data-ttu-id="23da3-331">**2017 年 9 月 4 日から年末までの期間、毎週月曜日の午後 1 時から午後 1 時 30 分まで会合する**</span><span class="sxs-lookup"><span data-stu-id="23da3-331">**Meet from 1:00 PM to 1:30 PM every Monday starting September 4, 2017, until the end of the year**</span></span>

  - <span data-ttu-id="23da3-332">「毎週月曜日」という要件については、`weekly` 繰り返しパターンの種類で簡単に対応できます。</span><span class="sxs-lookup"><span data-stu-id="23da3-332">The "every Monday" requirement is easily met by the `weekly` recurrence pattern type.</span></span>
  - <span data-ttu-id="23da3-333">「年末まで」という要件は、`endDate` 繰り返し範囲の種類を示しています。</span><span class="sxs-lookup"><span data-stu-id="23da3-333">The "until the end of the year" requirement indicates an `endDate` recurrence range type.</span></span>

  ```json
    "recurrence": {
      "pattern": {
        "type": "weekly",
        "interval": 1,
        "daysOfWeek": [ "Monday" ]
      },
      "range": {
        "type": "endDate",
        "startDate": "2017-09-04",
        "endDate": "2017-12-31"
      }
    }
  ```

  <span data-ttu-id="23da3-334">2017 年 12 月 31 日が日曜日のため、このシリーズの最後の回は 12 月 25 日月曜日になります。</span><span class="sxs-lookup"><span data-stu-id="23da3-334">Because December 31, 2017, is on a Sunday, the last occurrence in this series will be on Monday, December 25.</span></span>

- <span data-ttu-id="23da3-335">**2017 年 8 月 29 日から、隔月の最初の木曜日の午後 2 時から午後 3 時まで会合する**</span><span class="sxs-lookup"><span data-stu-id="23da3-335">**Meet from 2:00 PM to 3:00 PM on the first Thursday of every other month starting August 29, 2017**</span></span>

  - <span data-ttu-id="23da3-336">「隔月の最初の木曜日」という要件は、相対月パターンを使用して実現できます。</span><span class="sxs-lookup"><span data-stu-id="23da3-336">The "first Thursday of every other month" requirement is achievable by using a relative monthly pattern.</span></span> <span data-ttu-id="23da3-337">「隔月」の部分は、**interval** を `2` に設定する必要があることを示しています。</span><span class="sxs-lookup"><span data-stu-id="23da3-337">The "every other month" portion indicates that the **interval** should be set to `2`.</span></span>
  - <span data-ttu-id="23da3-338">終了日については要件が存在しないため、`noEnd` 範囲の種類を使用することができます。</span><span class="sxs-lookup"><span data-stu-id="23da3-338">Because there is no requirement on an end date, a `noEnd` range type can be used.</span></span>

  ```json
    "recurrence": {
      "pattern": {
        "type": "relativeMonthly",
        "interval": 2,
        "daysOfWeek": [ "Thursday" ],
        "index": "first"
      },
      "range": {
        "type": "noEnd",
        "startDate": "2017-08-29"
      }
    }
  ```

  <span data-ttu-id="23da3-339">**startDate** の値が 8 月の最初の木曜日を過ぎているため、このシリーズの最初の回は 9 月になります。</span><span class="sxs-lookup"><span data-stu-id="23da3-339">Because the value of **startDate** is after the first Thursday in August, the first occurrence of this series will be in September.</span></span>

## <a name="next-steps"></a><span data-ttu-id="23da3-340">次のステップ</span><span class="sxs-lookup"><span data-stu-id="23da3-340">Next steps</span></span>
    
<span data-ttu-id="23da3-341">詳細については、「[Outlook カレンダーとの統合](outlook-calendar-concept-overview.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="23da3-341">Find out more about [integrating with Outlook calendar](outlook-calendar-concept-overview.md).</span></span>
