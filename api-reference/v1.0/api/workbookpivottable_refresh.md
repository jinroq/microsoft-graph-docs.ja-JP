<span data-ttu-id="3d055-p103">成功した場合、このメソッドは `200, OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="3d055-p103">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

成功した場合、このメソッドは `200, OK` 応答コードを返します。応答本文には何も返されません。

## <a name="example"></a><span data-ttu-id="3d055-119">例</span><span class="sxs-lookup"><span data-stu-id="3d055-119">Example</span></span>
<span data-ttu-id="3d055-120">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="3d055-120">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="3d055-121">要求</span><span class="sxs-lookup"><span data-stu-id="3d055-121">Request</span></span>
<span data-ttu-id="3d055-122">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3d055-122">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookpivottable_refresh"
}-->
```http
POST https://graph.microsoft.com/v1.0/drive/root/workbook/worksheets/{id}/pivotTables/{id}/refresh
```

##### <a name="response"></a><span data-ttu-id="3d055-123">応答</span><span class="sxs-lookup"><span data-stu-id="3d055-123">Response</span></span>
<span data-ttu-id="3d055-124">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="3d055-124">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```
