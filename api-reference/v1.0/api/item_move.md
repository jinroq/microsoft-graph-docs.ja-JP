<span data-ttu-id="bb478-p103">**注:**OneDrive のルートにアイテムを移動するときには、`"id:" "root"` 構文は使用できません。ルート フォルダーの実際の ID を使用するか、親参照の `{"path": "/drive/root"}` を使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="bb478-p103">**Note:** When moving items to the root of a OneDrive you cannot use the `"id:" "root"` syntax. You either need to use the real ID of the root folder, or use `{"path": "/drive/root"}` for the parent reference.</span></span>

**注:**OneDrive のルートにアイテムを移動するときには、`"id:" "root"` 構文は使用できません。ルート フォルダーの実際の ID を使用するか、親参照の `{"path": "/drive/root"}` を使用する必要があります。

## <span data-ttu-id="bb478-125">応答</span><span class="sxs-lookup"><span data-stu-id="bb478-125">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="bb478-126">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された [DriveItem](../resources/driveitem.md) リソースを返します。</span><span class="sxs-lookup"><span data-stu-id="bb478-126">If successful, this method returns a `200 OK` response code and updated [DriveItem](../resources/driveitem.md) resource in the response body.</span></span>

## <span data-ttu-id="bb478-127">例</span><span class="sxs-lookup"><span data-stu-id="bb478-127">Example</span></span>
<a id="example" class="xliff"></a>
<span data-ttu-id="bb478-128">この例では、{item-id} で指定したアイテムを、ユーザーの OneDrive の **Documents** フォルダーに移動します</span><span class="sxs-lookup"><span data-stu-id="bb478-128">This example moves an item specified by {item-id} into the **Documents** folder in the user's OneDrive.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_item"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{item-id}
Content-type: application/json

{
    "name": "new-item-name",
    "parentReference" : {"path": "/drive/root:/Documents"}
}
```

## <span data-ttu-id="bb478-129">応答</span><span class="sxs-lookup"><span data-stu-id="bb478-129">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="bb478-130">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="bb478-130">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.driveItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "0123456789abc",
    "name": "new-item-name",
    "folder": { "childCount": 3 },
  "parentReference": {
    "id": "507DE6D5-0201-496A-AA87-5E2563247982",
    "path": "/drive/root:/Documents"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Move item",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
