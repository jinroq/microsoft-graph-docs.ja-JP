<span data-ttu-id="a1ece-p101">[**SharedDriveItem**](../resources/shareddriveitem.md) には、いくつかの有用な情報が含まれていますが、ほとんどのアプリは、共有の [DriveItem](../resources/driveitem.md)に直接アクセスする必要があります。**SharedDriveItem** リソースには、共有アイテムのスコープ内でコンテンツにアクセスできる、**root** と **items** のリレーションシップが含まれています。</span><span class="sxs-lookup"><span data-stu-id="a1ece-p101">While the [**SharedDriveItem**](../resources/shareddriveitem.md) contains some useful information, most apps will want to directly access the shared [DriveItem](../resources/driveitem.md). The **SharedDriveItem** resource includes a **root** and **items** relationships which can access content within the scope of the shared item.</span></span>

[**SharedDriveItem**](../resources/shareddriveitem.md) には、いくつかの有用な情報が含まれていますが、ほとんどのアプリは、共有の [DriveItem](../resources/driveitem.md)に直接アクセスする必要があります。**SharedDriveItem** リソースには、共有アイテムのスコープ内でコンテンツにアクセスできる、**root** と **items** のリレーションシップが含まれています。

### <span data-ttu-id="a1ece-122">例 (単一ファイル)</span><span class="sxs-lookup"><span data-stu-id="a1ece-122">Example (single file)</span></span>
<a id="example-single-file" class="xliff"></a>

##### <span data-ttu-id="a1ece-123">要求</span><span class="sxs-lookup"><span data-stu-id="a1ece-123">Request</span></span>
<a id="request" class="xliff"></a>

<span data-ttu-id="a1ece-124">**root** リレーションシップを要求することで、共有された **DriveItem** が返されます。</span><span class="sxs-lookup"><span data-stu-id="a1ece-124">By requesting the **root** relationship, the **DriveItem** that was shared will be returned.</span></span>

```http
GET https://graph.microsoft.com/v1.0/shares/{shareIdOrUrl}/root
```

##### <span data-ttu-id="a1ece-125">応答</span><span class="sxs-lookup"><span data-stu-id="a1ece-125">Response</span></span>
<a id="response" class="xliff"></a>

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "9FFFDB3C-5B87-4062-9606-1B008CA88E44",
  "name": "contoso project.docx",
  "eTag": "2246BD2D-7811-4660-BD0F-1CF36133677B,1",
  "file": {},
  "size": 109112
}
```

### <span data-ttu-id="a1ece-126">例 (共有フォルダー)</span><span class="sxs-lookup"><span data-stu-id="a1ece-126">Example (shared folder)</span></span>
<a id="example-shared-folder" class="xliff"></a>

##### <span data-ttu-id="a1ece-127">要求</span><span class="sxs-lookup"><span data-stu-id="a1ece-127">Request</span></span>
<a id="request" class="xliff"></a>

<span data-ttu-id="a1ece-128">**root** リレーションシップを要求して、**children** コレクションを展開することで、共有されている **DriveItem** が共有フォルダー内のファイルとともに返されます。</span><span class="sxs-lookup"><span data-stu-id="a1ece-128">By requesting the **root** relationship and expanding the **children** collection, the **DriveItem** that was shared will be returned along with the files within the shared folder.</span></span>

```http
GET https://graph.microsoft.com/v1.0/shares/{shareIdOrUrl}/root?$expand=children
```

##### <span data-ttu-id="a1ece-129">応答</span><span class="sxs-lookup"><span data-stu-id="a1ece-129">Response</span></span>
<a id="response" class="xliff"></a>

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "9FFFDB3C-5B87-4062-9606-1B008CA88E44",
  "name": "Contoso Project",
  "eTag": "2246BD2D-7811-4660-BD0F-1CF36133677B,1",
  "folder": {}
  "size": 10911212,
  "children": [
    {
      "id": "AFBBDD79-868E-452D-AD4D-24697D4A4044",
      "name": "Propsoal.docx",
      "file": {},
      "size": 19001
    },
    {
      "id": "A91FE90A-2F2C-4EE6-B412-C4FFBA3F71A6",
      "name": "Update to Proposal.docx",
      "file": {},
      "size": 91001
    }
  ]
}
```

## <span data-ttu-id="a1ece-130">共有の URL を変換する</span><span class="sxs-lookup"><span data-stu-id="a1ece-130">Transform a sharing URL</span></span>
<a id="transform-a-sharing-url" class="xliff"></a>

<span data-ttu-id="a1ece-131">**shares** API を使用して共有の URL にアクセスするには、URL を共有のトークンに変換する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a1ece-131">To access a sharing URL using the **shares** API, the URL needs to be transformed into a sharing token.</span></span>

<span data-ttu-id="a1ece-132">URL を共有のトークンに変化するには:</span><span class="sxs-lookup"><span data-stu-id="a1ece-132">To transform a URL into a sharing token:</span></span>

1. <span data-ttu-id="a1ece-133">共有の URL を Base64 エンコードします。</span><span class="sxs-lookup"><span data-stu-id="a1ece-133">Base64 encode the sharing URL.</span></span>
2. <span data-ttu-id="a1ece-134">次に示すように、base64 でエンコードしたデータを[パディングされていない base64url 形式](https://en.wikipedia.org/wiki/Base64)に変換します。</span><span class="sxs-lookup"><span data-stu-id="a1ece-134">Convert the base64 encoded data to [unpadded base64url format](https://en.wikipedia.org/wiki/Base64) by:</span></span>
  1. <span data-ttu-id="a1ece-135">文字列から、末尾の `=` 文字をトリミングします。</span><span class="sxs-lookup"><span data-stu-id="a1ece-135">Trim trailing `=` characters from the string</span></span>
  2. <span data-ttu-id="a1ece-136">安全でない URL 文字を同等の文字に置き換えます (`/` を `_` に、`+` を `-` に置換します)。</span><span class="sxs-lookup"><span data-stu-id="a1ece-136">Replace unsafe URL characters with an equivalent character; replace `/` with `_` and `+` with `-`.</span></span>
3. <span data-ttu-id="a1ece-137">文字列の先頭に `u!` を追加します。</span><span class="sxs-lookup"><span data-stu-id="a1ece-137">Append `u!` to the beginning of the string.</span></span>

<span data-ttu-id="a1ece-138">たとえば、次に示す C# メソッドにより、入力文字列を共有のトークンに変換します。</span><span class="sxs-lookup"><span data-stu-id="a1ece-138">For example, the following C# method transforms an input string into a sharing token:</span></span>

```csharp
string UrlToSharingToken(string inputUrl) {
  var base64Value = System.Convert.ToBase64String(System.Text.Encoding.UTF8.GetBytes(inputUrl));
  return "u!" + base64Value.TrimEnd('=').Replace('/','_').Replace('+','-');
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
