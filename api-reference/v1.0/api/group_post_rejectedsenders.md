<span data-ttu-id="6832d-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="6832d-p102">Bearer token. Required.</span></span>  | ベアラー {トークン}。必須。  |

## <span data-ttu-id="6832d-115">要求本文</span><span class="sxs-lookup"><span data-stu-id="6832d-115">Request body</span></span>
<a id="request-body" class="xliff"></a>
<span data-ttu-id="6832d-116">要求の本文で、ユーザーまたはグループのオブジェクトの id を指定します。</span><span class="sxs-lookup"><span data-stu-id="6832d-116">In the request body, supply the id of a user or group object.</span></span>


## <span data-ttu-id="6832d-117">応答</span><span class="sxs-lookup"><span data-stu-id="6832d-117">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="6832d-118">このメソッドは `204, No Content` 応答コードを返し、応答の本文は返しません。</span><span class="sxs-lookup"><span data-stu-id="6832d-118">This method returns `204, No Content` response code and no response body.</span></span>

## <span data-ttu-id="6832d-119">例</span><span class="sxs-lookup"><span data-stu-id="6832d-119">Example</span></span>
<a id="example" class="xliff"></a>
##### <span data-ttu-id="6832d-120">要求</span><span class="sxs-lookup"><span data-stu-id="6832d-120">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="6832d-121">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6832d-121">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/rejectedSenders/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id":"https://graph.microsoft.com/v1.0/users/alexd@contoso.com"
}
```
##### <span data-ttu-id="6832d-122">応答</span><span class="sxs-lookup"><span data-stu-id="6832d-122">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="6832d-123">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="6832d-123">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create rejectedSender",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
