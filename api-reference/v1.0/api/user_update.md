<span data-ttu-id="7a07f-p123">ディレクトリ内のユーザーの種類を分類するために使用する文字列値 (“Member”、“Guest” など)。$filter をサポートします。</span><span class="sxs-lookup"><span data-stu-id="7a07f-p123">A string value that can be used to classify user types in your directory, such as “Member” and “Guest”. Supports $filter.</span></span>|ディレクトリ内のユーザーの種類を分類するために使用する文字列値 (“Member”、“Guest” など)。$filter をサポートします。          |

## <a name="response"></a><span data-ttu-id="7a07f-261">応答</span><span class="sxs-lookup"><span data-stu-id="7a07f-261">Response</span></span>

<span data-ttu-id="7a07f-262">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="7a07f-262">If successful, this method returns a `204 No Content` response code.</span></span>
## <a name="example"></a><span data-ttu-id="7a07f-263">例</span><span class="sxs-lookup"><span data-stu-id="7a07f-263">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7a07f-264">要求</span><span class="sxs-lookup"><span data-stu-id="7a07f-264">Request</span></span>
<span data-ttu-id="7a07f-265">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7a07f-265">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_user"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me
Content-type: application/json
Content-length: 491

{
  "accountEnabled": true,
  "assignedLicenses": [
    {
      "disabledPlans": [ "bea13e0c-3828-4daa-a392-28af7ff61a0f" ],
      "skuId": "skuId-value"
    }
  ],
  "assignedPlans": [
    {
      "assignedDateTime": "datetime-value",
      "capabilityStatus": "capabilityStatus-value",
      "service": "service-value",
      "servicePlanId": "bea13e0c-3828-4daa-a392-28af7ff61a0f"
    }
  ],
  "businessPhones": [
    "businessPhones-value"
  ],
  "city": "city-value",
  "companyName": "companyName-value"
}
```
##### <a name="response"></a><span data-ttu-id="7a07f-266">応答</span><span class="sxs-lookup"><span data-stu-id="7a07f-266">Response</span></span>
<span data-ttu-id="7a07f-267">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="7a07f-267">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update user",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
