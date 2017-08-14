<span data-ttu-id="1bf4b-p103">成功した場合、このメソッドは `204, No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="1bf4b-p103">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

成功した場合、このメソッドは `204, No Content` 応答コードを返します。応答本文には何も返されません。

## <a name="example"></a><span data-ttu-id="1bf4b-130">例</span><span class="sxs-lookup"><span data-stu-id="1bf4b-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1bf4b-131">要求</span><span class="sxs-lookup"><span data-stu-id="1bf4b-131">Request</span></span>
<span data-ttu-id="1bf4b-132">以下は、イベントの添付ファイルを削除する要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1bf4b-132">Here is an example of the request to delete an attachment on an event.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_attachment"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/events/{id}/attachments/{id}
```
##### <a name="response"></a><span data-ttu-id="1bf4b-133">応答</span><span class="sxs-lookup"><span data-stu-id="1bf4b-133">Response</span></span>
<span data-ttu-id="1bf4b-134">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="1bf4b-134">Here is an example of the response.</span></span>
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
  "description": "Delete attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
