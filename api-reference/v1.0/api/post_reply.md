<span data-ttu-id="47a14-p103">成功した場合、このメソッドは `200, OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="47a14-p103">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>
成功した場合、このメソッドは `200, OK` 応答コードを返します。応答本文には何も返されません。

## <span data-ttu-id="47a14-125">例</span><span class="sxs-lookup"><span data-stu-id="47a14-125">Example</span></span>
<a id="example" class="xliff"></a>
<span data-ttu-id="47a14-126">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="47a14-126">Here is an example of how to call this API.</span></span>
##### <span data-ttu-id="47a14-127">要求</span><span class="sxs-lookup"><span data-stu-id="47a14-127">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="47a14-128">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="47a14-128">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_reply"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}/reply
Content-type: application/json
Content-length: 1131

{
  "post": {
    "body": {
      "contentType": "",
      "content": "content-value"
    },
    "receivedDateTime": "datetime-value",
    "hasAttachments": true,
    "from": {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    },
    "sender": {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    },
    "conversationThreadId": "conversationThreadId-value",
    "newParticipants": [
      {
        "emailAddress": {
          "name": "name-value",
          "address": "address-value"
        }
      }
    ],
    "conversationId": "conversationId-value",
    "createdDateTime": "datetime-value",
    "lastModifiedDateTime": "datetime-value",
    "changeKey": "changeKey-value",
    "categories": [
      "categories-value"
    ],
    "id": "id-value",
    "inReplyTo": {
    },
    "attachments": [
      {
        "lastModifiedDateTime": "datetime-value",
        "name": "name-value",
        "contentType": "contentType-value",
        "size": 99,
        "isInline": true,
        "id": "id-value"
      }
    ]
  }
}
```

##### <span data-ttu-id="47a14-129">応答</span><span class="sxs-lookup"><span data-stu-id="47a14-129">Response</span></span>
<a id="response" class="xliff"></a>
##### <span data-ttu-id="47a14-130">応答</span><span class="sxs-lookup"><span data-stu-id="47a14-130">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="47a14-131">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="47a14-131">Here is an example of the response.</span></span>
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
  "description": "post: reply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
