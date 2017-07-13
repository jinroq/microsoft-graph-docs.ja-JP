<span data-ttu-id="2e8cb-p105">成功した場合、このメソッドは `204, No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="2e8cb-p105">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>
成功した場合、このメソッドは `204, No Content` 応答コードを返します。応答本文には何も返されません。

## <span data-ttu-id="2e8cb-156">例</span><span class="sxs-lookup"><span data-stu-id="2e8cb-156">Example</span></span>
<a id="example" class="xliff"></a>
##### <span data-ttu-id="2e8cb-157">要求</span><span class="sxs-lookup"><span data-stu-id="2e8cb-157">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="2e8cb-158">最初の例では、名前で拡張情報を参照し、指定されたメッセージの拡張情報を削除します。</span><span class="sxs-lookup"><span data-stu-id="2e8cb-158">The first example references an extension by its name and deletes the extension in the specified message.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_opentypeextension"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions('Com.Contoso.Referral')
```

<span data-ttu-id="2e8cb-159">2 番目の例では、指定されたグループ イベントの拡張機能を削除します。</span><span class="sxs-lookup"><span data-stu-id="2e8cb-159">The second example deletes an extension in the specified group event.</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE https://graph.microsoft.com/v1.0/groups('f5480dfd-7d77-4d0b-ba2e-3391953cc74a')/events('AAMkADVlN17IsAAA=')/extensions('Com.Contoso.Referral')
```

 

##### <span data-ttu-id="2e8cb-160">応答</span><span class="sxs-lookup"><span data-stu-id="2e8cb-160">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="2e8cb-161">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="2e8cb-161">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete opentypeextension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->