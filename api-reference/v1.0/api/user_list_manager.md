<span data-ttu-id="607fb-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="607fb-p102">Bearer token. Required.</span></span>  | ベアラー {トークン}。必須。  |
| <span data-ttu-id="607fb-115">Content-Type</span><span class="sxs-lookup"><span data-stu-id="607fb-115">Content-Type</span></span>   | <span data-ttu-id="607fb-116">application/json</span><span class="sxs-lookup"><span data-stu-id="607fb-116">application/json</span></span>  | 

## <span data-ttu-id="607fb-117">要求本文</span><span class="sxs-lookup"><span data-stu-id="607fb-117">Request body</span></span>
<a id="request-body" class="xliff"></a>
<span data-ttu-id="607fb-118">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="607fb-118">Do not supply a request body for this method.</span></span>
## <span data-ttu-id="607fb-119">応答</span><span class="sxs-lookup"><span data-stu-id="607fb-119">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="607fb-120">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="607fb-120">If successful, this method returns a `200 OK` response code and a [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <span data-ttu-id="607fb-121">例</span><span class="sxs-lookup"><span data-stu-id="607fb-121">Example</span></span>
<a id="example" class="xliff"></a>
##### <span data-ttu-id="607fb-122">要求</span><span class="sxs-lookup"><span data-stu-id="607fb-122">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="607fb-123">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="607fb-123">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_manager"
}-->
```http
GET https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/manager
```
##### <span data-ttu-id="607fb-124">応答</span><span class="sxs-lookup"><span data-stu-id="607fb-124">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="607fb-125">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="607fb-125">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "objectType": "User",
  "id": "111048d2-2761-4347-b978-07354283363b",
  "accountEnabled": true,
  "city": "San Diego",
  "country": "United States",
  "department": "Sales & Marketing",
  "displayName": "Sara Davis",
  "givenName": "Sara",
  "jobTitle": "Finance VP",
  "mail": "SaraD@contoso.onmicrosoft.com",
  "mailNickname": "SaraD",
  "state": "CA",
  "streetAddress": "9256 Towne Center Dr., Suite 400",
  "surname": "Davis",
  "usageLocation": "US",
  "userPrincipalName": "SaraD@contoso.onmicrosoft.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List directReports",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
