# <a name="attendee-resource-type"></a><span data-ttu-id="2cda1-101">参加者リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2cda1-101">attendee resource type</span></span>

<span data-ttu-id="2cda1-102">イベントの参加者です。</span><span class="sxs-lookup"><span data-stu-id="2cda1-102">An event attendee.</span></span> <span data-ttu-id="2cda1-103">これはユーザー、またはテナントの Exchange Server 上でリソースとしてセットアップされている会議室や備品などのリソースとなります。</span><span class="sxs-lookup"><span data-stu-id="2cda1-103">This can be a person or resource such as a meeting room or equipment, that has been set up as a resource on the Exchange server for the tenant.</span></span>

<span data-ttu-id="2cda1-104">[attendeeBase](attendeebase.md) から派生します。</span><span class="sxs-lookup"><span data-stu-id="2cda1-104">Derived from [attendeeBase](attendeebase.md).</span></span>

## <a name="properties"></a><span data-ttu-id="2cda1-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2cda1-105">Properties</span></span>
| <span data-ttu-id="2cda1-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2cda1-106">Property</span></span>     | <span data-ttu-id="2cda1-107">型</span><span class="sxs-lookup"><span data-stu-id="2cda1-107">Type</span></span>   |<span data-ttu-id="2cda1-108">説明</span><span class="sxs-lookup"><span data-stu-id="2cda1-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2cda1-109">status</span><span class="sxs-lookup"><span data-stu-id="2cda1-109">status</span></span>|[<span data-ttu-id="2cda1-110">ResponseStatus</span><span class="sxs-lookup"><span data-stu-id="2cda1-110">ResponseStatus</span></span>](responsestatus.md)|<span data-ttu-id="2cda1-111">イベントに対する参加者からの応答 (なし、承諾、辞退など) と応答が送信された日時。</span><span class="sxs-lookup"><span data-stu-id="2cda1-111">The attendee's response (none, accepted, declined, etc.) for the event and date-time that the response was sent.</span></span>|
|<span data-ttu-id="2cda1-112">type</span><span class="sxs-lookup"><span data-stu-id="2cda1-112">type</span></span>|<span data-ttu-id="2cda1-113">String</span><span class="sxs-lookup"><span data-stu-id="2cda1-113">String</span></span>|<span data-ttu-id="2cda1-114">参加者のタイプは、`required`、`optional`、`resource` です。</span><span class="sxs-lookup"><span data-stu-id="2cda1-114">The attendee type: `required`, `optional`, `resource`.</span></span>|
|<span data-ttu-id="2cda1-115">emailAddress</span><span class="sxs-lookup"><span data-stu-id="2cda1-115">emailAddress</span></span>|[<span data-ttu-id="2cda1-116">emailAddress</span><span class="sxs-lookup"><span data-stu-id="2cda1-116">emailAddress</span></span>](emailAddress.md)|<span data-ttu-id="2cda1-117">参加者の名前と SMTP アドレスが含まれます。</span><span class="sxs-lookup"><span data-stu-id="2cda1-117">Includes the name and SMTP address of the attendee.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2cda1-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2cda1-118">JSON representation</span></span>

<span data-ttu-id="2cda1-119">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="2cda1-119">Here is a JSON representation of the resource</span></span>

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