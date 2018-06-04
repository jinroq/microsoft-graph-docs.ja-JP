# <a name="schedule-repeating-appointments-as-recurring-events-in-outlook"></a><span data-ttu-id="c34b5-101">定期的に繰り返される予定を、Outlook で定期的なイベントとして設定する</span><span class="sxs-lookup"><span data-stu-id="c34b5-101">Schedule repeating appointments as recurring events in Outlook</span></span>

<span data-ttu-id="c34b5-102">繰り返しイベントは、Outlook カレンダーの重要な部分です。</span><span class="sxs-lookup"><span data-stu-id="c34b5-102">Recurring events are an important part of Outlook calendaring.</span></span> <span data-ttu-id="c34b5-103">毎週行う上司との個別の打ち合わせや毎月第 2 火曜日に行われる部門全体のレビュー会議などの繰り返しイベントでは、イベントを一度作成するだけで、シリーズの残りの部分はサーバーによって入力されます。</span><span class="sxs-lookup"><span data-stu-id="c34b5-103">Whether it's a weekly one-on-one meeting with your manager, or a division-wide review meeting that happens on the second Tuesday of each month, recurring events make it easy to create the event once, and let the server fill in the rest of the series.</span></span>

<span data-ttu-id="c34b5-104">繰り返しイベントを個々の予定に「拡張」するための情報のキー ビットとなるものが繰り返しルールです。</span><span class="sxs-lookup"><span data-stu-id="c34b5-104">The key bit of information that allows recurring events to "expand" into individual occurrences is the recurrence rule.</span></span> <span data-ttu-id="c34b5-105">このルールは、イベントを繰り返す頻度と期間の両方を指定します。</span><span class="sxs-lookup"><span data-stu-id="c34b5-105">The rule specifies both how often an event repeats, and for how long.</span></span> <span data-ttu-id="c34b5-106">Outlook REST API は、[イベント リソース](../api-reference/v1.0/resources/event.md)の**recurrence**プロパティで繰り返しルールをモデル化します。</span><span class="sxs-lookup"><span data-stu-id="c34b5-106">The Outlook REST APIs model recurrence rules in the **** property of the [event resource](../api-reference/v1.0/resources/event.md).</span></span> 

<span data-ttu-id="c34b5-107">それぞれのパターンは、繰り返しパターン (頻度) と繰り返し範囲 (期間) の 2 つの部分で構成されます。</span><span class="sxs-lookup"><span data-stu-id="c34b5-107">Each  is made up of two parts: the recurrence pattern (how often), and the recurrence range (for how long).</span></span>

## <a name="recurrence-patterns"></a><span data-ttu-id="c34b5-108">繰り返しパターン</span><span class="sxs-lookup"><span data-stu-id="c34b5-108">Recurrence patterns</span></span>

<span data-ttu-id="c34b5-109">繰り返しの第 1 の部分は、パターンです。</span><span class="sxs-lookup"><span data-stu-id="c34b5-109">The first part of a recurrence is the pattern.</span></span> <span data-ttu-id="c34b5-110">これは、イベントを繰り返す頻度を指定します。</span><span class="sxs-lookup"><span data-stu-id="c34b5-110">This specifies how often the event repeats.</span></span> <span data-ttu-id="c34b5-111">たとえば、イベントを「3 日ごと」、「毎週木曜日」、または「毎年 7 月 22 日」に繰り返すことができます。</span><span class="sxs-lookup"><span data-stu-id="c34b5-111">For example, an event could repeat "every 3 days", "every Thursday", or "on July 22 every year".</span></span> <span data-ttu-id="c34b5-112">パターンは、API の [recurrencePattern リソース](../api-reference/v1.0/resources/recurrencepattern.md)で表されます。</span><span class="sxs-lookup"><span data-stu-id="c34b5-112">A pattern is represented in the API by the [recurrencePattern resource](../api-reference/v1.0/resources/recurrencepattern.md).</span></span>

<span data-ttu-id="c34b5-113">パターンの種類に応じて、**recurrencePattern**の特定のフィールドは、必須、オプションになるか、または無視されます。</span><span class="sxs-lookup"><span data-stu-id="c34b5-113">Depending on the type of pattern, certain fields of the **** are required, optional, or ignored.</span></span>

> <span data-ttu-id="c34b5-114">**注**: フィールドが無視される場合でも、検証は行われます。</span><span class="sxs-lookup"><span data-stu-id="c34b5-114">Even if a field is ignored, it is still validated.</span></span> <span data-ttu-id="c34b5-115">使用可能な値のセット リストがフィールドに含まれる場合、そのフィールドが無視されても、許可されたセットの範囲外の値を使用するとエラーが発生します。</span><span class="sxs-lookup"><span data-stu-id="c34b5-115">If a field has a set list of possible values, using a value outside the allowed set will cause an error, even if that field is ignored.</span></span>

<span data-ttu-id="c34b5-116">使用可能なパターンの種類を見てみましょう。</span><span class="sxs-lookup"><span data-stu-id="c34b5-116">Let's take a look at each of the possible pattern types.</span></span>

### <a name="daily"></a><span data-ttu-id="c34b5-117">Daily (日単位)</span><span class="sxs-lookup"><span data-stu-id="c34b5-117">Daily</span></span>

<span data-ttu-id="c34b5-118">Daily (日単位) の繰り返しパターンでは、次の予定までの日数に基づいてイベントが繰り返されます。</span><span class="sxs-lookup"><span data-stu-id="c34b5-118">The daily recurrence pattern causes an event to repeat based on a number of days between each occurrence.</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="c34b5-119">関連するプロパティ</span><span class="sxs-lookup"><span data-stu-id="c34b5-119">Relevant properties</span></span>

| <span data-ttu-id="c34b5-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c34b5-120">Property</span></span> | <span data-ttu-id="c34b5-121">関連性</span><span class="sxs-lookup"><span data-stu-id="c34b5-121">Relevance</span></span> | <span data-ttu-id="c34b5-122">説明</span><span class="sxs-lookup"><span data-stu-id="c34b5-122">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="c34b5-123">**interval**</span><span class="sxs-lookup"><span data-stu-id="c34b5-123">**interval**</span></span> | <span data-ttu-id="c34b5-124">必須</span><span class="sxs-lookup"><span data-stu-id="c34b5-124">Required</span></span> | <span data-ttu-id="c34b5-125">次の予定までの日数を指定します。</span><span class="sxs-lookup"><span data-stu-id="c34b5-125">Specifies the number of days between each occurrence.</span></span> |
| <span data-ttu-id="c34b5-126">**type**</span><span class="sxs-lookup"><span data-stu-id="c34b5-126">**type**</span></span> | <span data-ttu-id="c34b5-127">必須</span><span class="sxs-lookup"><span data-stu-id="c34b5-127">Required</span></span> | <span data-ttu-id="c34b5-128">`daily` に設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="c34b5-128">Must be set to `daily`.</span></span> |

#### <a name="examples"></a><span data-ttu-id="c34b5-129">例</span><span class="sxs-lookup"><span data-stu-id="c34b5-129">Examples</span></span>

- <span data-ttu-id="c34b5-130">このイベントを毎日繰り返す</span><span class="sxs-lookup"><span data-stu-id="c34b5-130">Repeat this event every day</span></span>

  ```json
    "pattern": {
      "type": "daily",
      "interval": 1
    }
  ```
- <span data-ttu-id="c34b5-131">このイベントを 3 日おきに繰り返す</span><span class="sxs-lookup"><span data-stu-id="c34b5-131">Repeat this event every three days</span></span>

  ```json
    "pattern": {
      "type": "daily",
      "interval": 3
    }
  ```

### <a name="weekly"></a><span data-ttu-id="c34b5-132">Weekly (週単位)</span><span class="sxs-lookup"><span data-stu-id="c34b5-132">Weekly</span></span>

<span data-ttu-id="c34b5-133">Weekly (週単位) の定期的なパターンでは、次の予定セットまでの週数に基づいて、同じ曜日 (複数の曜日も可) にイベントが繰り返されます。</span><span class="sxs-lookup"><span data-stu-id="c34b5-133">The weekly recurrence pattern causes an event to repeat on the same day or days of the week, based on the number of weeks between each set of occurrences.</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="c34b5-134">関連するプロパティ</span><span class="sxs-lookup"><span data-stu-id="c34b5-134">Relevant properties</span></span>

| <span data-ttu-id="c34b5-135">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c34b5-135">Property</span></span> | <span data-ttu-id="c34b5-136">関連性</span><span class="sxs-lookup"><span data-stu-id="c34b5-136">Relevance</span></span> | <span data-ttu-id="c34b5-137">説明</span><span class="sxs-lookup"><span data-stu-id="c34b5-137">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="c34b5-138">**daysOfWeek**</span><span class="sxs-lookup"><span data-stu-id="c34b5-138">**daysOfWeek**</span></span> | <span data-ttu-id="c34b5-139">必須</span><span class="sxs-lookup"><span data-stu-id="c34b5-139">Required</span></span> | <span data-ttu-id="c34b5-140">イベントが発生する曜日 (複数可) を指定します。</span><span class="sxs-lookup"><span data-stu-id="c34b5-140">Specifies on which day(s) of the week the event occurs.</span></span> |
| <span data-ttu-id="c34b5-141">**firstDayOfWeek**</span><span class="sxs-lookup"><span data-stu-id="c34b5-141">**FirstDayOfWeek**</span></span> | <span data-ttu-id="c34b5-142">省略可能</span><span class="sxs-lookup"><span data-stu-id="c34b5-142">Optional</span></span> | <span data-ttu-id="c34b5-143">週の最初の曜日となる日を指定します。</span><span class="sxs-lookup"><span data-stu-id="c34b5-143">Specifies which day is considered the first day of the week.</span></span> <span data-ttu-id="c34b5-144">既定値: `Sunday`。</span><span class="sxs-lookup"><span data-stu-id="c34b5-144">Default value: `Sunday`.</span></span> |
| <span data-ttu-id="c34b5-145">**interval**</span><span class="sxs-lookup"><span data-stu-id="c34b5-145">**interval**</span></span> | <span data-ttu-id="c34b5-146">必須</span><span class="sxs-lookup"><span data-stu-id="c34b5-146">Required</span></span> | <span data-ttu-id="c34b5-147">次の予定までの週数を指定します。</span><span class="sxs-lookup"><span data-stu-id="c34b5-147">Specifies the number of weeks between each set of occurrences.</span></span> |
| <span data-ttu-id="c34b5-148">**type**</span><span class="sxs-lookup"><span data-stu-id="c34b5-148">**type**</span></span> | <span data-ttu-id="c34b5-149">必須</span><span class="sxs-lookup"><span data-stu-id="c34b5-149">Required</span></span> | <span data-ttu-id="c34b5-150">`weekly` に設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="c34b5-150">Must be set to `weekly`.</span></span> |

#### <a name="examples"></a><span data-ttu-id="c34b5-151">例</span><span class="sxs-lookup"><span data-stu-id="c34b5-151">Examples</span></span>

- <span data-ttu-id="c34b5-152">このイベントを毎週木曜日に繰り返す</span><span class="sxs-lookup"><span data-stu-id="c34b5-152">Repeat this event every Thursday</span></span>

  ```json
    "pattern": {
      "type": "weekly",
      "interval": 1,
      "daysOfWeek": [ "Thursday" ]
    }
  ```
- <span data-ttu-id="c34b5-153">このイベントを隔週の月曜日と火曜日に繰り返す</span><span class="sxs-lookup"><span data-stu-id="c34b5-153">Repeat this event every other Monday and Tuesday</span></span>

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

### <a name="absolute-monthly"></a><span data-ttu-id="c34b5-154">絶対月</span><span class="sxs-lookup"><span data-stu-id="c34b5-154">Absolute monthly</span></span>

<span data-ttu-id="c34b5-155">絶対月というパターンでは、次の予定までの月数に基づいて月の同じ日 (たとえば、15 日) にイベントが繰り返されます。</span><span class="sxs-lookup"><span data-stu-id="c34b5-155">The absolute monthly pattern causes an event to repeat on the same day of the month (e.g. the 15th), based on the number of months between each occurrence.</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="c34b5-156">関連するプロパティ</span><span class="sxs-lookup"><span data-stu-id="c34b5-156">Relevant properties</span></span>

| <span data-ttu-id="c34b5-157">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c34b5-157">Property</span></span> | <span data-ttu-id="c34b5-158">関連性</span><span class="sxs-lookup"><span data-stu-id="c34b5-158">Relevance</span></span> | <span data-ttu-id="c34b5-159">説明</span><span class="sxs-lookup"><span data-stu-id="c34b5-159">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="c34b5-160">**dayOfMonth**</span><span class="sxs-lookup"><span data-stu-id="c34b5-160">**dayOfMonth**</span></span> | <span data-ttu-id="c34b5-161">必須</span><span class="sxs-lookup"><span data-stu-id="c34b5-161">Required</span></span> | <span data-ttu-id="c34b5-162">イベントが発生する月の日付を指定します。</span><span class="sxs-lookup"><span data-stu-id="c34b5-162">Specifies on which day of the month the event occurs.</span></span> |
| <span data-ttu-id="c34b5-163">**interval**</span><span class="sxs-lookup"><span data-stu-id="c34b5-163">**interval**</span></span> | <span data-ttu-id="c34b5-164">必須</span><span class="sxs-lookup"><span data-stu-id="c34b5-164">Required</span></span> | <span data-ttu-id="c34b5-165">次の予定までの月数を指定します。</span><span class="sxs-lookup"><span data-stu-id="c34b5-165">Specifies the number of months between each occurrence.</span></span> |
| <span data-ttu-id="c34b5-166">**type**</span><span class="sxs-lookup"><span data-stu-id="c34b5-166">**type**</span></span> | <span data-ttu-id="c34b5-167">必須</span><span class="sxs-lookup"><span data-stu-id="c34b5-167">Required</span></span> | <span data-ttu-id="c34b5-168">`absoluteMonthly` に設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="c34b5-168">Must be set to `absoluteMonthly`.</span></span> |

#### <a name="examples"></a><span data-ttu-id="c34b5-169">例</span><span class="sxs-lookup"><span data-stu-id="c34b5-169">Examples</span></span>

- <span data-ttu-id="c34b5-170">毎月 15 日にこのイベントを繰り返す</span><span class="sxs-lookup"><span data-stu-id="c34b5-170">Repeat this event on the 15th of every month</span></span>

  ```json
    "pattern": {
      "type": "absoluteMonthly",
      "interval": 1,
      "dayOfMonth": 15
    }
  ```
- <span data-ttu-id="c34b5-171">四半期 (3 か月ごと) の 7 日にこのイベントを繰り返す</span><span class="sxs-lookup"><span data-stu-id="c34b5-171">Repeat this event quarterly (every 3 months) on the 7th</span></span>

  ```json
    "pattern": {
      "type": "absoluteMonthly",
      "interval": 3,
      "dayOfMonth": 7
    }
  ```

### <a name="relative-monthly"></a><span data-ttu-id="c34b5-172">相対月</span><span class="sxs-lookup"><span data-stu-id="c34b5-172">Relative monthly</span></span>

<span data-ttu-id="c34b5-173">相対月というパターンでは、次の予定までの月数に基づいて、月の同じ相対位置にある同じ曜日にイベントが繰り返されます。</span><span class="sxs-lookup"><span data-stu-id="c34b5-173">The relative monthly pattern causes an event to repeat on the same day of the week in the same relative position in the month, based on the number of months between each occurrence.</span></span> <span data-ttu-id="c34b5-174">たとえば、「毎月第 2 水曜日」です。</span><span class="sxs-lookup"><span data-stu-id="c34b5-174">For example, "every second Wednesday of the month".</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="c34b5-175">関連するプロパティ</span><span class="sxs-lookup"><span data-stu-id="c34b5-175">Relevant properties</span></span>

| <span data-ttu-id="c34b5-176">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c34b5-176">Property</span></span> | <span data-ttu-id="c34b5-177">関連性</span><span class="sxs-lookup"><span data-stu-id="c34b5-177">Relevance</span></span> | <span data-ttu-id="c34b5-178">説明</span><span class="sxs-lookup"><span data-stu-id="c34b5-178">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="c34b5-179">**daysOfWeek**</span><span class="sxs-lookup"><span data-stu-id="c34b5-179">**daysOfWeek**</span></span> | <span data-ttu-id="c34b5-180">必須</span><span class="sxs-lookup"><span data-stu-id="c34b5-180">Required</span></span> | <span data-ttu-id="c34b5-181">イベントが発生することができる曜日を指定します。</span><span class="sxs-lookup"><span data-stu-id="c34b5-181">Specifies on which day(s) of the week the event can occur.</span></span> <span data-ttu-id="c34b5-182">相対月のイベントは、1 か月に一度発生するため、複数の値が指定されている場合、イベントはパターンを満たす最初の日にあたります。</span><span class="sxs-lookup"><span data-stu-id="c34b5-182">Relative monthly events only occur once per month, so if more than one value is specified, the event falls on the first day that satisfies the pattern.</span></span> |
| <span data-ttu-id="c34b5-183">**index**</span><span class="sxs-lookup"><span data-stu-id="c34b5-183">**index**</span></span> | <span data-ttu-id="c34b5-184">省略可能</span><span class="sxs-lookup"><span data-stu-id="c34b5-184">Optional</span></span> | <span data-ttu-id="c34b5-185">月の最初のインスタンスから数えて、**daysOfsWeek** で指定された許可日数のどのインスタンスでイベントが発生するか指定します。</span><span class="sxs-lookup"><span data-stu-id="c34b5-185">Specifies on which instance of the allowed days specified in **daysOfsWeek** the event occurs, counted from the first instance in the month.</span></span> <span data-ttu-id="c34b5-186">使用可能な値: `first`、`second`、`third`、`fourth`、`last`。</span><span class="sxs-lookup"><span data-stu-id="c34b5-186">Possible values: `first`, `second`, `third`, `fourth`, and `last`.</span></span> <span data-ttu-id="c34b5-187">既定値: `first`。</span><span class="sxs-lookup"><span data-stu-id="c34b5-187">Default value: `first`.</span></span> |
| <span data-ttu-id="c34b5-188">**interval**</span><span class="sxs-lookup"><span data-stu-id="c34b5-188">**interval**</span></span> | <span data-ttu-id="c34b5-189">必須</span><span class="sxs-lookup"><span data-stu-id="c34b5-189">Required</span></span> | <span data-ttu-id="c34b5-190">次の予定までの月数を指定します。</span><span class="sxs-lookup"><span data-stu-id="c34b5-190">Specifies the number of months between each occurrence.</span></span> |
| <span data-ttu-id="c34b5-191">**type**</span><span class="sxs-lookup"><span data-stu-id="c34b5-191">**type**</span></span> | <span data-ttu-id="c34b5-192">必須</span><span class="sxs-lookup"><span data-stu-id="c34b5-192">Required</span></span> | <span data-ttu-id="c34b5-193">`relativeMonthly` に設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="c34b5-193">Must be set to `relativeMonthly`.</span></span> |

#### <a name="examples"></a><span data-ttu-id="c34b5-194">例</span><span class="sxs-lookup"><span data-stu-id="c34b5-194">Examples</span></span>

- <span data-ttu-id="c34b5-195">毎月第 2 水曜日にこのイベントを繰り返す</span><span class="sxs-lookup"><span data-stu-id="c34b5-195">Repeat this event on the second Wednesday of every month</span></span>

  ```json
    "pattern": {
      "type": "relativeMonthly",
      "interval": 1,
      "daysOfWeek": [ "Wednesday" ],
      "index": "second"
    }
  ```
- <span data-ttu-id="c34b5-196">毎月第 1 木曜日または第 1 金曜日にこのイベントを繰り返す</span><span class="sxs-lookup"><span data-stu-id="c34b5-196">Repeat this event on the first Thursday or Friday of every month</span></span>

  ```json
    "pattern": {
      "type": "relativeMonthly",
      "interval": 1,
      "daysOfWeek": [ "Thursday", "Friday" ],
      "index": "first"
    }
  ```

### <a name="absolute-yearly"></a><span data-ttu-id="c34b5-197">絶対年</span><span class="sxs-lookup"><span data-stu-id="c34b5-197">Absolute yearly</span></span>

<span data-ttu-id="c34b5-198">絶対年というパターンでは、次の予定までの年数に基づいて同じ月の同じ日 (たとえば、4 月 15 日) にイベントが繰り返されます。</span><span class="sxs-lookup"><span data-stu-id="c34b5-198">The absolute yearly pattern causes an event to repeat on the same month and day (e.g. April 15th), based on the number of years between each occurrence.</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="c34b5-199">関連するプロパティ</span><span class="sxs-lookup"><span data-stu-id="c34b5-199">Relevant properties</span></span>

| <span data-ttu-id="c34b5-200">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c34b5-200">Property</span></span> | <span data-ttu-id="c34b5-201">関連性</span><span class="sxs-lookup"><span data-stu-id="c34b5-201">Relevance</span></span> | <span data-ttu-id="c34b5-202">説明</span><span class="sxs-lookup"><span data-stu-id="c34b5-202">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="c34b5-203">**dayOfMonth**</span><span class="sxs-lookup"><span data-stu-id="c34b5-203">**dayOfMonth**</span></span> | <span data-ttu-id="c34b5-204">必須</span><span class="sxs-lookup"><span data-stu-id="c34b5-204">Required</span></span> | <span data-ttu-id="c34b5-205">イベントが発生する月の日付を指定します。</span><span class="sxs-lookup"><span data-stu-id="c34b5-205">Specifies on which day of the month the event occurs.</span></span> |
| <span data-ttu-id="c34b5-206">**month**</span><span class="sxs-lookup"><span data-stu-id="c34b5-206">**month**</span></span> | <span data-ttu-id="c34b5-207">必須</span><span class="sxs-lookup"><span data-stu-id="c34b5-207">Required</span></span> | <span data-ttu-id="c34b5-208">イベントが発生する月を指定します。</span><span class="sxs-lookup"><span data-stu-id="c34b5-208">Specifies in which month the event occurs.</span></span> |
| <span data-ttu-id="c34b5-209">**interval**</span><span class="sxs-lookup"><span data-stu-id="c34b5-209">**interval**</span></span> | <span data-ttu-id="c34b5-210">必須</span><span class="sxs-lookup"><span data-stu-id="c34b5-210">Required</span></span> | <span data-ttu-id="c34b5-211">次の予定までの年数を指定します。</span><span class="sxs-lookup"><span data-stu-id="c34b5-211">Specifies the number of years between each occurrence.</span></span> |
| <span data-ttu-id="c34b5-212">**type**</span><span class="sxs-lookup"><span data-stu-id="c34b5-212">**type**</span></span> | <span data-ttu-id="c34b5-213">必須</span><span class="sxs-lookup"><span data-stu-id="c34b5-213">Required</span></span> | <span data-ttu-id="c34b5-214">`absoluteYearly` に設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="c34b5-214">Must be set to `absoluteYearly`.</span></span> |

#### <a name="example"></a><span data-ttu-id="c34b5-215">例</span><span class="sxs-lookup"><span data-stu-id="c34b5-215">Example</span></span>

- <span data-ttu-id="c34b5-216">毎年 4 月 15 日にこのイベントを繰り返す</span><span class="sxs-lookup"><span data-stu-id="c34b5-216">Repeat this event on April 15 every year</span></span>

  ```json
    "pattern": {
      "type": "absoluteYearly",
      "interval": 1,
      "dayOfMonth": 15,
      "month": 4
    }
  ```

### <a name="relative-yearly"></a><span data-ttu-id="c34b5-217">相対年</span><span class="sxs-lookup"><span data-stu-id="c34b5-217">Relative yearly</span></span>

<span data-ttu-id="c34b5-218">相対年というパターンでは、次の予定までの年数に基づいて、特定の月の同じ相対位置にある同じ曜日にイベントが繰り返されます。</span><span class="sxs-lookup"><span data-stu-id="c34b5-218">The relative yearly pattern causes an event to repeat on the same day of the week in the same relative position in a specific month, based on the number of years between each occurrence.</span></span> <span data-ttu-id="c34b5-219">たとえば、「11 月の最後の水曜日」です。</span><span class="sxs-lookup"><span data-stu-id="c34b5-219">For example, "every last Wednesday of November".</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="c34b5-220">関連するプロパティ</span><span class="sxs-lookup"><span data-stu-id="c34b5-220">Relevant properties</span></span>

| <span data-ttu-id="c34b5-221">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c34b5-221">Property</span></span> | <span data-ttu-id="c34b5-222">関連性</span><span class="sxs-lookup"><span data-stu-id="c34b5-222">Relevance</span></span> | <span data-ttu-id="c34b5-223">説明</span><span class="sxs-lookup"><span data-stu-id="c34b5-223">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="c34b5-224">**daysOfWeek**</span><span class="sxs-lookup"><span data-stu-id="c34b5-224">**daysOfWeek**</span></span> | <span data-ttu-id="c34b5-225">必須</span><span class="sxs-lookup"><span data-stu-id="c34b5-225">Required</span></span> | <span data-ttu-id="c34b5-226">イベントが発生することができる曜日を指定します。</span><span class="sxs-lookup"><span data-stu-id="c34b5-226">Specifies on which day(s) of the week the event can occur.</span></span> <span data-ttu-id="c34b5-227">相対年のイベントは、1 年に一度発生するため、複数の値が指定されている場合、イベントはパターンを満たす最初の日にあたります。</span><span class="sxs-lookup"><span data-stu-id="c34b5-227">Relative yearly events only occur once per year, so if more than one value is specified, the event falls on the first day that satisfies the pattern.</span></span> |
| <span data-ttu-id="c34b5-228">**index**</span><span class="sxs-lookup"><span data-stu-id="c34b5-228">**index**</span></span> | <span data-ttu-id="c34b5-229">省略可能</span><span class="sxs-lookup"><span data-stu-id="c34b5-229">Optional</span></span> | <span data-ttu-id="c34b5-230">月の最初のインスタンスから数えて、**daysOfsWeek** で指定された許可日数のどのインスタンスでイベントが発生するか指定します。</span><span class="sxs-lookup"><span data-stu-id="c34b5-230">Specifies on which instance of the allowed days specified in **daysOfsWeek** the event occurs, counted from the first instance in the month.</span></span> <span data-ttu-id="c34b5-231">使用可能な値: `first`、`second`、`third`、`fourth`、`last`。</span><span class="sxs-lookup"><span data-stu-id="c34b5-231">Possible values: `first`, `second`, `third`, `fourth`, and `last`.</span></span> <span data-ttu-id="c34b5-232">既定値: `first`。</span><span class="sxs-lookup"><span data-stu-id="c34b5-232">Default value: `first`.</span></span> |
| <span data-ttu-id="c34b5-233">**month**</span><span class="sxs-lookup"><span data-stu-id="c34b5-233">**month**</span></span> | <span data-ttu-id="c34b5-234">必須</span><span class="sxs-lookup"><span data-stu-id="c34b5-234">Required</span></span> | <span data-ttu-id="c34b5-235">イベントが発生する月を指定します。</span><span class="sxs-lookup"><span data-stu-id="c34b5-235">Specifies in which month the event occurs.</span></span> |
| <span data-ttu-id="c34b5-236">**interval**</span><span class="sxs-lookup"><span data-stu-id="c34b5-236">**interval**</span></span> | <span data-ttu-id="c34b5-237">必須</span><span class="sxs-lookup"><span data-stu-id="c34b5-237">Required</span></span> | <span data-ttu-id="c34b5-238">次の予定までの年数を指定します。</span><span class="sxs-lookup"><span data-stu-id="c34b5-238">Specifies the number of years between each occurrence.</span></span> |
| <span data-ttu-id="c34b5-239">**type**</span><span class="sxs-lookup"><span data-stu-id="c34b5-239">**type**</span></span> | <span data-ttu-id="c34b5-240">必須</span><span class="sxs-lookup"><span data-stu-id="c34b5-240">Required</span></span> | <span data-ttu-id="c34b5-241">`relativeMonthly` に設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="c34b5-241">Must be set to `relativeMonthly`.</span></span> |

#### <a name="examples"></a><span data-ttu-id="c34b5-242">例</span><span class="sxs-lookup"><span data-stu-id="c34b5-242">Examples</span></span>

- <span data-ttu-id="c34b5-243">毎年 11 月の最後の水曜日にこのイベントを繰り返す</span><span class="sxs-lookup"><span data-stu-id="c34b5-243">Repeat this event on the last Wednesday of November every year</span></span>

  ```json
    "pattern": {
      "type": "relativeYearly",
      "interval": 1,
      "daysOfWeek": [ "Wednesday" ],
      "index": "last",
      "month": 11
    }
  ```

## <a name="recurrence-ranges"></a><span data-ttu-id="c34b5-244">繰り返し範囲</span><span class="sxs-lookup"><span data-stu-id="c34b5-244">Recurrence ranges</span></span>

<span data-ttu-id="c34b5-245">繰り返しの第 2 の部分は範囲です。</span><span class="sxs-lookup"><span data-stu-id="c34b5-245">The second part of a recurrence is the range.</span></span> <span data-ttu-id="c34b5-246">パターンが繰り返される期間を指定します。</span><span class="sxs-lookup"><span data-stu-id="c34b5-246">This specifies how long the pattern repeats.</span></span> <span data-ttu-id="c34b5-247">たとえば、イベントは、10 回出現したら終了する、特定の日付で終了する、または終了しないというように設定できます。</span><span class="sxs-lookup"><span data-stu-id="c34b5-247">For example, an event could end after 10 occurrences, by a specific date, or could have no end.</span></span> <span data-ttu-id="c34b5-248">範囲は、API の [recurrenceRange リソース](../api-reference/v1.0/resources/recurrencepattern.md)で表されます。</span><span class="sxs-lookup"><span data-stu-id="c34b5-248">A range is represented in the API by the [recurrenceRange resource](../api-reference/v1.0/resources/recurrencepattern.md).</span></span>

<span data-ttu-id="c34b5-249">範囲の種類に応じて、**recurrenceRange** の特定のフィールドは、必須になるか、または無視されます。</span><span class="sxs-lookup"><span data-stu-id="c34b5-249">Depending on the type of range, certain fields of the **** are required or ignored.</span></span>

> <span data-ttu-id="c34b5-250">**注**: フィールドが無視される場合でも、検証は行われます。</span><span class="sxs-lookup"><span data-stu-id="c34b5-250">Even if a field is ignored, it is still validated.</span></span> <span data-ttu-id="c34b5-251">使用可能な値のセット リストがフィールドに含まれる場合、そのフィールドが無視されても、許可されたセットの範囲外の値を使用するとエラーが発生します。</span><span class="sxs-lookup"><span data-stu-id="c34b5-251">If a field has a set list of possible values, using a value outside the allowed set will cause an error, even if that field is ignored.</span></span>

<span data-ttu-id="c34b5-252">使用可能な範囲の種類を見てみましょう。</span><span class="sxs-lookup"><span data-stu-id="c34b5-252">Let's take a look at each of the possible range types.</span></span>

### <a name="numbered-range"></a><span data-ttu-id="c34b5-253">番号付き範囲</span><span class="sxs-lookup"><span data-stu-id="c34b5-253">Numbered range</span></span>

<span data-ttu-id="c34b5-254">番号付き範囲により、イベントは開始日から固定した回数、パターンに基づいて発生します。</span><span class="sxs-lookup"><span data-stu-id="c34b5-254">The numbered range causes an event to occur a fixed number of times (based on the pattern) from a start date.</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="c34b5-255">関連するプロパティ</span><span class="sxs-lookup"><span data-stu-id="c34b5-255">Relevant properties</span></span>

| <span data-ttu-id="c34b5-256">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c34b5-256">Property</span></span> | <span data-ttu-id="c34b5-257">関連性</span><span class="sxs-lookup"><span data-stu-id="c34b5-257">Relevance</span></span> | <span data-ttu-id="c34b5-258">説明</span><span class="sxs-lookup"><span data-stu-id="c34b5-258">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="c34b5-259">**numberOfOccurences**</span><span class="sxs-lookup"><span data-stu-id="c34b5-259">**numberOfOccurences**</span></span> | <span data-ttu-id="c34b5-260">必須</span><span class="sxs-lookup"><span data-stu-id="c34b5-260">Required</span></span> | <span data-ttu-id="c34b5-261">発生回数を指定します。</span><span class="sxs-lookup"><span data-stu-id="c34b5-261">Specifies the number of occurrences.</span></span> <span data-ttu-id="c34b5-262">正の整数であることが必要です。</span><span class="sxs-lookup"><span data-stu-id="c34b5-262">Must be a positive integer.</span></span> |
| <span data-ttu-id="c34b5-263">**recurrenceTimeZone**</span><span class="sxs-lookup"><span data-stu-id="c34b5-263">**RecurrenceTimeZone**</span></span> | <span data-ttu-id="c34b5-264">省略可能</span><span class="sxs-lookup"><span data-stu-id="c34b5-264">Optional</span></span> | <span data-ttu-id="c34b5-265">**startDate** プロパティのタイム ゾーンを指定します。</span><span class="sxs-lookup"><span data-stu-id="c34b5-265">Specifies the time zone for the **** property.</span></span> <span data-ttu-id="c34b5-266">指定しない場合は、イベントのタイム ゾーンが使用されます。</span><span class="sxs-lookup"><span data-stu-id="c34b5-266">If not specified, the time zone of the event is used.</span></span> |
| <span data-ttu-id="c34b5-267">**startDate**</span><span class="sxs-lookup"><span data-stu-id="c34b5-267">**startDate**</span></span> | <span data-ttu-id="c34b5-268">必須</span><span class="sxs-lookup"><span data-stu-id="c34b5-268">Required</span></span> | <span data-ttu-id="c34b5-269">パターンの適用を開始する日付を指定します。</span><span class="sxs-lookup"><span data-stu-id="c34b5-269">Specifies the date to start applying the pattern.</span></span> <span data-ttu-id="c34b5-270">**startDate** の値は、[イベント リソース](../api-reference/v1.0/resources/event.md)の **start** プロパティの日付値に対応している必要があります。</span><span class="sxs-lookup"><span data-stu-id="c34b5-270">The value of **** MUST correspond to the date value of the **** property on the [event resource](../api-reference/v1.0/resources/event.md).</span></span> <span data-ttu-id="c34b5-271">パターンと一致しない場合、会議の最初の回はこの日付には発生しないことにご注意ください。</span><span class="sxs-lookup"><span data-stu-id="c34b5-271">Note: the first occurrence of the meeting may not occur on this date if it does not fit the pattern.</span></span> |
| <span data-ttu-id="c34b5-272">**type**</span><span class="sxs-lookup"><span data-stu-id="c34b5-272">**type**</span></span> | <span data-ttu-id="c34b5-273">必須</span><span class="sxs-lookup"><span data-stu-id="c34b5-273">Required</span></span> | <span data-ttu-id="c34b5-274">`numbered` に設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="c34b5-274">Must be set to `numbered`.</span></span> |

#### <a name="examples"></a><span data-ttu-id="c34b5-275">例</span><span class="sxs-lookup"><span data-stu-id="c34b5-275">Examples</span></span>

- <span data-ttu-id="c34b5-276">このイベントを 10 回繰り返す</span><span class="sxs-lookup"><span data-stu-id="c34b5-276">Repeat this event 10 times</span></span>

  ```json
    "range": {
      "type": "numbered",
      "startDate": "2017-04-02",
      "numberOfOccurrences": 10
    }
  ```

### <a name="end-date-range"></a><span data-ttu-id="c34b5-277">終了日の範囲</span><span class="sxs-lookup"><span data-stu-id="c34b5-277">End date range</span></span>

<span data-ttu-id="c34b5-278">終了日の範囲を設定すると、開始日から終了日まで適用可能なパターンに適合するすべての日でイベントが発生します。</span><span class="sxs-lookup"><span data-stu-id="c34b5-278">The end date range causes an event to occur on all days that fit the applicable pattern between a start date and an end date.</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="c34b5-279">関連するプロパティ</span><span class="sxs-lookup"><span data-stu-id="c34b5-279">Relevant properties</span></span>

| <span data-ttu-id="c34b5-280">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c34b5-280">Property</span></span> | <span data-ttu-id="c34b5-281">関連性</span><span class="sxs-lookup"><span data-stu-id="c34b5-281">Relevance</span></span> | <span data-ttu-id="c34b5-282">説明</span><span class="sxs-lookup"><span data-stu-id="c34b5-282">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="c34b5-283">**endDate**</span><span class="sxs-lookup"><span data-stu-id="c34b5-283">**endDate**</span></span> | <span data-ttu-id="c34b5-284">必須</span><span class="sxs-lookup"><span data-stu-id="c34b5-284">Required</span></span> | <span data-ttu-id="c34b5-285">パターンの適用を停止する日付を指定します。</span><span class="sxs-lookup"><span data-stu-id="c34b5-285">Specifies the date to stop applying the pattern.</span></span> <span data-ttu-id="c34b5-286">パターンと一致しない場合、会議の最後の回はこの日付には発生しないことにご注意ください。</span><span class="sxs-lookup"><span data-stu-id="c34b5-286">Note: the last occurrence of the meeting may not occur on this date if it does not fit the pattern.</span></span> |
| <span data-ttu-id="c34b5-287">**recurrenceTimeZone**</span><span class="sxs-lookup"><span data-stu-id="c34b5-287">**RecurrenceTimeZone**</span></span> | <span data-ttu-id="c34b5-288">省略可能</span><span class="sxs-lookup"><span data-stu-id="c34b5-288">Optional</span></span> | <span data-ttu-id="c34b5-289">**startDate** プロパティと **endDate** プロパティのタイム ゾーンを指定します。</span><span class="sxs-lookup"><span data-stu-id="c34b5-289">Specifies the time zone for the **** and **** properties.</span></span> <span data-ttu-id="c34b5-290">指定しない場合は、イベントのタイム ゾーンが使用されます。</span><span class="sxs-lookup"><span data-stu-id="c34b5-290">If not specified, the time zone of the event is used.</span></span> |
| <span data-ttu-id="c34b5-291">**startDate**</span><span class="sxs-lookup"><span data-stu-id="c34b5-291">**startDate**</span></span> | <span data-ttu-id="c34b5-292">必須</span><span class="sxs-lookup"><span data-stu-id="c34b5-292">Required</span></span> | <span data-ttu-id="c34b5-293">パターンの適用を開始する日付を指定します。</span><span class="sxs-lookup"><span data-stu-id="c34b5-293">Specifies the date to start applying the pattern.</span></span> <span data-ttu-id="c34b5-294">**startDate** の値は、[イベント リソース](../api-reference/v1.0/resources/event.md)の **start** プロパティの日付値に対応している必要があります。</span><span class="sxs-lookup"><span data-stu-id="c34b5-294">The value of **** MUST correspond to the date value of the **** property on the [event resource](../api-reference/v1.0/resources/event.md).</span></span> <span data-ttu-id="c34b5-295">パターンと一致しない場合、会議の最初の回はこの日付には発生しないことにご注意ください。</span><span class="sxs-lookup"><span data-stu-id="c34b5-295">Note: the first occurrence of the meeting may not occur on this date if it does not fit the pattern.</span></span> |
| <span data-ttu-id="c34b5-296">**type**</span><span class="sxs-lookup"><span data-stu-id="c34b5-296">**type**</span></span> | <span data-ttu-id="c34b5-297">必須</span><span class="sxs-lookup"><span data-stu-id="c34b5-297">Required</span></span> | <span data-ttu-id="c34b5-298">**endDate** に設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="c34b5-298">Must be set to ****.</span></span> |

#### <a name="examples"></a><span data-ttu-id="c34b5-299">例</span><span class="sxs-lookup"><span data-stu-id="c34b5-299">Examples</span></span>

- <span data-ttu-id="c34b5-300">2017 年 7 月 1 日から 2017 年 7 月 31 日までこのイベントを繰り返す</span><span class="sxs-lookup"><span data-stu-id="c34b5-300">Repeat this event from July 1 2017 to July 31 2017</span></span>

  ```json
    "range": {
      "type": "endDate",
      "startDate": "2017-07-01",
      "endDate": "2017-07-31"
    }
  ```

### <a name="no-end-range"></a><span data-ttu-id="c34b5-301">終了範囲なし</span><span class="sxs-lookup"><span data-stu-id="c34b5-301">No end range</span></span>

<span data-ttu-id="c34b5-302">終了範囲なしに設定すると、開始日以降の適用可能なパターンに適合するすべての日でイベントが発生します。</span><span class="sxs-lookup"><span data-stu-id="c34b5-302">The no end range causes an event to occur on all days that fit the applicable pattern after a start date.</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="c34b5-303">関連するプロパティ</span><span class="sxs-lookup"><span data-stu-id="c34b5-303">Relevant properties</span></span>

| <span data-ttu-id="c34b5-304">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c34b5-304">Property</span></span> | <span data-ttu-id="c34b5-305">関連性</span><span class="sxs-lookup"><span data-stu-id="c34b5-305">Relevance</span></span> | <span data-ttu-id="c34b5-306">説明</span><span class="sxs-lookup"><span data-stu-id="c34b5-306">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="c34b5-307">**recurrenceTimeZone**</span><span class="sxs-lookup"><span data-stu-id="c34b5-307">**RecurrenceTimeZone**</span></span> | <span data-ttu-id="c34b5-308">省略可能</span><span class="sxs-lookup"><span data-stu-id="c34b5-308">Optional</span></span> | <span data-ttu-id="c34b5-309">**startDate** プロパティのタイム ゾーンを指定します。</span><span class="sxs-lookup"><span data-stu-id="c34b5-309">Specifies the time zone for the **** property.</span></span> <span data-ttu-id="c34b5-310">指定しない場合は、イベントのタイム ゾーンが使用されます。</span><span class="sxs-lookup"><span data-stu-id="c34b5-310">If not specified, the time zone of the event is used.</span></span> |
| <span data-ttu-id="c34b5-311">**startDate**</span><span class="sxs-lookup"><span data-stu-id="c34b5-311">**startDate**</span></span> | <span data-ttu-id="c34b5-312">必須</span><span class="sxs-lookup"><span data-stu-id="c34b5-312">Required</span></span> | <span data-ttu-id="c34b5-313">パターンの適用を開始する日付を指定します。</span><span class="sxs-lookup"><span data-stu-id="c34b5-313">Specifies the date to start applying the pattern.</span></span> <span data-ttu-id="c34b5-314">**startDate** の値は、[イベント リソース](../api-reference/v1.0/resources/event.md)の **start** プロパティの日付値に対応している必要があります。</span><span class="sxs-lookup"><span data-stu-id="c34b5-314">The value of **** MUST correspond to the date value of the **** property on the [event resource](../api-reference/v1.0/resources/event.md).</span></span> <span data-ttu-id="c34b5-315">パターンと一致しない場合、会議の最初の回はこの日付には発生しないことにご注意ください。</span><span class="sxs-lookup"><span data-stu-id="c34b5-315">Note: the first occurrence of the meeting may not occur on this date if it does not fit the pattern.</span></span> |
| <span data-ttu-id="c34b5-316">**type**</span><span class="sxs-lookup"><span data-stu-id="c34b5-316">**type**</span></span> | <span data-ttu-id="c34b5-317">必須</span><span class="sxs-lookup"><span data-stu-id="c34b5-317">Required</span></span> | <span data-ttu-id="c34b5-318">`noEnd` に設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="c34b5-318">Must be set to `noEnd`.</span></span> |

#### <a name="examples"></a><span data-ttu-id="c34b5-319">例</span><span class="sxs-lookup"><span data-stu-id="c34b5-319">Examples</span></span>

- <span data-ttu-id="c34b5-320">2017 年 5 月 15 日から永遠にこのイベントを繰り返す</span><span class="sxs-lookup"><span data-stu-id="c34b5-320">Repeat this event from May 15 2017 forever</span></span>

  ```json
    "range": {
      "type": "noEnd",
      "startDate": "2017-05-15"
    }
  ```

## <a name="using-patterns-and-ranges-to-create-recurring-events"></a><span data-ttu-id="c34b5-321">パターンおよび範囲を使用して繰り返しイベントを作成する</span><span class="sxs-lookup"><span data-stu-id="c34b5-321">Using patterns and ranges to create recurring events</span></span>

<span data-ttu-id="c34b5-322">これまでは、パターンと範囲について別々に考えてきました。次に、パターンと範囲がどのように連携し、イベントの **start** プロパティおよび **end** プロパティとどのようにやり取りするかを見てみましょう。</span><span class="sxs-lookup"><span data-stu-id="c34b5-322">Now that we've looked at patterns and ranges separately, let's look at how they work together and how they interact with the **** and **** properties on the event.</span></span>

### <a name="creating-a-recurrence-rule"></a><span data-ttu-id="c34b5-323">繰り返しルールの作成</span><span class="sxs-lookup"><span data-stu-id="c34b5-323">Creating a recurrence rule</span></span>

<span data-ttu-id="c34b5-324">繰り返しルールを作成するには、パターンと範囲の両方を指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="c34b5-324">In order to create a recurrence rule, you must specify both a pattern and a range.</span></span> <span data-ttu-id="c34b5-325">どのパターンの種類も、任意の範囲の種類で使用できます。</span><span class="sxs-lookup"><span data-stu-id="c34b5-325">Any pattern type can work with any range type.</span></span> <span data-ttu-id="c34b5-326">次にいくつかの例を示します。</span><span class="sxs-lookup"><span data-stu-id="c34b5-326">Here are a few suggestions:</span></span>

#### <a name="examples"></a><span data-ttu-id="c34b5-327">例</span><span class="sxs-lookup"><span data-stu-id="c34b5-327">Examples</span></span>

- <span data-ttu-id="c34b5-328">**2017 年 9 月 4 日から年末までの期間、毎週月曜日の午後 1 時から午後 1 時 30 分まで会合する**</span><span class="sxs-lookup"><span data-stu-id="c34b5-328">**Meet from 1:00 PM to 1:30 PM every Monday starting September 4, 2017 until the end of the year**</span></span>

  - <span data-ttu-id="c34b5-329">「毎週月曜日」という要件については、`weekly` 繰り返しパターンの種類で簡単に対応できます。</span><span class="sxs-lookup"><span data-stu-id="c34b5-329">The "every Monday" requirement is easily met by the `weekly` recurrence pattern type.</span></span>
  - <span data-ttu-id="c34b5-330">「年末まで」という要件は、`endDate` 繰り返し範囲の種類を示しています。</span><span class="sxs-lookup"><span data-stu-id="c34b5-330">The "until the end of the year" requirement indicates an `endDate` recurrence range type.</span></span>

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

  <span data-ttu-id="c34b5-331">2017 年 12 月 31 日が日曜日のため、このシリーズの最後の回は 12 月 25 日月曜日になります。</span><span class="sxs-lookup"><span data-stu-id="c34b5-331">Because December 31, 2017 is on a Sunday, the last occurrence in this series will be on Monday, December 25.</span></span>

- <span data-ttu-id="c34b5-332">**2017 年 8 月 29 日から、隔月の最初の木曜日の午後 2 時から午後 3 時まで会合する**</span><span class="sxs-lookup"><span data-stu-id="c34b5-332">**Meet from 2:00 PM to 3:00 PM on the first Thursday of every other month starting August 29, 2017**</span></span>

  - <span data-ttu-id="c34b5-333">「隔月の最初の木曜日」という要件は、相対月パターンを使用して実現できます。</span><span class="sxs-lookup"><span data-stu-id="c34b5-333">The "first Thursday of every other month" requirement is achievable using a relative monthly pattern.</span></span> <span data-ttu-id="c34b5-334">「隔月」の部分は、**interval** を `2` に設定する必要があることを示しています。</span><span class="sxs-lookup"><span data-stu-id="c34b5-334">The "every other month" portion indicates the **** should be set to `2`.</span></span>
  - <span data-ttu-id="c34b5-335">終了日については要件が存在しないため、`noEnd` 範囲の種類を使用することができます。</span><span class="sxs-lookup"><span data-stu-id="c34b5-335">Since there is no requirement on an end date, a `noEnd` range type can be used.</span></span>

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

  <span data-ttu-id="c34b5-336">**startDate** の値が 8 月の最初の木曜日を過ぎているため、このシリーズの最初の回は 9 月になります。</span><span class="sxs-lookup"><span data-stu-id="c34b5-336">Because the value of **** is after the first Thursday in August, the first occurrence of this series will be in September.</span></span>

## <a name="next-steps"></a><span data-ttu-id="c34b5-337">次のステップ</span><span class="sxs-lookup"><span data-stu-id="c34b5-337">Next steps</span></span>
    
<span data-ttu-id="c34b5-338">詳細については、「[Outlook カレンダーとの統合](outlook-calendar-concept-overview.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c34b5-338">Find out more about [integrating with Outlook calendar](outlook-calendar-concept-overview.md).</span></span>
