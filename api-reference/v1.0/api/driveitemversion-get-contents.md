---
title: '[ファイル] [ドライブ] [バージョン] リソースのコンテンツをダウンロードする'
description: DriveItem の特定のバージョンのコンテンツを取得します。
localization_priority: Normal
ms.prod: sharepoint
author: ''
doc_type: apiPageType
ms.openlocfilehash: a992390ac2a087d1df905a5eff606731b8944316
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36370537"
---
# <a name="download-contents-of-a-driveitemversion-resource"></a><span data-ttu-id="1f63c-103">[ファイル] [ドライブ] [バージョン] リソースのコンテンツをダウンロードする</span><span class="sxs-lookup"><span data-stu-id="1f63c-103">Download contents of a DriveItemVersion resource</span></span>

<span data-ttu-id="1f63c-104">[DriveItem](../resources/driveitem.md) の特定のバージョンのコンテンツを取得します。</span><span class="sxs-lookup"><span data-stu-id="1f63c-104">Retrieve the contents of a specific version of a [DriveItem](../resources/driveitem.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1f63c-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1f63c-105">Permissions</span></span>

<span data-ttu-id="1f63c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1f63c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f63c-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1f63c-108">Permission type</span></span>      | <span data-ttu-id="1f63c-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1f63c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1f63c-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1f63c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1f63c-111">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f63c-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="1f63c-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1f63c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1f63c-113">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f63c-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="1f63c-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1f63c-114">Application</span></span> | <span data-ttu-id="1f63c-115">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f63c-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="1f63c-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1f63c-116">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /drives/{drive-id}/items/{item-id}/versions/{version-id}/content
GET /groups/{group-id}/drive/{item-id}/versions/{version-id}/content
GET /me/drive/items/{item-id}/versions/{version-id}/content
GET /sites/{site-id}/drive/items/{item-id}/versions/{version-id}/content
GET /users/{user-id}/drive/items/{item-id}/versions/{version-id}/content
```

## <a name="response"></a><span data-ttu-id="1f63c-117">応答</span><span class="sxs-lookup"><span data-stu-id="1f63c-117">Response</span></span>

<span data-ttu-id="1f63c-118">ファイルのバイトの事前認証されたダウンロード URL にリダイレクトする、`302 Found` 応答を返します。</span><span class="sxs-lookup"><span data-stu-id="1f63c-118">Returns a `302 Found` response redirecting to a pre-authenticated download URL for the bytes of the file.</span></span>

<span data-ttu-id="1f63c-p102">ファイルのコンテンツをダウンロードするには、アプリケーションで応答の `Location` ヘッダーに従う必要があります。多くの HTTP クライアント ライブラリは、自動的に 302 リダイレクションに従い、即座にファイルのダウンロードを開始します。</span><span class="sxs-lookup"><span data-stu-id="1f63c-p102">To download the contents of the file your application will need to follow the `Location` header in the response. Many HTTP client libraries will automatically follow the 302 redirection and start downloading the file immedately.</span></span>

<span data-ttu-id="1f63c-121">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、ダウンロードのために `Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="1f63c-121">Pre-authenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to download.</span></span>

## <a name="example"></a><span data-ttu-id="1f63c-122">例</span><span class="sxs-lookup"><span data-stu-id="1f63c-122">Example</span></span>

<span data-ttu-id="1f63c-123">この例では、現在のユーザーのドライブ内のファイルのバージョンを取得します。</span><span class="sxs-lookup"><span data-stu-id="1f63c-123">This example retrieves a version of a file in the current user's drive.</span></span>

### <a name="http-request"></a><span data-ttu-id="1f63c-124">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1f63c-124">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="1f63c-125">プロトコル</span><span class="sxs-lookup"><span data-stu-id="1f63c-125">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-version-contents", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive/items/{item-id}/versions/{version-id}/content
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1f63c-126">C#</span><span class="sxs-lookup"><span data-stu-id="1f63c-126">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-version-contents-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1f63c-127">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1f63c-127">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-version-contents-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1f63c-128">目的-C</span><span class="sxs-lookup"><span data-stu-id="1f63c-128">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-version-contents-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="1f63c-129">Java</span><span class="sxs-lookup"><span data-stu-id="1f63c-129">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-version-contents-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1f63c-130">応答</span><span class="sxs-lookup"><span data-stu-id="1f63c-130">Response</span></span>

<span data-ttu-id="1f63c-131">そのバージョンのコンテンツをダウンロードできる場所へのリダイレクトを返します。</span><span class="sxs-lookup"><span data-stu-id="1f63c-131">This returns a redirect to where the contents of the version can be downloaded.</span></span>

<!-- { "blockType": "response", "isEmpty": true  } -->

```http
HTTP/1.1 302 Found
Location: https://onedrive.com/34FF49D6...
```


## <a name="remarks"></a><span data-ttu-id="1f63c-132">備考</span><span class="sxs-lookup"><span data-stu-id="1f63c-132">Remarks</span></span>

<span data-ttu-id="1f63c-133">OneDrive は、ファイルの旧バージョンの完全なメタデータを保持しません。</span><span class="sxs-lookup"><span data-stu-id="1f63c-133">OneDrive does not preserve the complete metadata for previous versions of a file.</span></span>

<span data-ttu-id="1f63c-134">アプリがファイルの利用可能なバージョンのリストを取得すると、[DriveItemVersion](../resources/driveitemversion.md) リソースが返され、特定のバージョンに関する利用可能な情報が提供されます。</span><span class="sxs-lookup"><span data-stu-id="1f63c-134">When your app retrieves the list of available versions for a file, a [DriveItemVersion](../resources/driveitemversion.md) resource is returned that provides the available information about the specific version.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history",
  "suppressions": [
  ]
} -->
