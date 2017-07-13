<span data-ttu-id="f8ae3-p104">成功した場合、このメソッドは `202, Accepted` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="f8ae3-p104">If successful, this method returns `202, Accepted` response code. It does not return anything in the response body.</span></span>
成功した場合、このメソッドは `202, Accepted` 応答コードを返します。応答本文には何も返されません。

## <span data-ttu-id="f8ae3-127">例</span><span class="sxs-lookup"><span data-stu-id="f8ae3-127">Example</span></span>
<a id="example" class="xliff"></a>
<span data-ttu-id="f8ae3-128">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="f8ae3-128">Here is an example of how to call this API.</span></span>
##### <span data-ttu-id="f8ae3-129">要求</span><span class="sxs-lookup"><span data-stu-id="f8ae3-129">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="f8ae3-130">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f8ae3-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "conversationthread_reply"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/reply
Content-type: application/json
Content-length: 1131

{
  "post": {
    "body": {
      "contentType": "",
      "content": "content-value"
    }
  }
}
```

##### <span data-ttu-id="f8ae3-131">応答</span><span class="sxs-lookup"><span data-stu-id="f8ae3-131">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="f8ae3-132">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="f8ae3-132">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conversationThread: reply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
