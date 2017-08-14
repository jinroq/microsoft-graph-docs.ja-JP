<span data-ttu-id="db64c-p102">成功した場合、このメソッドは `204, No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="db64c-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

成功した場合、このメソッドは `204, No Content` 応答コードを返します。応答本文には何も返されません。

## <a name="example"></a><span data-ttu-id="db64c-123">例</span><span class="sxs-lookup"><span data-stu-id="db64c-123">Example</span></span>
##### <a name="request"></a><span data-ttu-id="db64c-124">要求</span><span class="sxs-lookup"><span data-stu-id="db64c-124">Request</span></span>
<span data-ttu-id="db64c-125">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="db64c-125">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
"name": "delete_photo"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/photo
```
##### <a name="response"></a><span data-ttu-id="db64c-126">応答</span><span class="sxs-lookup"><span data-stu-id="db64c-126">Response</span></span>
<span data-ttu-id="db64c-127">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="db64c-127">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
