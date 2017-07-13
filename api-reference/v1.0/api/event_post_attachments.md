<span data-ttu-id="a07ed-p103">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="a07ed-p103">Nature of the data in the body of an entity. Required.</span></span>  | エンティティ本文内のデータの性質です。必須。 |

## <span data-ttu-id="a07ed-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="a07ed-122">Request body</span></span>
<a id="request-body" class="xliff"></a>
<span data-ttu-id="a07ed-123">要求本文で、[attachment](../resources/attachment.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a07ed-123">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>


## <span data-ttu-id="a07ed-124">応答</span><span class="sxs-lookup"><span data-stu-id="a07ed-124">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="a07ed-125">成功した場合、このメソッドは `201, Created` 応答コードと、応答本文で [attachment](../resources/attachment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a07ed-125">If successful, this method returns `201, Created` response code and [attachment](../resources/attachment.md) object in the response body.</span></span>

## <span data-ttu-id="a07ed-126">例 (添付ファイル)</span><span class="sxs-lookup"><span data-stu-id="a07ed-126">Example (file attachment)</span></span>
<a id="example-file-attachment" class="xliff"></a>

##### <span data-ttu-id="a07ed-127">要求</span><span class="sxs-lookup"><span data-stu-id="a07ed-127">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="a07ed-128">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a07ed-128">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_file_attachment_from_event"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events('AAMkAGI1AAAt9AHjAAA=')/attachments 
Content-type: application/json
Content-length: 151

{
    "@odata.type": "#microsoft.graph.fileAttachment",
    "name": "menu.txt",
    "contentBytes": "bWFjIGFuZCBjaGVlc2UgdG9kYXk="   
}
```

<span data-ttu-id="a07ed-129">要求本文で、[Attachment](../resources/attachment.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a07ed-129">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

##### <span data-ttu-id="a07ed-130">応答</span><span class="sxs-lookup"><span data-stu-id="a07ed-130">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="a07ed-131">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="a07ed-131">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP 201 Created
Content-Length: 735

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/events('AAMkAGI1AAAt9AHjAAA%3D')/attachments/$entity",
    "@odata.type":"#microsoft.graph.fileAttachment",
    "id":"AAMkAGI1AAAt9AHjAAABEgAQAEdBogju-MJEu6Ngg-1_W0g=",
    "lastModifiedDateTime":"2017-04-15T03:21:49Z",
    "name":"menu.txt",
    "contentType":"text/plain",
    "size":178,
    "isInline":false,
    "contentId":null,
    "contentLocation":null,
    "contentBytes":"bWFjIGFuZCBjaGVlc2UgdG9kYXk="
}
```

## <span data-ttu-id="a07ed-132">例 (項目の添付ファイル)</span><span class="sxs-lookup"><span data-stu-id="a07ed-132">Example (item attachment)</span></span>
<a id="example-item-attachment" class="xliff"></a>

##### <span data-ttu-id="a07ed-133">要求</span><span class="sxs-lookup"><span data-stu-id="a07ed-133">Request</span></span>
<a id="request" class="xliff"></a>

<span data-ttu-id="a07ed-134">以下は、アイテムの添付ファイルとしてイベントを別のイベントに添付する例です。</span><span class="sxs-lookup"><span data-stu-id="a07ed-134">Here is an example which attaches an event with another event as an item attachment.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_item_attachment_from_event"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events/{AAMkAGI1AAAt9AHjAAA=}/attachments
Content-type: application/json
Content-length: 600

{
  "@odata.type": "#microsoft.graph.itemAttachment",
  "name": "Holiday event", 
  "item": {
        "@odata.type": "microsoft.graph.event",
        "subject": "Discuss gifts for children",
        "body": {
            "contentType": "HTML",
            "content": "Let's look for funding!"
         },
         "start": {
             "dateTime": "2016-12-02T18:00:00",
             "timeZone": "Pacific Standard Time"
          },
          "end": {
             "dateTime": "2016-12-02T19:00:00",
             "timeZone": "Pacific Standard Time"
          }
    }
}
```

##### <span data-ttu-id="a07ed-135">応答</span><span class="sxs-lookup"><span data-stu-id="a07ed-135">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="a07ed-136">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="a07ed-136">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP 201 Created
Content-type: application/json
Content-length: 162

{
    "@odata.context":"https://graph.microsoft.com/api/v1.0/$metadata#me/events('AAMkAGI1AAAt9AHjAAA=')/attachments/$entity",
    "@odata.type":"#microsoft.graph.itemAttachment",
    "@odata.id":"https://graph.microsoft.com/api/v1.0/users('fdcbcf34-2505-4d07-be5b-0a55b699d157@41a5b830-45ac-4f1b-9bfc-baafa3b7db2e')/events('AAMkAGI1AAAt9AHjAAA=')/attachments('AAMkADNkN2Jp5JVnQIe9r0=')",
    "id":"AAMkADNkNJp5JVnQIe9r0=",
    "lastModifiedDateTime":"2016-12-01T22:27:13Z",
    "name":"Holiday event",
    "contentType":null,
    "size":2473,
    "isInline":false
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
