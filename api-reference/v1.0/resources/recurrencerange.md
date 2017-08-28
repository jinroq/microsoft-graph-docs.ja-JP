# <a name="recurrencerange-resource-type"></a><span data-ttu-id="33bd7-101">recurrenceRange リソースの種類</span><span class="sxs-lookup"><span data-stu-id="33bd7-101">recurrenceRange resource type</span></span>

<span data-ttu-id="33bd7-102">イベントの期間。</span><span class="sxs-lookup"><span data-stu-id="33bd7-102">The duration of an event.</span></span>

## <a name="properties"></a><span data-ttu-id="33bd7-103">プロパティ</span><span class="sxs-lookup"><span data-stu-id="33bd7-103">Properties</span></span>

| <span data-ttu-id="33bd7-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="33bd7-104">Property</span></span>     | <span data-ttu-id="33bd7-105">型</span><span class="sxs-lookup"><span data-stu-id="33bd7-105">Type</span></span>   |<span data-ttu-id="33bd7-106">説明</span><span class="sxs-lookup"><span data-stu-id="33bd7-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="33bd7-107">endDate</span><span class="sxs-lookup"><span data-stu-id="33bd7-107">endDate</span></span>|<span data-ttu-id="33bd7-108">Date</span><span class="sxs-lookup"><span data-stu-id="33bd7-108">Date</span></span>|<span data-ttu-id="33bd7-109">繰り返しの終了日です。</span><span class="sxs-lookup"><span data-stu-id="33bd7-109">The end date of the series.</span></span>|
|<span data-ttu-id="33bd7-110">numberOfOccurrences</span><span class="sxs-lookup"><span data-stu-id="33bd7-110">numberOfOccurrences</span></span>|<span data-ttu-id="33bd7-111">Int32</span><span class="sxs-lookup"><span data-stu-id="33bd7-111">Int32</span></span>|<span data-ttu-id="33bd7-112">イベントを繰り返す回数。</span><span class="sxs-lookup"><span data-stu-id="33bd7-112">How many times to repeat the event.</span></span>|
|<span data-ttu-id="33bd7-113">recurrenceTimeZone</span><span class="sxs-lookup"><span data-stu-id="33bd7-113">recurrenceTimeZone</span></span>|<span data-ttu-id="33bd7-114">String</span><span class="sxs-lookup"><span data-stu-id="33bd7-114">String</span></span> |<span data-ttu-id="33bd7-115">**startDate** プロパティと **endDate** プロパティのタイム ゾーン。</span><span class="sxs-lookup"><span data-stu-id="33bd7-115">Time zone for the **startDate** and **endDate** properties.</span></span> |
|<span data-ttu-id="33bd7-116">startDate</span><span class="sxs-lookup"><span data-stu-id="33bd7-116">startDate</span></span>|<span data-ttu-id="33bd7-117">Date</span><span class="sxs-lookup"><span data-stu-id="33bd7-117">Date</span></span>|<span data-ttu-id="33bd7-118">繰り返しの開始日です。</span><span class="sxs-lookup"><span data-stu-id="33bd7-118">The start date of the series.</span></span>|
|<span data-ttu-id="33bd7-119">type</span><span class="sxs-lookup"><span data-stu-id="33bd7-119">type</span></span>|<span data-ttu-id="33bd7-120">String</span><span class="sxs-lookup"><span data-stu-id="33bd7-120">String</span></span>|<span data-ttu-id="33bd7-p101">次のような繰り返し範囲があります。終了日 = 0、無制限 = 1、番号順 = 2。可能な値は、`EndDate`、`NoEnd`、`Numbered` です。</span><span class="sxs-lookup"><span data-stu-id="33bd7-p101">The recurrence range: EndDate = 0, NoEnd = 1, Numbered = 2. Possible values are: `EndDate`, `NoEnd`, `Numbered`.</span></span>||

## <a name="json-representation"></a><span data-ttu-id="33bd7-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="33bd7-123">JSON representation</span></span>

<span data-ttu-id="33bd7-124">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="33bd7-124">Here is a JSON representation of the resource</span></span>

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
