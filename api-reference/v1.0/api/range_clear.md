<span data-ttu-id="daad2-p103">成功した場合、このメソッドは `200, OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="daad2-p103">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>
成功した場合、このメソッドは `200, OK` 応答コードを返します。応答本文には何も返されません。

## <span data-ttu-id="daad2-126">例</span><span class="sxs-lookup"><span data-stu-id="daad2-126">Example</span></span>
<a id="example" class="xliff"></a>
<span data-ttu-id="daad2-127">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="daad2-127">Here is an example of how to call this API.</span></span>
##### <span data-ttu-id="daad2-128">要求</span><span class="sxs-lookup"><span data-stu-id="daad2-128">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="daad2-129">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="daad2-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_clear"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/clear
Content-type: application/json
Content-length: 32

{
  "applyTo": "applyTo-value"
}
```

##### <span data-ttu-id="daad2-130">応答</span><span class="sxs-lookup"><span data-stu-id="daad2-130">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="daad2-131">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="daad2-131">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->