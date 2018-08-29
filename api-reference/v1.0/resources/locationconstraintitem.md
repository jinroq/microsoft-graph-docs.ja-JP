# <a name="locationconstraintitem-resource-type"></a><span data-ttu-id="b9431-101">locationConstraintItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b9431-101">locationConstraintItem resource type</span></span>

<span data-ttu-id="b9431-102">会議の場所に関して、クライアントが表明している条件です。</span><span class="sxs-lookup"><span data-stu-id="b9431-102">The conditions stated by a client for the location of a meeting.</span></span>

<span data-ttu-id="b9431-103">[location](location.md) から派生します。</span><span class="sxs-lookup"><span data-stu-id="b9431-103">Derived from [location](location.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="b9431-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b9431-104">JSON representation</span></span>

<span data-ttu-id="b9431-105">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="b9431-105">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.location",
  "@odata.type": "microsoft.graph.locationConstraintItem"
}-->

```json
{
  "resolveAvailability": true,
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "displayName": "string",
  "locationEmailAddress": "string"
}

```
## <a name="properties"></a><span data-ttu-id="b9431-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b9431-106">Properties</span></span>
| <span data-ttu-id="b9431-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b9431-107">Property</span></span>     | <span data-ttu-id="b9431-108">タイプ</span><span class="sxs-lookup"><span data-stu-id="b9431-108">Type</span></span>   |<span data-ttu-id="b9431-109">説明</span><span class="sxs-lookup"><span data-stu-id="b9431-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b9431-110">address</span><span class="sxs-lookup"><span data-stu-id="b9431-110">address</span></span> | [<span data-ttu-id="b9431-111">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="b9431-111">physicalAddress</span></span>](physicalAddress.md) |<span data-ttu-id="b9431-112">場所の番地。</span><span class="sxs-lookup"><span data-stu-id="b9431-112">The street address of the location.</span></span> |
| <span data-ttu-id="b9431-113">displayName</span><span class="sxs-lookup"><span data-stu-id="b9431-113">displayName</span></span>  | <span data-ttu-id="b9431-114">文字列</span><span class="sxs-lookup"><span data-stu-id="b9431-114">String</span></span> | <span data-ttu-id="b9431-115">場所に関連付けられた名前。</span><span class="sxs-lookup"><span data-stu-id="b9431-115">The name associated with the location.</span></span>                       |
| <span data-ttu-id="b9431-116">locationEmailAddress</span><span class="sxs-lookup"><span data-stu-id="b9431-116">locationEmailAddress</span></span> | <span data-ttu-id="b9431-117">文字列</span><span class="sxs-lookup"><span data-stu-id="b9431-117">String</span></span> | <span data-ttu-id="b9431-118">場所の電子メール アドレス (省略可能)。</span><span class="sxs-lookup"><span data-stu-id="b9431-118">Optional email address of the location.</span></span> |
| <span data-ttu-id="b9431-119">resolveAvailability</span><span class="sxs-lookup"><span data-stu-id="b9431-119">resolveAvailability</span></span> | <span data-ttu-id="b9431-120">ブーリアン</span><span class="sxs-lookup"><span data-stu-id="b9431-120">Boolean</span></span> | <span data-ttu-id="b9431-121">true に設定されているときに指定したリソースがビジー状態である場合は、[findMeetingTimes](../api/user_findmeetingtimes.md) 空いている別のリソースを検索します。</span><span class="sxs-lookup"><span data-stu-id="b9431-121">If set to true and the specified resource is busy, [findMeetingTimes](../api/user_findmeetingtimes.md) looks for another resource that is free.</span></span> <span data-ttu-id="b9431-122">false に設定されているときに指定したリソースがビジー状態である場合は、**findMeetingTimes** はリソースが空いているかどうかを確認しないで、ユーザーのキャッシュでトップにランク付けられているリソースを返します。</span><span class="sxs-lookup"><span data-stu-id="b9431-122">If set to true and the specified resource is busy, findMeetingTimes looks for another resource that is free. If set to false and the specified resource is busy, **findMeetingTimes** returns the resource best ranked in the user's cache without checking if it's free. Default is true.</span></span> <span data-ttu-id="b9431-123">既定では true を指定 します。</span><span class="sxs-lookup"><span data-stu-id="b9431-123">Default is True.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "locationConstraintItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->