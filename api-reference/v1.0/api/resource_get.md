<span data-ttu-id="6f4e6-p101">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="6f4e6-p101">Bearer {token}. Required.</span></span>  | ベアラー {トークン}。必須。 |

## <a name="request-body"></a><span data-ttu-id="6f4e6-115">要求本文</span><span class="sxs-lookup"><span data-stu-id="6f4e6-115">Request body</span></span>
<span data-ttu-id="6f4e6-116">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="6f4e6-116">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6f4e6-117">応答</span><span class="sxs-lookup"><span data-stu-id="6f4e6-117">Response</span></span>

<span data-ttu-id="6f4e6-118">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で画像またはファイルのバイナリ データを返します。</span><span class="sxs-lookup"><span data-stu-id="6f4e6-118">If successful, this method returns a `200 OK` response code and the image or file binary data in the response body.</span></span>

<span data-ttu-id="6f4e6-119">注:残りのページのコンテンツと同様、画像を取得するには承認が必要となるため、ブラウザーでは画像は直接表示されません。</span><span class="sxs-lookup"><span data-stu-id="6f4e6-119">Note: Images won't render directly in a browser because they require authorization to retrieve them, like the rest of the page content.</span></span>
## <a name="example"></a><span data-ttu-id="6f4e6-120">例</span><span class="sxs-lookup"><span data-stu-id="6f4e6-120">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6f4e6-121">要求</span><span class="sxs-lookup"><span data-stu-id="6f4e6-121">Request</span></span>
<span data-ttu-id="6f4e6-122">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6f4e6-122">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_resource"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/resources/{id}/content
```
##### <a name="response"></a><span data-ttu-id="6f4e6-123">応答</span><span class="sxs-lookup"><span data-stu-id="6f4e6-123">Response</span></span>
<span data-ttu-id="6f4e6-124">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="6f4e6-124">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->
```http
HTTP/1.1 200 OK

...binary data...
```
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.onenoteResource"
} -->

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
