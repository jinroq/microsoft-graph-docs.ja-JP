<span data-ttu-id="cf4f1-p104">成功した場合、このメソッドは `200, OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="cf4f1-p104">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

成功した場合、このメソッドは `200, OK` 応答コードを返します。応答本文には何も返されません。

## <a name="example"></a><span data-ttu-id="cf4f1-131">例</span><span class="sxs-lookup"><span data-stu-id="cf4f1-131">Example</span></span>
<span data-ttu-id="cf4f1-132">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="cf4f1-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="cf4f1-133">要求</span><span class="sxs-lookup"><span data-stu-id="cf4f1-133">Request</span></span>
<span data-ttu-id="cf4f1-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="cf4f1-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chart_setposition"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/setPosition
Content-type: application/json
Content-length: 66

{
  "startCell": "startCell-value",
  "endCell": "endCell-value"
}
```

##### <a name="response"></a><span data-ttu-id="cf4f1-135">応答</span><span class="sxs-lookup"><span data-stu-id="cf4f1-135">Response</span></span>
<span data-ttu-id="cf4f1-136">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="cf4f1-136">Here is an example of the response.</span></span> 
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
  "description": "Chart: setPosition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->