<span data-ttu-id="d2f96-p105">成功した場合、このメソッドは `202 Accepted` 応答コードと `Operation-Location` ヘッダーを返します。Operation-Location エンドポイントをポーリングして、[コピー操作の状態を取得します](onenoteoperation_get.md)。</span><span class="sxs-lookup"><span data-stu-id="d2f96-p105">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header. Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation_get.md).</span></span>
成功した場合、このメソッドは `202 Accepted` 応答コードと `Operation-Location` ヘッダーを返します。Operation-Location エンドポイントをポーリングして、[コピー操作の状態を取得します](onenoteoperation_get.md)。

## <span data-ttu-id="d2f96-138">例</span><span class="sxs-lookup"><span data-stu-id="d2f96-138">Example</span></span>
<a id="example" class="xliff"></a>
<span data-ttu-id="d2f96-139">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="d2f96-139">Here is an example of how to call this API.</span></span>
##### <span data-ttu-id="d2f96-140">要求</span><span class="sxs-lookup"><span data-stu-id="d2f96-140">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="d2f96-141">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d2f96-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "section_copytosectiongroup"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/sections/{id}/copyToSectionGroup
Content-type: application/json
Content-length: 84

{
  "id": "id-value",
  "groupId": "groupId-value",
  "renameAs": "renameAs-value"
}
```

##### <span data-ttu-id="d2f96-142">応答</span><span class="sxs-lookup"><span data-stu-id="d2f96-142">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="d2f96-143">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="d2f96-143">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteOperation"
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "section: copyToSectionGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->