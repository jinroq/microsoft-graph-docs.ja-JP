# <a name="get-subscription"></a><span data-ttu-id="12754-101">サブスクリプションを取得する</span><span class="sxs-lookup"><span data-stu-id="12754-101">Get subscription</span></span>

<span data-ttu-id="12754-102">サブスクリプションのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="12754-102">Retrieve the properties and relationships of a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="12754-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="12754-103">Permissions</span></span>

<span data-ttu-id="12754-p101">次の表に、各リソースに必要な、推奨されるアクセス許可を示します。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="12754-p101">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="12754-106">リソースの種類/項目</span><span class="sxs-lookup"><span data-stu-id="12754-106">Resource type / Item</span></span>        | <span data-ttu-id="12754-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="12754-107">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="12754-108">連絡先</span><span class="sxs-lookup"><span data-stu-id="12754-108">Contacts</span></span>                    | <span data-ttu-id="12754-109">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="12754-109">Contacts.Read</span></span>       |
| <span data-ttu-id="12754-110">スレッド</span><span class="sxs-lookup"><span data-stu-id="12754-110">Conversations</span></span>               | <span data-ttu-id="12754-111">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="12754-111">Group.Read.All</span></span>      |
| <span data-ttu-id="12754-112">イベント</span><span class="sxs-lookup"><span data-stu-id="12754-112">Events</span></span>                      | <span data-ttu-id="12754-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="12754-113">Calendars.Read</span></span>      |
| <span data-ttu-id="12754-114">メッセージ</span><span class="sxs-lookup"><span data-stu-id="12754-114">Messages</span></span>                    | <span data-ttu-id="12754-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="12754-115">Mail.Read</span></span>           |
| <span data-ttu-id="12754-116">Groups</span><span class="sxs-lookup"><span data-stu-id="12754-116">Groups</span></span>                      | <span data-ttu-id="12754-117">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="12754-117">Group.Read.All</span></span>      |
| <span data-ttu-id="12754-118">Users</span><span class="sxs-lookup"><span data-stu-id="12754-118">Users</span></span>                       | <span data-ttu-id="12754-119">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="12754-119">User.Read.All</span></span>       |
| <span data-ttu-id="12754-120">ドライブ (ユーザーの OneDrive)</span><span class="sxs-lookup"><span data-stu-id="12754-120">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="12754-121">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="12754-121">Files.ReadWrite</span></span>     |
| <span data-ttu-id="12754-122">ドライブ (共有、SharePoint コンテンツおよびドライブ)</span><span class="sxs-lookup"><span data-stu-id="12754-122">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="12754-123">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12754-123">Files.ReadWrite.All</span></span> |
|<span data-ttu-id="12754-124">セキュリティの警告</span><span class="sxs-lookup"><span data-stu-id="12754-124">Security alert</span></span>| <span data-ttu-id="12754-125">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12754-125">SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="12754-126">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="12754-126">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="12754-127">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="12754-127">Optional query parameters</span></span>

<span data-ttu-id="12754-128">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="12754-128">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="12754-129">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="12754-129">Request headers</span></span>

| <span data-ttu-id="12754-130">名前</span><span class="sxs-lookup"><span data-stu-id="12754-130">Name</span></span>       | <span data-ttu-id="12754-131">型</span><span class="sxs-lookup"><span data-stu-id="12754-131">Type</span></span> | <span data-ttu-id="12754-132">説明</span><span class="sxs-lookup"><span data-stu-id="12754-132">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="12754-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="12754-133">Authorization</span></span>  | <span data-ttu-id="12754-134">string</span><span class="sxs-lookup"><span data-stu-id="12754-134">string</span></span>  | <span data-ttu-id="12754-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="12754-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="12754-137">要求本文</span><span class="sxs-lookup"><span data-stu-id="12754-137">Request body</span></span>

<span data-ttu-id="12754-138">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="12754-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="12754-139">応答</span><span class="sxs-lookup"><span data-stu-id="12754-139">Response</span></span>

<span data-ttu-id="12754-140">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [subscription](../resources/subscription.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="12754-140">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12754-141">例</span><span class="sxs-lookup"><span data-stu-id="12754-141">Example</span></span>

##### <a name="request"></a><span data-ttu-id="12754-142">要求</span><span class="sxs-lookup"><span data-stu-id="12754-142">Request</span></span>

<span data-ttu-id="12754-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="12754-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}-->

```http
GET https://graph.microsoft.com/v1.0/subscriptions/{id}
```

##### <a name="response"></a><span data-ttu-id="12754-144">応答</span><span class="sxs-lookup"><span data-stu-id="12754-144">Response</span></span>

<span data-ttu-id="12754-145">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="12754-145">Here is an example of the response.</span></span>
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
  "applicationId" : "string",
  "changeType":"created,updated",
  "clientState":"secretClientValue",
  "notificationUrl":"https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime":"2016-11-20T18:23:45.9356913Z",
  "creatorId": "string"
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
