<span data-ttu-id="33103-p102">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="33103-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>
要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。

| <span data-ttu-id="33103-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="33103-118">Property</span></span>     | <span data-ttu-id="33103-119">型</span><span class="sxs-lookup"><span data-stu-id="33103-119">Type</span></span>   |<span data-ttu-id="33103-120">説明</span><span class="sxs-lookup"><span data-stu-id="33103-120">Description</span></span>|
|:---------------|:--------|:----------|

## <span data-ttu-id="33103-121">応答</span><span class="sxs-lookup"><span data-stu-id="33103-121">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="33103-122">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された[写真](../resources/photo.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="33103-122">If successful, this method returns a `200 OK` response code and updated [photo](../resources/photo.md) object in the response body.</span></span>
## <span data-ttu-id="33103-123">例</span><span class="sxs-lookup"><span data-stu-id="33103-123">Example</span></span>
<a id="example" class="xliff"></a>
##### <span data-ttu-id="33103-124">要求</span><span class="sxs-lookup"><span data-stu-id="33103-124">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="33103-125">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="33103-125">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_photo"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/photo
Content-type: application/json
Content-length: 53

{
  "height": 99,
  "width": 99,
  "id": "id-value"
}
```
##### <span data-ttu-id="33103-126">応答</span><span class="sxs-lookup"><span data-stu-id="33103-126">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="33103-127">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="33103-127">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.profilePhoto"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 53

{
  "height": 99,
  "width": 99,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
