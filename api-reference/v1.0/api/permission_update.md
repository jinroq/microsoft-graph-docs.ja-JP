<span data-ttu-id="4e888-p101">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="4e888-p101">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>
要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。

| <span data-ttu-id="4e888-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4e888-120">Property</span></span>     | <span data-ttu-id="4e888-121">型</span><span class="sxs-lookup"><span data-stu-id="4e888-121">Type</span></span>   | <span data-ttu-id="4e888-122">説明</span><span class="sxs-lookup"><span data-stu-id="4e888-122">Description</span></span>                   |
|:-------------|:-------|:------------------------------|
| <span data-ttu-id="4e888-123">**roles**</span><span class="sxs-lookup"><span data-stu-id="4e888-123">**roles**</span></span>    | <span data-ttu-id="4e888-124">String</span><span class="sxs-lookup"><span data-stu-id="4e888-124">String</span></span> | <span data-ttu-id="4e888-125">アクセス許可の種類の配列。</span><span class="sxs-lookup"><span data-stu-id="4e888-125">An array of permission types.</span></span> |

## <a name="response"></a><span data-ttu-id="4e888-126">応答</span><span class="sxs-lookup"><span data-stu-id="4e888-126">Response</span></span>

<span data-ttu-id="4e888-127">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された[アクセス許可](../resources/permission.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="4e888-127">If successful, this method returns a `200 OK` response code and updated [permission](../resources/permission.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4e888-128">例</span><span class="sxs-lookup"><span data-stu-id="4e888-128">Example</span></span>

##### <a name="request"></a><span data-ttu-id="4e888-129">要求</span><span class="sxs-lookup"><span data-stu-id="4e888-129">Request</span></span>

<span data-ttu-id="4e888-130">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4e888-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_permission"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{item-id}/permissions/{perm-id}
Content-type: application/json

{
  "roles": [ "read" ]
}
```
##### <a name="response"></a><span data-ttu-id="4e888-131">応答</span><span class="sxs-lookup"><span data-stu-id="4e888-131">Response</span></span>

<span data-ttu-id="4e888-132">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="4e888-132">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permission"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "grantedTo": {
    "user": {
      "displayName": "Ryan Gregg",
      "id": "efee1b77-fb3b-4f65-99d6-274c11914d12"
    }
  },
  "id": "1",
  "roles": [ "read" ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update permission",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Update permission"
}-->
