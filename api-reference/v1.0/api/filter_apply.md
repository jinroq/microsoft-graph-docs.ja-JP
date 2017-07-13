<span data-ttu-id="4b93c-p102">成功した場合、このメソッドは `200, OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="4b93c-p102">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>
成功した場合、このメソッドは `200, OK` 応答コードを返します。応答本文には何も返されません。

## <span data-ttu-id="4b93c-124">例</span><span class="sxs-lookup"><span data-stu-id="4b93c-124">Example</span></span>
<a id="example" class="xliff"></a>
<span data-ttu-id="4b93c-125">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="4b93c-125">Here is an example of how to call this API.</span></span>
##### <span data-ttu-id="4b93c-126">要求</span><span class="sxs-lookup"><span data-stu-id="4b93c-126">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="4b93c-127">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4b93c-127">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "filter_apply"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/filter/apply
Content-type: application/json
Content-length: 321

{
  "criteria": {
    "criterion1": "criterion1-value",
    "criterion2": "criterion2-value",
    "color": "color-value",
    "operator": {
    },
    "icon": {
      "set": "set-value",
      "index": 99
    },
    "dynamicCriteria": "dynamicCriteria-value",
    "values": {
    },
    "filterOn": "filterOn-value"
  }
}
```

##### <span data-ttu-id="4b93c-128">応答</span><span class="sxs-lookup"><span data-stu-id="4b93c-128">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="4b93c-129">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="4b93c-129">Here is an example of the response.</span></span> 
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
  "description": "Filter: apply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->