<span data-ttu-id="62453-p102">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るには、変更する値のみを含めます。</span><span class="sxs-lookup"><span data-stu-id="62453-p102">In the request body, supply the values for relevant fields to be updated. Existing properties not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance, only include changed values.</span></span>

要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るには、変更する値のみを含めます。

### <a name="response"></a><span data-ttu-id="62453-120">応答</span><span class="sxs-lookup"><span data-stu-id="62453-120">Response</span></span>

<span data-ttu-id="62453-121">成功した場合、このメソッドは `204 No Content` 応答コードを返しますが、応答本文は返しません。</span><span class="sxs-lookup"><span data-stu-id="62453-121">If successful, this method returns a `204 No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="62453-122">例</span><span class="sxs-lookup"><span data-stu-id="62453-122">Example</span></span>
##### <a name="request"></a><span data-ttu-id="62453-123">要求</span><span class="sxs-lookup"><span data-stu-id="62453-123">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_domain"
}-->
```http
PATCH https://graph.microsoft.com/V1.0/domains/contoso.com
Content-type: application/json

{
  "isDefault": true,
  "supportedServices": [
    "Email",
    "OfficeCommunicationsOnline"
  ]
}
```

##### <a name="response"></a><span data-ttu-id="62453-124">応答</span><span class="sxs-lookup"><span data-stu-id="62453-124">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domain"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update domain",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->