<span data-ttu-id="f3030-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f3030-p102">Bearer token. Required.</span></span>  | ベアラー {トークン}。必須。 |

## <span data-ttu-id="f3030-117">応答</span><span class="sxs-lookup"><span data-stu-id="f3030-117">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="f3030-118">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [subscription](../resources/subscription.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f3030-118">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>
## <span data-ttu-id="f3030-119">例</span><span class="sxs-lookup"><span data-stu-id="f3030-119">Example</span></span>
<a id="example" class="xliff"></a>
##### <span data-ttu-id="f3030-120">要求</span><span class="sxs-lookup"><span data-stu-id="f3030-120">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="f3030-121">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f3030-121">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_subscription"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/subscriptions/{subscriptionId}
Content-type: application/json

{
   "expirationDateTime":"2016-11-22T18:23:45.9356913Z"
}
```

##### <span data-ttu-id="f3030-122">応答</span><span class="sxs-lookup"><span data-stu-id="f3030-122">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="f3030-123">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="f3030-123">Here is an example of the response.</span></span>
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
  "expirationDateTime":"2016-11-22T18:23:45.9356913Z"
}
```


<!-- {
  "type": "#page.annotation",
  "description": "Update subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
