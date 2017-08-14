<span data-ttu-id="3fba4-p102">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="3fba4-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。

## <a name="example"></a><span data-ttu-id="3fba4-123">例</span><span class="sxs-lookup"><span data-stu-id="3fba4-123">Example</span></span>

##### <a name="request"></a><span data-ttu-id="3fba4-124">要求</span><span class="sxs-lookup"><span data-stu-id="3fba4-124">Request</span></span>

<span data-ttu-id="3fba4-125">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3fba4-125">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_permission"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/drive/root/items/{item-id}/permissions/{perm-id}
```

##### <a name="response"></a><span data-ttu-id="3fba4-126">応答</span><span class="sxs-lookup"><span data-stu-id="3fba4-126">Response</span></span>

<span data-ttu-id="3fba4-127">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="3fba4-127">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="remarks"></a><span data-ttu-id="3fba4-128">備考</span><span class="sxs-lookup"><span data-stu-id="3fba4-128">Remarks</span></span>

* <span data-ttu-id="3fba4-129">`personal` (OneDrive Personal) の **driveType** を持つ[ドライブ](../resources/drive.md)は、DriveItem のルートでの作成やアクセス許可の変更を行えません。</span><span class="sxs-lookup"><span data-stu-id="3fba4-129">[Drives](../resources/drive.md) with a **driveType** of `personal` (OneDrive Personal) cannot create or modify permissions on the root DriveItem.</span></span> 

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete permission",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Delete permission"
}-->
