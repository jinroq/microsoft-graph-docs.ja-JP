<span data-ttu-id="82e1e-p101">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="82e1e-p101">Bearer token. Required.</span></span>  | ベアラー {トークン}。必須。 |

## <span data-ttu-id="82e1e-116">要求本文</span><span class="sxs-lookup"><span data-stu-id="82e1e-116">Request body</span></span>
<a id="request-body" class="xliff"></a>
<span data-ttu-id="82e1e-117">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="82e1e-117">Do not supply a request body for this method.</span></span>
## <span data-ttu-id="82e1e-118">応答</span><span class="sxs-lookup"><span data-stu-id="82e1e-118">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="82e1e-119">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [subscription](../resources/subscription.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="82e1e-119">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>
## <span data-ttu-id="82e1e-120">例</span><span class="sxs-lookup"><span data-stu-id="82e1e-120">Example</span></span>
<a id="example" class="xliff"></a>
##### <span data-ttu-id="82e1e-121">要求</span><span class="sxs-lookup"><span data-stu-id="82e1e-121">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="82e1e-122">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="82e1e-122">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}-->
```http
GET https://graph.microsoft.com/v1.0/subscriptions/{subscriptionId}
```
##### <span data-ttu-id="82e1e-123">応答</span><span class="sxs-lookup"><span data-stu-id="82e1e-123">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="82e1e-124">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="82e1e-124">Here is an example of the response.</span></span>
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
