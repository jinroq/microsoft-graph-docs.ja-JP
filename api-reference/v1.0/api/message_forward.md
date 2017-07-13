<span data-ttu-id="02bb9-p105">成功した場合、このメソッドは `202, Accepted` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="02bb9-p105">If successful, this method returns `202, Accepted` response code. It does not return anything in the response body.</span></span>
成功した場合、このメソッドは `202, Accepted` 応答コードを返します。応答本文には何も返されません。

## <span data-ttu-id="02bb9-134">例</span><span class="sxs-lookup"><span data-stu-id="02bb9-134">Example</span></span>
<a id="example" class="xliff"></a>
<span data-ttu-id="02bb9-135">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="02bb9-135">Here is an example of how to call this API.</span></span>
##### <span data-ttu-id="02bb9-136">要求</span><span class="sxs-lookup"><span data-stu-id="02bb9-136">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="02bb9-137">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="02bb9-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_forward"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/forward
Content-type: application/json
Content-length: 166

{
  "comment": "comment-value",
  "toRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ]
}
```

##### <span data-ttu-id="02bb9-138">応答</span><span class="sxs-lookup"><span data-stu-id="02bb9-138">Response</span></span>
<a id="response" class="xliff"></a>
##### <span data-ttu-id="02bb9-139">応答</span><span class="sxs-lookup"><span data-stu-id="02bb9-139">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="02bb9-140">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="02bb9-140">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: forward",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
