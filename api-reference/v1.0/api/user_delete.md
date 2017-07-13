<span data-ttu-id="03b10-p102">成功した場合、このメソッドは `204, No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="03b10-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>
成功した場合、このメソッドは `204, No Content` 応答コードを返します。応答本文には何も返されません。

## <span data-ttu-id="03b10-117">例</span><span class="sxs-lookup"><span data-stu-id="03b10-117">Example</span></span>
<a id="example" class="xliff"></a>
##### <span data-ttu-id="03b10-118">要求</span><span class="sxs-lookup"><span data-stu-id="03b10-118">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="03b10-119">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="03b10-119">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_user"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/users/mba9a3254-9f18-4209-aeb3-9e42a35b5be4
```
##### <span data-ttu-id="03b10-120">応答</span><span class="sxs-lookup"><span data-stu-id="03b10-120">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="03b10-121">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="03b10-121">Here is an example of the response.</span></span> 
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
  "description": "Delete user",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->