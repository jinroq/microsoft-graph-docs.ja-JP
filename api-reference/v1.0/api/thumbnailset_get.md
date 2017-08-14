<span data-ttu-id="1a439-p101">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="1a439-p101">Bearer {token}. Required.</span></span>  | ベアラー {トークン}。必須。 |


## <a name="request-body"></a><span data-ttu-id="1a439-118">要求本文</span><span class="sxs-lookup"><span data-stu-id="1a439-118">Request body</span></span>
<span data-ttu-id="1a439-119">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="1a439-119">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1a439-120">応答</span><span class="sxs-lookup"><span data-stu-id="1a439-120">Response</span></span>

<span data-ttu-id="1a439-121">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [thumbnailSet](../resources/thumbnailset.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="1a439-121">If successful, this method returns a `200 OK` response code and [thumbnailSet](../resources/thumbnailset.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1a439-122">例</span><span class="sxs-lookup"><span data-stu-id="1a439-122">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1a439-123">要求</span><span class="sxs-lookup"><span data-stu-id="1a439-123">Request</span></span>
<span data-ttu-id="1a439-124">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1a439-124">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_thumbnailset"
}-->
```http
GET https://graph.microsoft.com/v1.0/drive/root/thumbnails/{id}
```
##### <a name="response"></a><span data-ttu-id="1a439-125">応答</span><span class="sxs-lookup"><span data-stu-id="1a439-125">Response</span></span>
<span data-ttu-id="1a439-126">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="1a439-126">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.thumbnailSet"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 456

{
  "id": "id-value",
  "large": {
    "height": 99,
    "url": "url-value",
    "width": 99
  },
  "medium": {
    "height": 99,
    "url": "url-value",
    "width": 99
  },
  "small": {
    "height": 99,
    "url": "url-value",
    "width": 99
  },
  "source": {
    "height": 99,
    "url": "url-value",
    "width": 99
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get thumbnailSet",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
