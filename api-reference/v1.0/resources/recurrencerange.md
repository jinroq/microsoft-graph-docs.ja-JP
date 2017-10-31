# <a name="recurrencerange-resource-type"></a><span data-ttu-id="42ed4-101">recurrenceRange リソースの種類</span><span class="sxs-lookup"><span data-stu-id="42ed4-101">recurrenceRange resource type</span></span>

<span data-ttu-id="42ed4-102">定期的な[イベント](event.md)を繰り返す期間について説明します。</span><span class="sxs-lookup"><span data-stu-id="42ed4-102">Describes a date range over which a recurring [event](event.md) repeats.</span></span> 

<span data-ttu-id="42ed4-103">シナリオに応じて、定期的なイベントの 3 通りの期間のいずれかを指定できます。</span><span class="sxs-lookup"><span data-stu-id="42ed4-103">You can specify the date range for a recurring event in one of 3 ways depending on your scenario.</span></span> <span data-ttu-id="42ed4-104">期間の **startDate** 値は必ず指定する必要がありますが、定期的なイベントの終了は、たとえば、特定の日付までに終了する、終了しない、または 5 回繰り返した後に終了する、など指定することができます。</span><span class="sxs-lookup"><span data-stu-id="42ed4-104">While you must always specify a **startDate** value for the date range, you can, for example, specify a recurring event that ends by a specific date, or that doesn't end, or that ends after 5 occurrences.</span></span> <span data-ttu-id="42ed4-105">イベントに対して指定した期間内の定期的なイベントは、必ずこの定期的なパターンに従って発生します。</span><span class="sxs-lookup"><span data-stu-id="42ed4-105">Note that the actual occurrences within the date range always follow the recurrence pattern that you specify for the recurring event.</span></span> <span data-ttu-id="42ed4-106">定期的なイベントは常に、[recurrencePattern](recurrencepattern.md) (イベントを繰り返す頻度)、および **recurrenceRange** (イベントを繰り返す期間) によって定義されます。</span><span class="sxs-lookup"><span data-stu-id="42ed4-106">A recurring event is always defined by its [recurrencePattern](recurrencepattern.md) (how frequently the event repeats), and its **recurrenceRange** (for how long the event repeats).</span></span>

<span data-ttu-id="42ed4-107">**type** プロパティを使用して、**recurrenceRange** のさまざまな種類から期間を指定します。</span><span class="sxs-lookup"><span data-stu-id="42ed4-107">Use the **type** property to specify the different types of **recurrenceRange**.</span></span> <span data-ttu-id="42ed4-108">種類ごとに必要なプロパティについては、次の表の説明を参照してください。</span><span class="sxs-lookup"><span data-stu-id="42ed4-108">Note the required properties for each type, as described in the following table.</span></span>

| <span data-ttu-id="42ed4-109">繰り返す期間の種類</span><span class="sxs-lookup"><span data-stu-id="42ed4-109">Type of recurrence range</span></span> | <span data-ttu-id="42ed4-110">type プロパティの値</span><span class="sxs-lookup"><span data-stu-id="42ed4-110">Value of type property</span></span> | <span data-ttu-id="42ed4-111">説明</span><span class="sxs-lookup"><span data-stu-id="42ed4-111">Description</span></span> | <span data-ttu-id="42ed4-112">例</span><span class="sxs-lookup"><span data-stu-id="42ed4-112">Example</span></span> | <span data-ttu-id="42ed4-113">必須のプロパティ</span><span class="sxs-lookup"><span data-stu-id="42ed4-113">Required properties</span></span> |
|:---------------|:--------|:--------|:--------|:----------|
|<span data-ttu-id="42ed4-114">終了日が指定された期間</span><span class="sxs-lookup"><span data-stu-id="42ed4-114">Range with end date</span></span> | `endDate` | <span data-ttu-id="42ed4-115">**startDate** と **endDate** の間の、対応する定期的なパターンに適合するすべての日に、イベントが繰り返されます。</span><span class="sxs-lookup"><span data-stu-id="42ed4-115">Event repeats on all the days that fit the corresponding recurrence pattern between the **startDate** and **endDate**.</span></span> | <span data-ttu-id="42ed4-116">2017 年 6 月 1 日から 2017 年 6 月 15 日の期間で、イベントを繰り返します。</span><span class="sxs-lookup"><span data-stu-id="42ed4-116">Repeat event in the date range between June 1, 2017 and June 15, 2017.</span></span> | <span data-ttu-id="42ed4-117">**type**、**startDate**、**endDate**</span><span class="sxs-lookup"><span data-stu-id="42ed4-117">**type**, **startDate**, **endDate**</span></span> | 
|<span data-ttu-id="42ed4-118">終了日が指定されていない期間</span><span class="sxs-lookup"><span data-stu-id="42ed4-118">Range without an end date</span></span> | `noEnd` | <span data-ttu-id="42ed4-119">**startDate** に始まる、対応する定期的なパターンに適合するすべての日に、イベントが繰り返されます。</span><span class="sxs-lookup"><span data-stu-id="42ed4-119">Event repeats on all the days that fit the corresponding recurrence pattern beginning on the **startDate**.</span></span> | <span data-ttu-id="42ed4-120">2017 年 6 月 1 日に始まる期間に、イベントを無期限に繰り返します。</span><span class="sxs-lookup"><span data-stu-id="42ed4-120">Repeat event in the date range starting on June 1, 2017 indefinitely.</span></span> | <span data-ttu-id="42ed4-121">**type**、**startDate**</span><span class="sxs-lookup"><span data-stu-id="42ed4-121">**type**, **startDate**</span></span> |
|<span data-ttu-id="42ed4-122">発生回数を指定した期間</span><span class="sxs-lookup"><span data-stu-id="42ed4-122">Range with specific number of occurrences</span></span> | `numbered` | <span data-ttu-id="42ed4-123">**startDate** に始まる定期的なパターンに基づいて、**numberOfOccurrences** で指定した回数、イベントが繰り返されます。</span><span class="sxs-lookup"><span data-stu-id="42ed4-123">Event repeats for the **numberOfOccurrences** based on the recurrence pattern beginning on the **startDate**.</span></span> | <span data-ttu-id="42ed4-124">2017 年 6 月 1 日に始まる期間に、イベントを 10 回繰り返します。</span><span class="sxs-lookup"><span data-stu-id="42ed4-124">Repeat event in the date range starting on June 1, 2017, for 10 occurrences.</span></span>  | <span data-ttu-id="42ed4-125">**type**、**startDate**、**numberOfOccurrences**</span><span class="sxs-lookup"><span data-stu-id="42ed4-125">**type**, **startDate**, **numberOfOccurrences**</span></span> |


## <a name="properties"></a><span data-ttu-id="42ed4-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="42ed4-126">Properties</span></span>

| <span data-ttu-id="42ed4-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="42ed4-127">Property</span></span>     | <span data-ttu-id="42ed4-128">型</span><span class="sxs-lookup"><span data-stu-id="42ed4-128">Type</span></span>   |<span data-ttu-id="42ed4-129">説明</span><span class="sxs-lookup"><span data-stu-id="42ed4-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="42ed4-130">endDate</span><span class="sxs-lookup"><span data-stu-id="42ed4-130">endDate</span></span>|<span data-ttu-id="42ed4-131">Date</span><span class="sxs-lookup"><span data-stu-id="42ed4-131">Date</span></span>|<span data-ttu-id="42ed4-132">定期的なパターンの適用を停止する日付。</span><span class="sxs-lookup"><span data-stu-id="42ed4-132">Specifies the date to stop applying the pattern.</span></span> <span data-ttu-id="42ed4-133">イベントの定期的なパターンによっては、最後に会議が発生するのは、この日付にならない可能性があります。</span><span class="sxs-lookup"><span data-stu-id="42ed4-133">Depending on the recurrence pattern of the event, the last occurrence of the meeting may not be this date.</span></span> <span data-ttu-id="42ed4-134">**type** が `endDate` の場合、必要です。</span><span class="sxs-lookup"><span data-stu-id="42ed4-134">Required if **type** is `endDate`.</span></span>|
|<span data-ttu-id="42ed4-135">numberOfOccurrences</span><span class="sxs-lookup"><span data-stu-id="42ed4-135">numberOfOccurrences</span></span>|<span data-ttu-id="42ed4-136">Int32</span><span class="sxs-lookup"><span data-stu-id="42ed4-136">Int32</span></span>|<span data-ttu-id="42ed4-137">イベントを繰り返す回数を指定します。</span><span class="sxs-lookup"><span data-stu-id="42ed4-137">The number of times to repeat the event.</span></span> <span data-ttu-id="42ed4-138">必須です。**type** が `numbered` の場合、正の値である必要があります。</span><span class="sxs-lookup"><span data-stu-id="42ed4-138">Required and must be positive if **type** is `numbered`.</span></span>|
|<span data-ttu-id="42ed4-139">recurrenceTimeZone</span><span class="sxs-lookup"><span data-stu-id="42ed4-139">recurrenceTimeZone</span></span>|<span data-ttu-id="42ed4-140">String</span><span class="sxs-lookup"><span data-stu-id="42ed4-140">String</span></span> |<span data-ttu-id="42ed4-141">**startDate** プロパティと **endDate** プロパティのタイム ゾーン。</span><span class="sxs-lookup"><span data-stu-id="42ed4-141">Time zone for the **startDate** and **endDate** properties.</span></span> <span data-ttu-id="42ed4-142">省略可能。</span><span class="sxs-lookup"><span data-stu-id="42ed4-142">Optional.</span></span> <span data-ttu-id="42ed4-143">指定されていない場合は、イベントのタイム ゾーンが使用されます。</span><span class="sxs-lookup"><span data-stu-id="42ed4-143">If not specified, the time zone of the event is used.</span></span>|
|<span data-ttu-id="42ed4-144">startDate</span><span class="sxs-lookup"><span data-stu-id="42ed4-144">startDate</span></span>|<span data-ttu-id="42ed4-145">Date</span><span class="sxs-lookup"><span data-stu-id="42ed4-145">Date</span></span>|<span data-ttu-id="42ed4-146">定期的なパターンの適用を開始する日付。</span><span class="sxs-lookup"><span data-stu-id="42ed4-146">Specifies the date to start applying the pattern.</span></span> <span data-ttu-id="42ed4-147">イベントの定期的なパターンによっては、最初に会議が発生するのは、この日付以降になる場合があります。</span><span class="sxs-lookup"><span data-stu-id="42ed4-147">The first occurrence of the meeting may be this date or later, depending on the recurrence pattern of the event.</span></span> <span data-ttu-id="42ed4-148">定期的な[イベント](event.md)の **start** プロパティと同じ値である必要があります。</span><span class="sxs-lookup"><span data-stu-id="42ed4-148">Must be the same value as the **start** property of the recurring [event](event.md).</span></span> <span data-ttu-id="42ed4-149">必須。</span><span class="sxs-lookup"><span data-stu-id="42ed4-149">Required.</span></span>|
|<span data-ttu-id="42ed4-150">type</span><span class="sxs-lookup"><span data-stu-id="42ed4-150">type</span></span>|<span data-ttu-id="42ed4-151">String</span><span class="sxs-lookup"><span data-stu-id="42ed4-151">String</span></span>|<span data-ttu-id="42ed4-152">繰り返す期間。</span><span class="sxs-lookup"><span data-stu-id="42ed4-152">The recurrence pattern and range.</span></span> <span data-ttu-id="42ed4-153">使用可能な値は、`endDate`、`noEnd`、`numbered` です。</span><span class="sxs-lookup"><span data-stu-id="42ed4-153">Possible values are: `endDate`, `noEnd`, `numbered`, .</span></span> <span data-ttu-id="42ed4-154">必須。</span><span class="sxs-lookup"><span data-stu-id="42ed4-154">Required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="42ed4-155">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="42ed4-155">JSON representation</span></span>

<span data-ttu-id="42ed4-156">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="42ed4-156">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recurrencerange"
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
<!-- {
  "type": "#page.annotation",
  "description": "recurrenceRange resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
