<span data-ttu-id="7f509-p101">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7f509-p101">Bearer token. Required.</span></span>  | ベアラー {トークン}。必須。 |

## <span data-ttu-id="7f509-114">要求本文</span><span class="sxs-lookup"><span data-stu-id="7f509-114">Request body</span></span>
<a id="request-body" class="xliff"></a>
<span data-ttu-id="7f509-115">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="7f509-115">Do not supply a request body for this method.</span></span>
## <span data-ttu-id="7f509-116">応答</span><span class="sxs-lookup"><span data-stu-id="7f509-116">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="7f509-117">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="7f509-117">If successful, this method returns a `204 No Content` response code.</span></span>
## <span data-ttu-id="7f509-118">例</span><span class="sxs-lookup"><span data-stu-id="7f509-118">Example</span></span>
<a id="example" class="xliff"></a>
##### <span data-ttu-id="7f509-119">要求</span><span class="sxs-lookup"><span data-stu-id="7f509-119">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="7f509-120">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7f509-120">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{subscriptionId}
```
##### <span data-ttu-id="7f509-121">応答</span><span class="sxs-lookup"><span data-stu-id="7f509-121">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="7f509-122">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="7f509-122">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription"
} -->
```http
HTTP/1.1 204 No Content
```


<!-- {
  "type": "#page.annotation",
  "description": "Delete subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
