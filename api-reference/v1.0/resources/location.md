# <a name="location-resource-type"></a><span data-ttu-id="4027d-101">Location リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4027d-101">Location resource type</span></span>

<span data-ttu-id="4027d-102">[イベント](event.md)の場所の情報を表します。</span><span class="sxs-lookup"><span data-stu-id="4027d-102">Represents location information of an [event](event.md).</span></span>

<span data-ttu-id="4027d-103">カレンダー内にイベントを作成するには、複数の方法があります。たとえば、アプリで[イベント作成](../api/user_post_events.md) REST API を使用するという方法、Outlook ユーザー インターフェイスを手動で使用するという方法などです。</span><span class="sxs-lookup"><span data-stu-id="4027d-103">There are multiple ways to create events in a calendar, for example, through an app using the [create event](../api/user_post_events.md) REST API, or manually using the Outlook user interface.</span></span> <span data-ttu-id="4027d-104">ユーザー インターフェイスを使用してイベントを作成する場合は、場所をプレーン テキストとして指定することも、Outlook、[Bing Autosuggest](https://blogs.bing.com/search/2013/02/20/a-look-at-autosuggest/)、または [Bing ローカル検索](https://blogs.bing.com/search/2010/08/17/local-search-on-m-bing-com/)で提供される会議室リストから選択して指定することもできます。</span><span class="sxs-lookup"><span data-stu-id="4027d-104">When you create an event using the user interface, you can specify the location as plain text (for example, "Harry's Bar"), or from the rooms list provided by Outlook, [Bing Autosuggest](https://blogs.bing.com/search/2013/02/20/a-look-at-autosuggest/), or [Bing local search](https://blogs.bing.com/search/2010/08/17/local-search-on-m-bing-com/).</span></span> 

<span data-ttu-id="4027d-105">イベントの作成方法によって、Outlook は読み取り専用の **locationType** プロパティを異なる方法で設定します。</span><span class="sxs-lookup"><span data-stu-id="4027d-105">Depending on how an event is created, expect Outlook to set the read-only **locationType** property differently.</span></span> 

| <span data-ttu-id="4027d-106">イベントの作成方法</span><span class="sxs-lookup"><span data-stu-id="4027d-106">How event was created</span></span>  | <span data-ttu-id="4027d-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4027d-107">Property</span></span>   | <span data-ttu-id="4027d-108">予期される値</span><span class="sxs-lookup"><span data-stu-id="4027d-108">Expected value</span></span> |
|:----------|:-------|:--------------------------------|
| <span data-ttu-id="4027d-109">[イベント作成](../api/user_post_events.md) REST API</span><span class="sxs-lookup"><span data-stu-id="4027d-109">[create event](../api/user_post_events.md) REST API</span></span> | <span data-ttu-id="4027d-110">**locationType**</span><span class="sxs-lookup"><span data-stu-id="4027d-110">**locationType**</span></span> | `default` |
| <span data-ttu-id="4027d-111">Outlook のユーザー インターフェイス</span><span class="sxs-lookup"><span data-stu-id="4027d-111">User interface in Outlook</span></span> | <span data-ttu-id="4027d-112">**locationType**</span><span class="sxs-lookup"><span data-stu-id="4027d-112">**locationType**</span></span> | <span data-ttu-id="4027d-113">以下のいずれか:</span><span class="sxs-lookup"><span data-stu-id="4027d-113">One of the following:</span></span> <ul><li><span data-ttu-id="4027d-114">プレーン テキストとして入力された場所の場合は `default`。</span><span class="sxs-lookup"><span data-stu-id="4027d-114">`default` for a location entered as plain text.</span></span></li><li><span data-ttu-id="4027d-115">Outlook の会議室リストで提供された会議室の場合は `conferenceRoom`。</span><span class="sxs-lookup"><span data-stu-id="4027d-115">`conferenceRoom` for a room provided by the Outlook rooms list.</span></span></li><li><span data-ttu-id="4027d-116">Bing Autosuggest または Bing ローカル検索による場所の場合は、`homeAddress`、`businessAddress`、`geoCoordinates`、`streetAddress`、`hotel`、`restaurant`、`localBusiness`、`postalAddress` のいずれか。</span><span class="sxs-lookup"><span data-stu-id="4027d-116">Or, any of this list - `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress` - for a location from Bing Autosuggest or Bing local search.</span></span></li></ul> |

## <a name="properties"></a><span data-ttu-id="4027d-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4027d-117">Properties</span></span>
| <span data-ttu-id="4027d-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4027d-118">Property</span></span>  | <span data-ttu-id="4027d-119">型</span><span class="sxs-lookup"><span data-stu-id="4027d-119">Type</span></span>   | <span data-ttu-id="4027d-120">説明</span><span class="sxs-lookup"><span data-stu-id="4027d-120">Description</span></span>                                                     |
|:----------|:-------|:----------------------------------------------------------------|
| <span data-ttu-id="4027d-121">address</span><span class="sxs-lookup"><span data-stu-id="4027d-121">address</span></span> | [<span data-ttu-id="4027d-122">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="4027d-122">physicalAddress</span></span>](physicaladdress.md) |<span data-ttu-id="4027d-123">場所の番地。</span><span class="sxs-lookup"><span data-stu-id="4027d-123">The street address of the location.</span></span> |
| <span data-ttu-id="4027d-124">coordinates</span><span class="sxs-lookup"><span data-stu-id="4027d-124">coordinates</span></span> | [<span data-ttu-id="4027d-125">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="4027d-125">outlookGeoCoordinates</span></span>](outlookgeocoordinates.md) | <span data-ttu-id="4027d-126">場所の地理的座標と標高。</span><span class="sxs-lookup"><span data-stu-id="4027d-126">The geographic coordinates and elevation of the location.</span></span> |
| <span data-ttu-id="4027d-127">displayName</span><span class="sxs-lookup"><span data-stu-id="4027d-127">displayName</span></span>  | <span data-ttu-id="4027d-128">String</span><span class="sxs-lookup"><span data-stu-id="4027d-128">String</span></span> | <span data-ttu-id="4027d-129">場所に関連付けられた名前。</span><span class="sxs-lookup"><span data-stu-id="4027d-129">The name associated with the location.</span></span>                       |
| <span data-ttu-id="4027d-130">locationEmailAddress</span><span class="sxs-lookup"><span data-stu-id="4027d-130">locationEmailAddress</span></span> | <span data-ttu-id="4027d-131">String</span><span class="sxs-lookup"><span data-stu-id="4027d-131">String</span></span> | <span data-ttu-id="4027d-132">場所のメール アドレス (省略可能)。</span><span class="sxs-lookup"><span data-stu-id="4027d-132">Optional email address of the location.</span></span>              |
| <span data-ttu-id="4027d-133">locationUri</span><span class="sxs-lookup"><span data-stu-id="4027d-133">locationUri</span></span> | <span data-ttu-id="4027d-134">String</span><span class="sxs-lookup"><span data-stu-id="4027d-134">String</span></span> | <span data-ttu-id="4027d-135">場所を表す URI (省略可能)。</span><span class="sxs-lookup"><span data-stu-id="4027d-135">Optional URI representing the location.</span></span> |
| <span data-ttu-id="4027d-136">locationType</span><span class="sxs-lookup"><span data-stu-id="4027d-136">locationType</span></span> | <span data-ttu-id="4027d-137">String</span><span class="sxs-lookup"><span data-stu-id="4027d-137">String</span></span> | <span data-ttu-id="4027d-138">場所の種類。</span><span class="sxs-lookup"><span data-stu-id="4027d-138">The type of location.</span></span> <span data-ttu-id="4027d-139">可能な値は、`default`、`conferenceRoom`、`homeAddress`、`businessAddress`、`geoCoordinates`、`streetAddress`、`hotel`、`restaurant`、`localBusiness`、`postalAddress` です。</span><span class="sxs-lookup"><span data-stu-id="4027d-139">Possible values are: `default`, `conferenceRoom`, `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress`.</span></span> <span data-ttu-id="4027d-140">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="4027d-140">Read-only.</span></span>|
| <span data-ttu-id="4027d-141">uniqueId</span><span class="sxs-lookup"><span data-stu-id="4027d-141">uniqueId</span></span> | <span data-ttu-id="4027d-142">String</span><span class="sxs-lookup"><span data-stu-id="4027d-142">String</span></span> | <span data-ttu-id="4027d-143">内部使用のみ。</span><span class="sxs-lookup"><span data-stu-id="4027d-143">For internal use only.</span></span>|
| <span data-ttu-id="4027d-144">uniqueIdType</span><span class="sxs-lookup"><span data-stu-id="4027d-144">uniqueIdType</span></span> | <span data-ttu-id="4027d-145">String</span><span class="sxs-lookup"><span data-stu-id="4027d-145">String</span></span> | <span data-ttu-id="4027d-146">内部使用のみ。</span><span class="sxs-lookup"><span data-stu-id="4027d-146">For internal use only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4027d-147">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4027d-147">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.location"
}-->
```json
{
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "coordinates": {"@odata.type": "microsoft.graph.outlookGeoCoordinates"},
  "displayName": "string",
  "locationEmailAddress": "string",
  "locationUri": "string",
  "locationType": "string",
  "uniqueId": "string",
  "uniqueIdType": "string"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "location resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
