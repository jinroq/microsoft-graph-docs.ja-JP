<span data-ttu-id="78351-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="78351-p103">Bearer {token}. Required.</span></span> | ベアラー {トークン}。必須。 |


## <span data-ttu-id="78351-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="78351-128">Request body</span></span>
<a id="request-body" class="xliff"></a>
<span data-ttu-id="78351-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="78351-129">Do not supply a request body for this method.</span></span>

## <span data-ttu-id="78351-130">応答</span><span class="sxs-lookup"><span data-stu-id="78351-130">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="78351-131">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [driveItem](../resources/driveitem.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="78351-131">If successful, this method returns a `200 OK` response code and a [driveItem](../resources/driveitem.md) object in the response body.</span></span>

## <span data-ttu-id="78351-132">例</span><span class="sxs-lookup"><span data-stu-id="78351-132">Example</span></span>
<a id="example" class="xliff"></a>

##### <span data-ttu-id="78351-133">要求</span><span class="sxs-lookup"><span data-stu-id="78351-133">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="78351-134">以下はユーザーのドライブの要求例です。</span><span class="sxs-lookup"><span data-stu-id="78351-134">Here is an example of the request for the user's drives.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_drive_special"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/special/{name}
```

##### <span data-ttu-id="78351-135">応答</span><span class="sxs-lookup"><span data-stu-id="78351-135">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="78351-136">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="78351-136">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.driveItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "folder": { },
  "id": "s!lkjqwlkj124912049an",
  "name": "Photos",
  "specialFolder": { "name": "photos" },
  "webUrl": "https://contoso-my.sharepoint.com/personal/rgregg_contoso_com/Documents/Photos",
}
```

## <span data-ttu-id="78351-137">注釈</span><span class="sxs-lookup"><span data-stu-id="78351-137">Remarks</span></span>
<a id="remarks" class="xliff"></a>

<span data-ttu-id="78351-138">特殊フォルダーの子を要求する場合は、`children` コレクションを要求するか、子コレクションを展開する [expand](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) オプションを使用します。</span><span class="sxs-lookup"><span data-stu-id="78351-138">To request the children of a special folder, you can request the `children` collection or use the [expand](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) option to expand the children collection.</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "List drives",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Drive/Get special folder"
}-->
