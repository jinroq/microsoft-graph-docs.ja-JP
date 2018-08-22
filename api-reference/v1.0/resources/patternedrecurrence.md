# <a name="patternedrecurrence-resource-type"></a><span data-ttu-id="f79b7-101">patternedRecurrence リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f79b7-101">patternedRecurrence resource type</span></span>

<span data-ttu-id="f79b7-102">繰り返しのパターンと範囲です。</span><span class="sxs-lookup"><span data-stu-id="f79b7-102">The recurrence pattern and range.</span></span>

## <a name="properties"></a><span data-ttu-id="f79b7-103">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f79b7-103">Properties</span></span>
| <span data-ttu-id="f79b7-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f79b7-104">Property</span></span>     | <span data-ttu-id="f79b7-105">Type</span><span class="sxs-lookup"><span data-stu-id="f79b7-105">Type</span></span>   |<span data-ttu-id="f79b7-106">説明</span><span class="sxs-lookup"><span data-stu-id="f79b7-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f79b7-107">pattern</span><span class="sxs-lookup"><span data-stu-id="f79b7-107">pattern</span></span>|[<span data-ttu-id="f79b7-108">RecurrencePattern</span><span class="sxs-lookup"><span data-stu-id="f79b7-108">RecurrencePattern</span></span>](recurrencepattern.md)|<span data-ttu-id="f79b7-109">イベントの頻度。</span><span class="sxs-lookup"><span data-stu-id="f79b7-109">The frequency of an event.</span></span>|
|<span data-ttu-id="f79b7-110">range</span><span class="sxs-lookup"><span data-stu-id="f79b7-110">range</span></span>|[<span data-ttu-id="f79b7-111">RecurrenceRange</span><span class="sxs-lookup"><span data-stu-id="f79b7-111">RecurrenceRange</span></span>](recurrencerange.md)|<span data-ttu-id="f79b7-112">イベントの期間。</span><span class="sxs-lookup"><span data-stu-id="f79b7-112">The duration of an event.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f79b7-113">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f79b7-113">JSON representation</span></span>

<span data-ttu-id="f79b7-114">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="f79b7-114">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.patternedRecurrence"
}-->

```json
{
  "pattern": {"@odata.type": "microsoft.graph.recurrencePattern"},
  "range": {"@odata.type": "microsoft.graph.recurrenceRange"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "patternedRecurrence resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
