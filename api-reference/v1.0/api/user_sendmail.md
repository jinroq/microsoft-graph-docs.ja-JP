<span data-ttu-id="1643b-p105">成功した場合、このメソッドは `202, Accepted` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="1643b-p105">If successful, this method returns `202, Accepted` response code. It does not return anything in the response body.</span></span>
成功した場合、このメソッドは `202, Accepted` 応答コードを返します。応答本文には何も返されません。

## <span data-ttu-id="1643b-133">例</span><span class="sxs-lookup"><span data-stu-id="1643b-133">Example</span></span>
<a id="example" class="xliff"></a>
<span data-ttu-id="1643b-134">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="1643b-134">Here is an example of how to call this API.</span></span>
##### <span data-ttu-id="1643b-135">要求</span><span class="sxs-lookup"><span data-stu-id="1643b-135">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="1643b-136">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1643b-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_sendmail"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/sendMail
Content-type: application/json
Content-length: 512

{
  "message": {
    "subject": "Meet for lunch?",
    "body": {
      "contentType": "Text",
      "content": "The new cafeteria is open."
    },
    "toRecipients": [
      {
        "emailAddress": {
          "address": "fannyd@contoso.onmicrosoft.com"
        }
      }
    ],
    "ccRecipients": [
      {
        "emailAddress": {
          "address": "danas@contoso.onmicrosoft.com"
        }
      }
    ]
  },
  "saveToSentItems": "false"
}
```

##### <span data-ttu-id="1643b-137">応答</span><span class="sxs-lookup"><span data-stu-id="1643b-137">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="1643b-138">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="1643b-138">Here is an example of the response.</span></span>
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
  "description": "user: sendMail",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
