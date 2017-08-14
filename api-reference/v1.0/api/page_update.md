<span data-ttu-id="05d88-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。PATCH 要求に対して JSON データは返されません。</span><span class="sxs-lookup"><span data-stu-id="05d88-p103">If successful, this method returns a `204 No Content` response code.  No JSON data is returned for a PATCH request.</span></span>
成功した場合、このメソッドは `204 No Content` 応答コードを返します。PATCH 要求に対して JSON データは返されません。
## <a name="example"></a><span data-ttu-id="05d88-123">例</span><span class="sxs-lookup"><span data-stu-id="05d88-123">Example</span></span>
##### <a name="request"></a><span data-ttu-id="05d88-124">要求</span><span class="sxs-lookup"><span data-stu-id="05d88-124">Request</span></span>
<span data-ttu-id="05d88-125">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="05d88-125">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_page"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/onenote/pages/{id}/content
Content-type: application/json
Content-length: 312

[
   {
    'target':'#para-id',
    'action':'insert',
    'position':'before',
    'content':'<img src="image-url-or-part-name" alt="image-alt-text" />'
  }, 
  {
    'target':'#list-id',
    'action':'append',
    'content':'<li>new-page-content</li>'
  }
]
```
##### <a name="response"></a><span data-ttu-id="05d88-126">応答</span><span class="sxs-lookup"><span data-stu-id="05d88-126">Response</span></span>
<span data-ttu-id="05d88-127">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="05d88-127">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenotePage"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update page",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
