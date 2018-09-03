# <a name="attendeeavailability-resource-type"></a><span data-ttu-id="209c6-101">attendeeAvailability リソースの種類</span><span class="sxs-lookup"><span data-stu-id="209c6-101">attendeeAvailability resource type</span></span>

<span data-ttu-id="209c6-102">出席者の種類と空き時間情報。</span><span class="sxs-lookup"><span data-stu-id="209c6-102">The type and availability of an attendee.</span></span>

## <a name="json-representation"></a><span data-ttu-id="209c6-103">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="209c6-103">JSON representation</span></span>

<span data-ttu-id="209c6-104">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="209c6-104">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attendeeAvailability"
}-->

```json
{
  "attendee": {"@odata.type": "microsoft.graph.attendeeBase"},
  "availability": "String"
}

```
## <a name="properties"></a><span data-ttu-id="209c6-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="209c6-105">Properties</span></span>
| <span data-ttu-id="209c6-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="209c6-106">Property</span></span>     | <span data-ttu-id="209c6-107">タイプ</span><span class="sxs-lookup"><span data-stu-id="209c6-107">Type</span></span>   |<span data-ttu-id="209c6-108">説明</span><span class="sxs-lookup"><span data-stu-id="209c6-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="209c6-109">出席者</span><span class="sxs-lookup"><span data-stu-id="209c6-109">attendee</span></span>|[<span data-ttu-id="209c6-110">AttendeeBase</span><span class="sxs-lookup"><span data-stu-id="209c6-110">AttendeeBase</span></span>](attendeebase.md)|<span data-ttu-id="209c6-111">出席者の種類 - 人、またはリソースのいずれか、さらに人である場合は、必須かどうか。</span><span class="sxs-lookup"><span data-stu-id="209c6-111">The type of attendee - whether it's a person or a resource, and whether required or optional if it's a person.</span></span>|
|<span data-ttu-id="209c6-112">状態</span><span class="sxs-lookup"><span data-stu-id="209c6-112">availability</span></span>|<span data-ttu-id="209c6-113">FreeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="209c6-113">FreeBusyStatus</span></span>| <span data-ttu-id="209c6-114">出席者の空き時間の状態。</span><span class="sxs-lookup"><span data-stu-id="209c6-114">The availability status of the attendee.</span></span> <span data-ttu-id="209c6-115">指定できる値は、  `free`、`tentative`、`busy`、`oof`、`workingElsewhere`、`unknown` です。</span><span class="sxs-lookup"><span data-stu-id="209c6-115">The possible values are `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`, , , , , , or .</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attendeeAvailability resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
