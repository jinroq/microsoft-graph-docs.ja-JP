# <a name="download-the-contents-of-a-driveitem"></a><span data-ttu-id="0a680-101">DriveItem のコンテンツをダウンロードする</span><span class="sxs-lookup"><span data-stu-id="0a680-101">Download the contents of a DriveItem</span></span>

<span data-ttu-id="0a680-p101">driveItem のコンテンツをダウンロードします。**file** プロパティを持つ driveItem のみがダウンロード可能です。</span><span class="sxs-lookup"><span data-stu-id="0a680-p101">Download the contents for a driveItem. Only driveItem with the **file** property can be downloaded.</span></span>

## <a name="permissions"></a><span data-ttu-id="0a680-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0a680-104">Permissions</span></span>
<span data-ttu-id="0a680-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0a680-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0a680-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0a680-107">Permission type</span></span>      | <span data-ttu-id="0a680-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0a680-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0a680-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0a680-109">Delegated (work or school account)</span></span> | <span data-ttu-id="0a680-110">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a680-110">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="0a680-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0a680-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0a680-112">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a680-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="0a680-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0a680-113">Application</span></span> | <span data-ttu-id="0a680-114">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a680-114">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0a680-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0a680-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/root:/{item-path}:/content
GET /me/drive/items/{item-id}/content
GET /drives/items/{item-id}/content
GET /groups/{group-id}/drive/items/{item-id}/content
```

## <a name="request-headers"></a><span data-ttu-id="0a680-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0a680-116">Request headers</span></span>

| <span data-ttu-id="0a680-117">名前</span><span class="sxs-lookup"><span data-stu-id="0a680-117">Name</span></span>          | <span data-ttu-id="0a680-118">値</span><span class="sxs-lookup"><span data-stu-id="0a680-118">Value</span></span>  | <span data-ttu-id="0a680-119">説明</span><span class="sxs-lookup"><span data-stu-id="0a680-119">Description</span></span>                                                                                                                                              |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="0a680-120">if-none-match</span><span class="sxs-lookup"><span data-stu-id="0a680-120">if-none-match</span></span> | <span data-ttu-id="0a680-121">String</span><span class="sxs-lookup"><span data-stu-id="0a680-121">String</span></span> | <span data-ttu-id="0a680-122">この要求ヘッダーが含まれている場合、指定された eTag (または cTag) がファイルの現在のタグに一致すると、`HTTP 304 Not Modified` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="0a680-122">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0a680-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="0a680-123">Request body</span></span>
<span data-ttu-id="0a680-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="0a680-124">Do not supply a request body for this method.</span></span>

## <a name="example"></a><span data-ttu-id="0a680-125">例</span><span class="sxs-lookup"><span data-stu-id="0a680-125">Example</span></span>
<span data-ttu-id="0a680-126">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="0a680-126">Here is an example of how to call this API.</span></span>


<!-- { "blockType": "request", "name": "driveitem-download-contents" } -->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{item-id}/content
```

##### <a name="response"></a><span data-ttu-id="0a680-127">応答</span><span class="sxs-lookup"><span data-stu-id="0a680-127">Response</span></span>
<span data-ttu-id="0a680-p103">ファイルの事前認証されたダウンロード URL にリダイレクトする、`302 Found` 応答を返します。これは、DriveItem の `@microsoft.graph.downloadUrl` プロパティを通じて使用可能な URL と同じものです。</span><span class="sxs-lookup"><span data-stu-id="0a680-p103">Returns a `302 Found` response redirecting to a pre-authenticated download URL for the file. This is the same URL available through the `@microsoft.graph.downloadUrl` property on the DriveItem.</span></span>

<span data-ttu-id="0a680-p104">ファイルのコンテンツをダウンロードするには、アプリケーションで応答の `Location` ヘッダーに従う必要があります。多くの HTTP クライアント ライブラリは、自動的に 302 リダイレクションに従い、即座にファイルのダウンロードを開始します。</span><span class="sxs-lookup"><span data-stu-id="0a680-p104">To download the contents of the file your application will need to follow the `Location` header in the response. Many HTTP client libraries will automatically follow the 302 redirection and start downloading the file immedately.</span></span>

<span data-ttu-id="0a680-132">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、ダウンロードのために `Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="0a680-132">Pre-authenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to download.</span></span>

<!-- { "blockType": "response", "@odata.type": "stream" } -->
```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

## <a name="partial-range-downloads"></a><span data-ttu-id="0a680-133">部分的な範囲のダウンロード</span><span class="sxs-lookup"><span data-stu-id="0a680-133">Partial range downloads</span></span>

<span data-ttu-id="0a680-p105">ファイルから部分的なバイトの範囲をダウンロードするには、[RFC 2616](https://www.ietf.org/rfc/rfc2616.txt) で規定されているように、アプリで `Range` ヘッダーを使用します。`Range` ヘッダーは実際の `@microsoft.graph.downloadUrl` URL に追加する必要があり、`/content` の要求には追加しない点に注意してください。</span><span class="sxs-lookup"><span data-stu-id="0a680-p105">To download a partial range of bytes from the file, your app can use the `Range` header as specified in [RFC 2616](https://www.ietf.org/rfc/rfc2616.txt). Note that you must append the `Range` header to the actual `@microsoft.graph.downloadUrl` URL and not to the request for `/content`.</span></span>

<!-- { "blockType": "request", "name": "driveitem-get-partial-content" } -->
```http
GET https://b0mpua-by3301.files.1drv.com/y23vmag
Range: bytes=0-1023
```

<span data-ttu-id="0a680-p106">これにより、ファイルからのバイトの要求範囲を含む `HTTP 206 Partial Content` 応答が返されます。範囲が生成できない場合、Range ヘッダーは無視され、ファイルの完全なコンテンツを含む `HTTP 200` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="0a680-p106">This will return an `HTTP 206 Partial Content` response with the request range of bytes from the file. If the range cannot be generated the Range header may be ignored and an `HTTP 200` response would be returned with the full contents of the file.</span></span>

<!-- { "blockType": "response", "@odata.type": "stream" } -->
```http
HTTP/1.1 206 Partial Content
Content-Range: bytes 0-1023/2048

<first 1024 bytes of file>
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Download item",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Download file"
}-->
