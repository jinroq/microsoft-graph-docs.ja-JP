<span data-ttu-id="b80f8-p102">成功した場合、このメソッドは `204, No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="b80f8-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

成功した場合、このメソッドは `204, No Content` 応答コードを返します。応答本文には何も返されません。

## <a name="example"></a><span data-ttu-id="b80f8-120">例</span><span class="sxs-lookup"><span data-stu-id="b80f8-120">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b80f8-121">要求</span><span class="sxs-lookup"><span data-stu-id="b80f8-121">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_groupsetting"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groupSettings/{id}
```
##### <a name="response"></a><span data-ttu-id="b80f8-122">応答</span><span class="sxs-lookup"><span data-stu-id="b80f8-122">Response</span></span>
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
  "description": "Delete groupSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->