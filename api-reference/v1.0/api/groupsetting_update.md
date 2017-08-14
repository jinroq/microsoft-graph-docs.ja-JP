<span data-ttu-id="07958-p102">更新された値のセットです。注:コレクション セット全体を指定する必要があります。単一の値のセットを更新することはできません。</span><span class="sxs-lookup"><span data-stu-id="07958-p102">The updated set of values.  NOTE: You must supply the entire collection set. You cannot update a single set of values.</span></span> | 更新された値のセットです。注:コレクション セット全体を指定する必要があります。単一の値のセットを更新することはできません。 |

## <a name="response"></a><span data-ttu-id="07958-126">応答</span><span class="sxs-lookup"><span data-stu-id="07958-126">Response</span></span>

<span data-ttu-id="07958-127">成功した場合、このメソッドは `204 OK` 応答コードと、応答本文で、更新された [groupSetting](../resources/groupsetting.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="07958-127">If successful, this method returns a `204 OK` response code and [directoryObject](../resources/groupsetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="07958-128">例</span><span class="sxs-lookup"><span data-stu-id="07958-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="07958-129">要求</span><span class="sxs-lookup"><span data-stu-id="07958-129">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_groupsetting"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/groupSettings/{id}
Content-type: application/json
Content-length: 173

{
  "displayName": "displayName-value",
  "templateId": "templateId-value",
  "values": [
    {
      "name": "name-value",
      "value": "value-value"
    }
  ]
}
```
##### <a name="response"></a><span data-ttu-id="07958-130">応答</span><span class="sxs-lookup"><span data-stu-id="07958-130">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSetting"
} -->
```http
HTTP/1.1 204 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update groupSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->