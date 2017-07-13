<span data-ttu-id="3eecd-p101">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="3eecd-p101">Bearer token. Required.</span></span>  | ベアラー {トークン}。必須。 |
| <span data-ttu-id="3eecd-114">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3eecd-114">Content-Type</span></span>  | <span data-ttu-id="3eecd-115">application/json</span><span class="sxs-lookup"><span data-stu-id="3eecd-115">application/json</span></span>  |

## <span data-ttu-id="3eecd-116">要求本文</span><span class="sxs-lookup"><span data-stu-id="3eecd-116">Request body</span></span>
<a id="request-body" class="xliff"></a>
<span data-ttu-id="3eecd-117">要求本文で、追加する [directoryObject](../resources/directoryobject.md) または[ユーザー](../resources/user.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="3eecd-117">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) or [user](../resources/user.md) object to be added.</span></span>

## <span data-ttu-id="3eecd-118">応答</span><span class="sxs-lookup"><span data-stu-id="3eecd-118">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="3eecd-119">成功した場合、このメソッドは `204, No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="3eecd-119">If successful, this method returns `204, No Content` response code.</span></span>

## <span data-ttu-id="3eecd-120">例</span><span class="sxs-lookup"><span data-stu-id="3eecd-120">Example</span></span>
<a id="example" class="xliff"></a>
##### <span data-ttu-id="3eecd-121">要求</span><span class="sxs-lookup"><span data-stu-id="3eecd-121">Request</span></span>
<a id="request" class="xliff"></a>

<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directoryrole"
}-->
```http
POST https://graph.microsoft.com/v1.0/directoryRoles/{id}/members
Content-type: application/json

{
  "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
}
```

##### <span data-ttu-id="3eecd-122">応答</span><span class="sxs-lookup"><span data-stu-id="3eecd-122">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="3eecd-123">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="3eecd-123">Note: The response object shown here may be truncated for brevity.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
Content-type: text/plain

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->