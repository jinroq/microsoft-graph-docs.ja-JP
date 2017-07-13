<span data-ttu-id="b4f39-p102">成功した場合、このメソッドは `204, No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="b4f39-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>
成功した場合、このメソッドは `204, No Content` 応答コードを返します。応答本文には何も返されません。

## <span data-ttu-id="b4f39-119">例</span><span class="sxs-lookup"><span data-stu-id="b4f39-119">Example</span></span>
<a id="example" class="xliff"></a>
##### <span data-ttu-id="b4f39-120">要求</span><span class="sxs-lookup"><span data-stu-id="b4f39-120">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="b4f39-121">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b4f39-121">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_mailfolder"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/mailFolders/{id}
```
##### <span data-ttu-id="b4f39-122">応答</span><span class="sxs-lookup"><span data-stu-id="b4f39-122">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="b4f39-123">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="b4f39-123">Here is an example of the response.</span></span> 
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
  "description": "Delete mailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->