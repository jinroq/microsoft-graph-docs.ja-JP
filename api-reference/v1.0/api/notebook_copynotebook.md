<span data-ttu-id="c077e-p106">成功した場合、このメソッドは `202 Accepted` 応答コードと `Operation-Location` ヘッダーを返します。Operation-Location エンドポイントをポーリングして、[コピー操作の状態を取得します](onenoteOperation_get.md)。</span><span class="sxs-lookup"><span data-stu-id="c077e-p106">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header. Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteOperation_get.md).</span></span>
成功した場合、このメソッドは `202 Accepted` 応答コードと `Operation-Location` ヘッダーを返します。Operation-Location エンドポイントをポーリングして、[コピー操作の状態を取得します](onenoteOperation_get.md)。

## <span data-ttu-id="c077e-136">例</span><span class="sxs-lookup"><span data-stu-id="c077e-136">Example</span></span>
<a id="example" class="xliff"></a>
<span data-ttu-id="c077e-137">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="c077e-137">Here is an example of how to call this API.</span></span>
##### <span data-ttu-id="c077e-138">要求</span><span class="sxs-lookup"><span data-stu-id="c077e-138">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="c077e-139">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c077e-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "notebook_copynotebook"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/notebooks/{id}/copyNotebook
Content-type: application/json
Content-length: 108

{
  "groupId": "groupId-value",
  "renameAs": "renameAs-value"
}
```

##### <span data-ttu-id="c077e-140">応答</span><span class="sxs-lookup"><span data-stu-id="c077e-140">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="c077e-141">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="c077e-141">Here is an example of the response.</span></span>
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
  "description": "notebook: copyNotebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
