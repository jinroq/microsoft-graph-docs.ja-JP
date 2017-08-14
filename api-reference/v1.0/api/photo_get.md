<span data-ttu-id="dc2ad-p101">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="dc2ad-p101">Bearer {token}. Required.</span></span>  | ベアラー {トークン}。必須。 |

## <a name="request-body"></a><span data-ttu-id="dc2ad-117">要求本文</span><span class="sxs-lookup"><span data-stu-id="dc2ad-117">Request body</span></span>
<span data-ttu-id="dc2ad-118">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="dc2ad-118">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dc2ad-119">応答</span><span class="sxs-lookup"><span data-stu-id="dc2ad-119">Response</span></span>

<span data-ttu-id="dc2ad-120">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で[写真](../resources/photo.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="dc2ad-120">If successful, this method returns a `200 OK` response code and [photo](../resources/photo.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="dc2ad-121">例</span><span class="sxs-lookup"><span data-stu-id="dc2ad-121">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dc2ad-122">要求</span><span class="sxs-lookup"><span data-stu-id="dc2ad-122">Request</span></span>
<span data-ttu-id="dc2ad-123">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="dc2ad-123">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_photo"
}-->
```http
GET https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/photo
```
##### <a name="response"></a><span data-ttu-id="dc2ad-124">応答</span><span class="sxs-lookup"><span data-stu-id="dc2ad-124">Response</span></span>
<span data-ttu-id="dc2ad-125">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="dc2ad-125">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.profilePhoto"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 53

{
  "height": 99,
  "width": 99,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
