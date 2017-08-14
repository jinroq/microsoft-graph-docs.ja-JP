<span data-ttu-id="76aee-p103">成功した場合、このメソッドは `200, OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="76aee-p103">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

成功した場合、このメソッドは `200, OK` 応答コードを返します。応答本文には何も返されません。

## <a name="example"></a><span data-ttu-id="76aee-125">例</span><span class="sxs-lookup"><span data-stu-id="76aee-125">Example</span></span>
<span data-ttu-id="76aee-126">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="76aee-126">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="76aee-127">要求</span><span class="sxs-lookup"><span data-stu-id="76aee-127">Request</span></span>
<span data-ttu-id="76aee-128">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="76aee-128">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheetprotection_unprotect"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/protection/unprotect
Content-type: application/json
Content-length: 34

{
  "password": "password-value"
}
```

##### <a name="response"></a><span data-ttu-id="76aee-129">応答</span><span class="sxs-lookup"><span data-stu-id="76aee-129">Response</span></span>
<span data-ttu-id="76aee-130">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="76aee-130">Here is an example of the response.</span></span> 
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
  "description": "WorksheetProtection: unprotect",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->