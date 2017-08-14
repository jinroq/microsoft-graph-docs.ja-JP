<span data-ttu-id="39909-p103">成功した場合、このメソッドは `200, OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="39909-p103">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

成功した場合、このメソッドは `200, OK` 応答コードを返します。応答本文には何も返されません。

## <a name="example"></a><span data-ttu-id="39909-129">例</span><span class="sxs-lookup"><span data-stu-id="39909-129">Example</span></span>
<span data-ttu-id="39909-130">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="39909-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="39909-131">要求</span><span class="sxs-lookup"><span data-stu-id="39909-131">Request</span></span>
<span data-ttu-id="39909-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="39909-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "event_snoozereminder"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events/{id}/snoozeReminder
Content-type: application/json
Content-length: 97

{
  "newReminderTime": {
    "dateTime": "dateTime-value",
    "timeZone": "timeZone-value"
  }
}
```

##### <a name="response"></a><span data-ttu-id="39909-133">応答</span><span class="sxs-lookup"><span data-stu-id="39909-133">Response</span></span>
<span data-ttu-id="39909-134">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="39909-134">Here is an example of the response.</span></span>
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
  "description": "event: snoozeReminder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
