# <a name="get-subscription"></a><span data-ttu-id="6742b-101">サブスクリプションを取得する</span><span class="sxs-lookup"><span data-stu-id="6742b-101">Get subscription</span></span>

<span data-ttu-id="6742b-102">サブスクリプションのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="6742b-102">Retrieve the properties and relationships of a subscription.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6742b-103">前提条件</span><span class="sxs-lookup"><span data-stu-id="6742b-103">Prerequisites</span></span>

<span data-ttu-id="6742b-104">次の表に、各リソースに必要な、推奨されるアクセス許可を示します。</span><span class="sxs-lookup"><span data-stu-id="6742b-104">The following table lists the suggested permission needed for each resource.</span></span>

| <span data-ttu-id="6742b-105">リソースの種類/項目</span><span class="sxs-lookup"><span data-stu-id="6742b-105">Resource type / Item</span></span>        | <span data-ttu-id="6742b-106">範囲</span><span class="sxs-lookup"><span data-stu-id="6742b-106">Scope</span></span>               |
|-----------------------------|---------------------|
| <span data-ttu-id="6742b-107">連絡先</span><span class="sxs-lookup"><span data-stu-id="6742b-107">Contacts</span></span>                    | <span data-ttu-id="6742b-108">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="6742b-108">Contacts.Read</span></span>       |
| <span data-ttu-id="6742b-109">スレッド</span><span class="sxs-lookup"><span data-stu-id="6742b-109">Conversations</span></span>               | <span data-ttu-id="6742b-110">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="6742b-110">Group.Read.All</span></span>      |
| <span data-ttu-id="6742b-111">イベント</span><span class="sxs-lookup"><span data-stu-id="6742b-111">Events</span></span>                      | <span data-ttu-id="6742b-112">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6742b-112">Calendars.Read</span></span>      |
| <span data-ttu-id="6742b-113">メッセージ</span><span class="sxs-lookup"><span data-stu-id="6742b-113">Messages</span></span>                    | <span data-ttu-id="6742b-114">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="6742b-114">Mail.Read</span></span>           |
| <span data-ttu-id="6742b-115">ドライブ (ユーザーの OneDrive)</span><span class="sxs-lookup"><span data-stu-id="6742b-115">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="6742b-116">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6742b-116">Files.ReadWrite</span></span>     |
| <span data-ttu-id="6742b-117">ドライブ (Sharepoint の共有コンテンツとドライブ)</span><span class="sxs-lookup"><span data-stu-id="6742b-117">Drives (Sharepoint shared content and drives)</span></span> | <span data-ttu-id="6742b-118">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6742b-118">Files.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6742b-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6742b-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /subscriptions/{subscriptionId}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6742b-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="6742b-120">Optional query parameters</span></span>
<span data-ttu-id="6742b-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="6742b-121">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6742b-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6742b-122">Request headers</span></span>
| <span data-ttu-id="6742b-123">名前</span><span class="sxs-lookup"><span data-stu-id="6742b-123">Name</span></span>       | <span data-ttu-id="6742b-124">型</span><span class="sxs-lookup"><span data-stu-id="6742b-124">Type</span></span> | <span data-ttu-id="6742b-125">説明</span><span class="sxs-lookup"><span data-stu-id="6742b-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6742b-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="6742b-126">Authorization</span></span>  | <span data-ttu-id="6742b-127">string</span><span class="sxs-lookup"><span data-stu-id="6742b-127">string</span></span>  | <span data-ttu-id="6742b-p101">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="6742b-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6742b-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="6742b-130">Request body</span></span>
<span data-ttu-id="6742b-131">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="6742b-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6742b-132">応答</span><span class="sxs-lookup"><span data-stu-id="6742b-132">Response</span></span>

<span data-ttu-id="6742b-133">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [subscription](../resources/subscription.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="6742b-133">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6742b-134">例</span><span class="sxs-lookup"><span data-stu-id="6742b-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6742b-135">要求</span><span class="sxs-lookup"><span data-stu-id="6742b-135">Request</span></span>
<span data-ttu-id="6742b-136">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6742b-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}-->
```http
GET https://graph.microsoft.com/v1.0/subscriptions/{subscriptionId}
```
##### <a name="response"></a><span data-ttu-id="6742b-137">応答</span><span class="sxs-lookup"><span data-stu-id="6742b-137">Response</span></span>
<span data-ttu-id="6742b-138">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="6742b-138">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 252

{
  "id":"7f105c7d-2dc5-4530-97cd-4e7ae6534c07",
  "resource":"me/messages",
  "changeType":"created,updated",
  "clientState":"subscription-identifier",
  "notificationUrl":"https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime":"2016-11-20T18:23:45.9356913Z"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
