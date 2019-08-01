---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: ファイルをダウンロードする
localization_priority: Priority
ms.prod: sharepoint
description: DriveItem のプライマリ ストリーム (ファイル) のコンテンツをダウンロードします。 file プロパティを持つ driveItem のみがダウンロード可能です。
doc_type: apiPageType
ms.openlocfilehash: 97ea17f8cfe6ac8230d91cc6e4ac6995b3512e90
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36015489"
---
# <a name="download-the-contents-of-a-driveitem"></a><span data-ttu-id="73083-104">DriveItem のコンテンツをダウンロードする</span><span class="sxs-lookup"><span data-stu-id="73083-104">Download the contents of a DriveItem</span></span>

<span data-ttu-id="73083-105">DriveItem のプライマリ ストリーム (ファイル) のコンテンツをダウンロードします。</span><span class="sxs-lookup"><span data-stu-id="73083-105">Download the contents of the primary stream (file) of a DriveItem.</span></span> <span data-ttu-id="73083-106">**file** プロパティを持つ driveItem のみがダウンロード可能です。</span><span class="sxs-lookup"><span data-stu-id="73083-106">Only driveItems with the **file** property can be downloaded.</span></span>

## <a name="permissions"></a><span data-ttu-id="73083-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="73083-107">Permissions</span></span>

<span data-ttu-id="73083-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="73083-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73083-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="73083-110">Permission type</span></span>      | <span data-ttu-id="73083-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="73083-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="73083-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="73083-112">Delegated (work or school account)</span></span> | <span data-ttu-id="73083-113">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73083-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="73083-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="73083-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="73083-115">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73083-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="73083-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="73083-116">Application</span></span> | <span data-ttu-id="73083-117">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73083-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="73083-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="73083-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/content
GET /groups/{group-id}/drive/items/{item-id}/content
GET /me/drive/root:/{item-path}:/content
GET /me/drive/items/{item-id}/content
GET /sites/{siteId}/drive/items/{item-id}/content
GET /users/{userId}/drive/items/{item-id}/content
```

## <a name="optional-request-headers"></a><span data-ttu-id="73083-119">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="73083-119">Optional request headers</span></span>

| <span data-ttu-id="73083-120">名前</span><span class="sxs-lookup"><span data-stu-id="73083-120">Name</span></span>          | <span data-ttu-id="73083-121">値</span><span class="sxs-lookup"><span data-stu-id="73083-121">Value</span></span>  | <span data-ttu-id="73083-122">説明</span><span class="sxs-lookup"><span data-stu-id="73083-122">Description</span></span>                                                                                                                                              |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="73083-123">if-none-match</span><span class="sxs-lookup"><span data-stu-id="73083-123">if-none-match</span></span> | <span data-ttu-id="73083-124">String</span><span class="sxs-lookup"><span data-stu-id="73083-124">String</span></span> | <span data-ttu-id="73083-125">この要求ヘッダーが含まれている場合、指定された eTag (または cTag) がファイルの現在のタグに一致すると、`HTTP 304 Not Modified` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="73083-125">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="example"></a><span data-ttu-id="73083-126">例</span><span class="sxs-lookup"><span data-stu-id="73083-126">Example</span></span>

<span data-ttu-id="73083-127">完全なファイルをダウンロードする例を示します。</span><span class="sxs-lookup"><span data-stu-id="73083-127">Here is an example to download a complete file.</span></span>



# <a name="httptabhttp"></a>[<span data-ttu-id="73083-128">HTTP</span><span class="sxs-lookup"><span data-stu-id="73083-128">--Http</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "download-item-content", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/content
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="73083-129">C#</span><span class="sxs-lookup"><span data-stu-id="73083-129">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/download-item-content-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="73083-130">Javascript</span><span class="sxs-lookup"><span data-stu-id="73083-130">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/download-item-content-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="73083-131">Objective-C</span><span class="sxs-lookup"><span data-stu-id="73083-131">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/download-item-content-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="73083-132">Java</span><span class="sxs-lookup"><span data-stu-id="73083-132">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/download-item-content-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="73083-133">応答</span><span class="sxs-lookup"><span data-stu-id="73083-133">Response</span></span>

<span data-ttu-id="73083-p104">ファイルの事前認証されたダウンロード URL にリダイレクトする、`302 Found` 応答を返します。これは、DriveItem の `@microsoft.graph.downloadUrl` プロパティを通じて使用可能な URL と同じものです。</span><span class="sxs-lookup"><span data-stu-id="73083-p104">Returns a `302 Found` response redirecting to a pre-authenticated download URL for the file. This is the same URL available through the `@microsoft.graph.downloadUrl` property on the DriveItem.</span></span>

<span data-ttu-id="73083-136">ファイルのコンテンツをダウンロードするには、アプリケーションで応答の `Location` ヘッダーに従う必要があります。</span><span class="sxs-lookup"><span data-stu-id="73083-136">To download the contents of the file your application will need to follow the `Location` header in the response.</span></span>
<span data-ttu-id="73083-137">多くの HTTP クライアント ライブラリは、自動的に 302 リダイレクションに従い、即座にファイルのダウンロードを開始します。</span><span class="sxs-lookup"><span data-stu-id="73083-137">Many HTTP client libraries will automatically follow the 302 redirection and start downloading the file immediately.</span></span>

<span data-ttu-id="73083-138">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、ダウンロードのために `Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="73083-138">Pre-authenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to download.</span></span>

<!-- { "blockType": "response", "@odata.type": "stream" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

## <a name="partial-range-downloads"></a><span data-ttu-id="73083-139">部分的な範囲のダウンロード</span><span class="sxs-lookup"><span data-stu-id="73083-139">Partial range downloads</span></span>

<span data-ttu-id="73083-p106">ファイルから部分的なバイトの範囲をダウンロードするには、[RFC 2616](https://www.ietf.org/rfc/rfc2616.txt) で規定されているように、アプリで `Range` ヘッダーを使用します。`Range` ヘッダーは実際の `@microsoft.graph.downloadUrl` URL に追加する必要があり、`/content` の要求には追加しない点に注意してください。</span><span class="sxs-lookup"><span data-stu-id="73083-p106">To download a partial range of bytes from the file, your app can use the `Range` header as specified in [RFC 2616](https://www.ietf.org/rfc/rfc2616.txt). Note that you must append the `Range` header to the actual `@microsoft.graph.downloadUrl` URL and not to the request for `/content`.</span></span>

<!-- { "blockType": "request", "opaqueUrl": true, "name": "download-item-partial", "scopes": "files.read" } -->

```http
GET https://b0mpua-by3301.files.1drv.com/y23vmag
Range: bytes=0-1023
```

<span data-ttu-id="73083-p107">これにより、ファイルからのバイトの要求範囲を含む `HTTP 206 Partial Content` 応答が返されます。範囲が生成できない場合、Range ヘッダーは無視され、ファイルの完全なコンテンツを含む `HTTP 200` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="73083-p107">This will return an `HTTP 206 Partial Content` response with the request range of bytes from the file. If the range cannot be generated the Range header may be ignored and an `HTTP 200` response would be returned with the full contents of the file.</span></span>

<!-- { "blockType": "response", "name": "download-item-partial", "@odata.type": "stream" } -->

```http
HTTP/1.1 206 Partial Content
Content-Range: bytes 0-1023/2048
Content-Type: application/octet-stream

<first 1024 bytes of file>
```

### <a name="error-responses"></a><span data-ttu-id="73083-144">エラー応答</span><span class="sxs-lookup"><span data-stu-id="73083-144">Error responses</span></span>

<span data-ttu-id="73083-145">エラーがどのように返されるかについては、「[エラー応答][error-response]」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="73083-145">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Download the contents of a DriveItem.",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Items/Download",
  "suppressions": [
  ]
} -->
