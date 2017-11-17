# <a name="attendee-resource-type"></a><span data-ttu-id="c5fcc-101">参加者リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c5fcc-101">attendee resource type</span></span>

<span data-ttu-id="c5fcc-102">イベントの参加者です。</span><span class="sxs-lookup"><span data-stu-id="c5fcc-102">An event attendee.</span></span>

<span data-ttu-id="c5fcc-103">[attendeeBase](attendeebase.md) から派生します。</span><span class="sxs-lookup"><span data-stu-id="c5fcc-103">Derived from [attendeeBase](attendeebase.md).</span></span>

## <a name="properties"></a><span data-ttu-id="c5fcc-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c5fcc-104">Properties</span></span>
| <span data-ttu-id="c5fcc-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c5fcc-105">Property</span></span>     | <span data-ttu-id="c5fcc-106">型</span><span class="sxs-lookup"><span data-stu-id="c5fcc-106">Type</span></span>   |<span data-ttu-id="c5fcc-107">説明</span><span class="sxs-lookup"><span data-stu-id="c5fcc-107">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c5fcc-108">status</span><span class="sxs-lookup"><span data-stu-id="c5fcc-108">status</span></span>|[<span data-ttu-id="c5fcc-109">ResponseStatus</span><span class="sxs-lookup"><span data-stu-id="c5fcc-109">ResponseStatus</span></span>](responsestatus.md)|<span data-ttu-id="c5fcc-110">イベントに対する参加者からの応答 (なし、承諾、辞退など) と応答が送信された日時。</span><span class="sxs-lookup"><span data-stu-id="c5fcc-110">The attendee's response (none, accepted, declined, etc.) for the event and date-time that the response was sent.</span></span>|
|<span data-ttu-id="c5fcc-111">type</span><span class="sxs-lookup"><span data-stu-id="c5fcc-111">type</span></span>|<span data-ttu-id="c5fcc-112">String</span><span class="sxs-lookup"><span data-stu-id="c5fcc-112">String</span></span>|<span data-ttu-id="c5fcc-113">参加者のタイプは、`Required`、`Optional`、`Resource` です。</span><span class="sxs-lookup"><span data-stu-id="c5fcc-113">The attendee type: `Required`, `Optional`, `Resource`.</span></span>|
|<span data-ttu-id="c5fcc-114">emailAddress</span><span class="sxs-lookup"><span data-stu-id="c5fcc-114">emailAddress</span></span>|[<span data-ttu-id="c5fcc-115">emailAddress</span><span class="sxs-lookup"><span data-stu-id="c5fcc-115">emailAddress</span></span>](emailAddress.md)|<span data-ttu-id="c5fcc-116">参加者の名前と SMTP アドレスが含まれます。</span><span class="sxs-lookup"><span data-stu-id="c5fcc-116">Includes the name and SMTP address of the attendee.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c5fcc-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c5fcc-117">JSON representation</span></span>

<span data-ttu-id="c5fcc-118">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="c5fcc-118">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attendee"
}-->

```json
{
  "status": {"@odata.type": "microsoft.graph.responseStatus"},
  "type": "String",
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"}
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attendee resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->