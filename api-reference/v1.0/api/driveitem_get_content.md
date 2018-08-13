---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: ファイルをダウンロードする
ms.openlocfilehash: b5456acc6661fdc7a9682bf2b0ff70a2e5e38a3e
ms.sourcegitcommit: 9f5a17e9978197ab47b460c53f7fe2cec180d4a2
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/10/2018
ms.locfileid: "19492733"
---
# <a name="download-the-contents-of-a-driveitem"></a><span data-ttu-id="738fb-102">DriveItem のコンテンツをダウンロードする</span><span class="sxs-lookup"><span data-stu-id="738fb-102">Download the contents of a DriveItem</span></span>

<span data-ttu-id="738fb-103">DriveItem のプライマリ ストリーム (ファイル) のコンテンツをダウンロードします。</span><span class="sxs-lookup"><span data-stu-id="738fb-103">Download the contents of the primary stream (file) of a DriveItem.</span></span> <span data-ttu-id="738fb-104">**file** プロパティを持つ driveItem のみがダウンロード可能です。</span><span class="sxs-lookup"><span data-stu-id="738fb-104">Only driveItems with the **file** property can be downloaded.</span></span>

## <a name="permissions"></a><span data-ttu-id="738fb-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="738fb-105">Permissions</span></span>

<span data-ttu-id="738fb-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="738fb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="738fb-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="738fb-108">Permission type</span></span>      | <span data-ttu-id="738fb-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="738fb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="738fb-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="738fb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="738fb-111">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="738fb-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="738fb-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="738fb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="738fb-113">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="738fb-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="738fb-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="738fb-114">Application</span></span> | <span data-ttu-id="738fb-115">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="738fb-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="738fb-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="738fb-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/content
GET /groups/{group-id}/drive/items/{item-id}/content
GET /me/drive/root:/{item-path}:/content
GET /me/drive/items/{item-id}/content
GET /sites/{siteId}/drive/items/{item-id}/content
GET /users/{userId}/drive/items/{item-id}/content
```

## <a name="optional-request-headers"></a><span data-ttu-id="738fb-117">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="738fb-117">Optional request headers</span></span>

| <span data-ttu-id="738fb-118">名前</span><span class="sxs-lookup"><span data-stu-id="738fb-118">Name</span></span>          | <span data-ttu-id="738fb-119">値</span><span class="sxs-lookup"><span data-stu-id="738fb-119">Value</span></span>  | <span data-ttu-id="738fb-120">説明</span><span class="sxs-lookup"><span data-stu-id="738fb-120">Description</span></span>                                                                                                                                              |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="738fb-121">if-none-match</span><span class="sxs-lookup"><span data-stu-id="738fb-121">if-none-match</span></span> | <span data-ttu-id="738fb-122">String</span><span class="sxs-lookup"><span data-stu-id="738fb-122">String</span></span> | <span data-ttu-id="738fb-123">この要求ヘッダーが含まれている場合、指定された eTag (または cTag) がファイルの現在のタグに一致すると、`HTTP 304 Not Modified` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="738fb-123">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="example"></a><span data-ttu-id="738fb-124">例</span><span class="sxs-lookup"><span data-stu-id="738fb-124">Example</span></span>

<span data-ttu-id="738fb-125">完全なファイルをダウンロードする例を示します。</span><span class="sxs-lookup"><span data-stu-id="738fb-125">Here is an example to download a complete file.</span></span>


<!-- { "blockType": "request", "name": "download-item-content", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/content
```

### <a name="response"></a><span data-ttu-id="738fb-126">応答</span><span class="sxs-lookup"><span data-stu-id="738fb-126">Response</span></span>

<span data-ttu-id="738fb-p103">ファイルの事前認証されたダウンロード URL にリダイレクトする、`302 Found` 応答を返します。これは、DriveItem の `@microsoft.graph.downloadUrl` プロパティを通じて使用可能な URL と同じものです。</span><span class="sxs-lookup"><span data-stu-id="738fb-p103">Returns a `302 Found` response redirecting to a pre-authenticated download URL for the file. This is the same URL available through the `@microsoft.graph.downloadUrl` property on the DriveItem.</span></span>

<span data-ttu-id="738fb-p104">ファイルのコンテンツをダウンロードするには、アプリケーションで応答の `Location` ヘッダーに従う必要があります。多くの HTTP クライアント ライブラリは、自動的に 302 リダイレクションに従い、即座にファイルのダウンロードを開始します。</span><span class="sxs-lookup"><span data-stu-id="738fb-p104">To download the contents of the file your application will need to follow the `Location` header in the response. Many HTTP client libraries will automatically follow the 302 redirection and start downloading the file immedately.</span></span>

<span data-ttu-id="738fb-131">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、ダウンロードのために `Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="738fb-131">Pre-authenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to download.</span></span>

<!-- { "blockType": "response", "@odata.type": "stream" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

## <a name="partial-range-downloads"></a><span data-ttu-id="738fb-132">部分的な範囲のダウンロード</span><span class="sxs-lookup"><span data-stu-id="738fb-132">Partial range downloads</span></span>

<span data-ttu-id="738fb-p105">ファイルから部分的なバイトの範囲をダウンロードするには、[RFC 2616](https://www.ietf.org/rfc/rfc2616.txt) で規定されているように、アプリで `Range` ヘッダーを使用します。`Range` ヘッダーは実際の `@microsoft.graph.downloadUrl` URL に追加する必要があり、`/content` の要求には追加しない点に注意してください。</span><span class="sxs-lookup"><span data-stu-id="738fb-p105">To download a partial range of bytes from the file, your app can use the `Range` header as specified in [RFC 2616](https://www.ietf.org/rfc/rfc2616.txt). Note that you must append the `Range` header to the actual `@microsoft.graph.downloadUrl` URL and not to the request for `/content`.</span></span>

<!-- { "blockType": "request", "name": "download-item-partial", "scopes": "files.read" } -->

```http
GET https://b0mpua-by3301.files.1drv.com/y23vmag
Range: bytes=0-1023
```

<span data-ttu-id="738fb-p106">これにより、ファイルからのバイトの要求範囲を含む `HTTP 206 Partial Content` 応答が返されます。範囲が生成できない場合、Range ヘッダーは無視され、ファイルの完全なコンテンツを含む `HTTP 200` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="738fb-p106">This will return an `HTTP 206 Partial Content` response with the request range of bytes from the file. If the range cannot be generated the Range header may be ignored and an `HTTP 200` response would be returned with the full contents of the file.</span></span>

<!-- { "blockType": "response", "name": "download-item-partial", "@odata.type": "stream" } -->

```http
HTTP/1.1 206 Partial Content
Content-Range: bytes 0-1023/2048

<first 1024 bytes of file>
```

### <a name="error-responses"></a><span data-ttu-id="738fb-137">エラー応答</span><span class="sxs-lookup"><span data-stu-id="738fb-137">Error responses</span></span>

<span data-ttu-id="738fb-138">エラーがどのように返されるかについては、「[エラー応答][error-response]」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="738fb-138">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: ../../../concepts/errors.md

<!-- {
  "type": "#page.annotation",
  "description": "Download the contents of a DriveItem.",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Items/Download"
} -->
