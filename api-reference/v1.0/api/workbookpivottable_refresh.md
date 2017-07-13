<span data-ttu-id="f6fd6-p103">成功した場合、このメソッドは `200, OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="f6fd6-p103">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>
成功した場合、このメソッドは `200, OK` 応答コードを返します。応答本文には何も返されません。

### <span data-ttu-id="f6fd6-119">例</span><span class="sxs-lookup"><span data-stu-id="f6fd6-119">Example</span></span>
<a id="example" class="xliff"></a>
<span data-ttu-id="f6fd6-120">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="f6fd6-120">Here is an example of how to call this API.</span></span>
##### <span data-ttu-id="f6fd6-121">要求</span><span class="sxs-lookup"><span data-stu-id="f6fd6-121">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="f6fd6-122">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f6fd6-122">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookpivottable_refresh"
}-->
```http
POST https://graph.microsoft.com/v1.0/drive/root/workbook/worksheets/{id}/pivotTables/{id}/refresh
```

##### <span data-ttu-id="f6fd6-123">応答</span><span class="sxs-lookup"><span data-stu-id="f6fd6-123">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="f6fd6-124">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="f6fd6-124">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```
