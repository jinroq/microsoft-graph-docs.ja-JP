# <a name="attendeebase-resource-type"></a><span data-ttu-id="e0080-101">attendeeBase リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e0080-101">attendeeBase resource type</span></span>

<span data-ttu-id="e0080-102">出席者の種類です。</span><span class="sxs-lookup"><span data-stu-id="e0080-102">The type of attendee.</span></span>

<span data-ttu-id="e0080-103">[recipient](recipient.md) から派生します。</span><span class="sxs-lookup"><span data-stu-id="e0080-103">Derived from [recipient](recipient.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="e0080-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e0080-104">JSON representation</span></span>

<span data-ttu-id="e0080-105">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="e0080-105">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.recipient",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attendeeBase"
}-->

```json
{
  "type": "String",
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"}
}

```
## <a name="properties"></a><span data-ttu-id="e0080-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e0080-106">Properties</span></span>
| <span data-ttu-id="e0080-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e0080-107">Property</span></span>     | <span data-ttu-id="e0080-108">タイプ</span><span class="sxs-lookup"><span data-stu-id="e0080-108">Type</span></span>   |<span data-ttu-id="e0080-109">説明</span><span class="sxs-lookup"><span data-stu-id="e0080-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e0080-110">型</span><span class="sxs-lookup"><span data-stu-id="e0080-110">type</span></span>|<span data-ttu-id="e0080-111">AttendeeType</span><span class="sxs-lookup"><span data-stu-id="e0080-111">AttendeeType</span></span>| <span data-ttu-id="e0080-112">出席者の種類です。</span><span class="sxs-lookup"><span data-stu-id="e0080-112">The type of attendee.</span></span> <span data-ttu-id="e0080-113">可能な値は、 `required`、`optional`、`resource` です。</span><span class="sxs-lookup"><span data-stu-id="e0080-113">The possible values are `required`, `optional`, or `resource`.</span></span> <span data-ttu-id="e0080-114">現時点では、出席者が 1 人である場合、[FindMeetingTimes](../api/user_findmeetingtimes.md) では常にその人は `Required` 型と見なされます。</span><span class="sxs-lookup"><span data-stu-id="e0080-114">Currently if the attendee is a person, [FindMeetingTimes](../api/user_findmeetingtimes.md) always considers the person is of the `Required` type.</span></span>|
|<span data-ttu-id="e0080-115">emailAddress</span><span class="sxs-lookup"><span data-stu-id="e0080-115">emailAddress</span></span>|[<span data-ttu-id="e0080-116">emailAddress</span><span class="sxs-lookup"><span data-stu-id="e0080-116">emailAddress</span></span>](emailAddress.md)|<span data-ttu-id="e0080-117">参加者の名前と SMTP アドレスが含まれます。</span><span class="sxs-lookup"><span data-stu-id="e0080-117">Includes the name and SMTP address of the attendee.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attendeeBase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
