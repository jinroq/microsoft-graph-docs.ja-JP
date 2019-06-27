---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 以前のバージョンをダウンロードする
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 55bc0d029cd64e420b956c41f10f3786a62cce88
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35259991"
---
# <a name="download-contents-of-a-driveitemversion-resource-preview"></a><span data-ttu-id="1979c-102">DriveItemVersion リソースのコンテンツをダウンロードする (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="1979c-102">Download contents of a DriveItemVersion resource (preview)</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1979c-103">特定のバージョンの[ドライブ項目](../resources/driveitem.md)の内容を取得します。</span><span class="sxs-lookup"><span data-stu-id="1979c-103">Retrieve the contents of a specific version of a [driveItem](../resources/driveitem.md).</span></span> 

><span data-ttu-id="1979c-104">**注:** 現在のバージョンのコンテンツを取得することはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1979c-104">**Note:** Getting the content of the current version is not supported.</span></span> <span data-ttu-id="1979c-105">代わりに、[ドライブアイテムコンテンツエンドポイント](driveitem-get-content.md)を使用してください。</span><span class="sxs-lookup"><span data-stu-id="1979c-105">Instead, use the [driveItem content endpoint](driveitem-get-content.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1979c-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1979c-106">Permissions</span></span>

<span data-ttu-id="1979c-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1979c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1979c-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1979c-109">Permission type</span></span>      | <span data-ttu-id="1979c-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1979c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1979c-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1979c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1979c-112">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1979c-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="1979c-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1979c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1979c-114">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1979c-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="1979c-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1979c-115">Application</span></span> | <span data-ttu-id="1979c-116">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1979c-116">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="1979c-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1979c-117">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /drives/{drive-id}/items/{item-id}/versions/{version-id}/content
GET /groups/{group-id}/drive/{item-id}/versions/{version-id}/content
GET /me/drive/items/{item-id}/versions/{version-id}/content
GET /sites/{site-id}/drive/items/{item-id}/versions/{version-id}/content
GET /users/{user-id}/drive/items/{item-id}/versions/{version-id}/content
```

## <a name="response"></a><span data-ttu-id="1979c-118">応答</span><span class="sxs-lookup"><span data-stu-id="1979c-118">Response</span></span>

<span data-ttu-id="1979c-119">ファイルのバイトの事前認証されたダウンロード URL にリダイレクトする、`302 Found` 応答を返します。</span><span class="sxs-lookup"><span data-stu-id="1979c-119">Returns a `302 Found` response redirecting to a pre-authenticated download URL for the bytes of the file.</span></span>

<span data-ttu-id="1979c-p103">ファイルのコンテンツをダウンロードするには、アプリケーションで応答の `Location` ヘッダーに従う必要があります。多くの HTTP クライアント ライブラリは、自動的に 302 リダイレクションに従い、即座にファイルのダウンロードを開始します。</span><span class="sxs-lookup"><span data-stu-id="1979c-p103">To download the contents of the file your application will need to follow the `Location` header in the response. Many HTTP client libraries will automatically follow the 302 redirection and start downloading the file immedately.</span></span>

<span data-ttu-id="1979c-122">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、ダウンロードのために `Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="1979c-122">Pre-authenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to download.</span></span>

## <a name="example"></a><span data-ttu-id="1979c-123">例</span><span class="sxs-lookup"><span data-stu-id="1979c-123">Example</span></span>

<span data-ttu-id="1979c-124">この例では、現在のユーザーのドライブ内のファイルのバージョンを取得します。</span><span class="sxs-lookup"><span data-stu-id="1979c-124">This example retrieves a version of a file in the current user's drive.</span></span>

### <a name="request"></a><span data-ttu-id="1979c-125">要求</span><span class="sxs-lookup"><span data-stu-id="1979c-125">Request</span></span>

<!-- { "blockType": "request", "name": "get-version-contents", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive/items/{item-id}/versions/{version-id}/content
```

### <a name="response"></a><span data-ttu-id="1979c-126">応答</span><span class="sxs-lookup"><span data-stu-id="1979c-126">Response</span></span>

<span data-ttu-id="1979c-127">そのバージョンのコンテンツをダウンロードできる場所へのリダイレクトを返します。</span><span class="sxs-lookup"><span data-stu-id="1979c-127">This returns a redirect to where the contents of the version can be downloaded.</span></span>

<!-- { "blockType": "response", "isEmpty": true  } -->

```http
HTTP/1.1 302 Redirect
Location: https://onedrive.com/34FF49D6...
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="1979c-128">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="1979c-128">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="1979c-129">C#</span><span class="sxs-lookup"><span data-stu-id="1979c-129">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-version-contents-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1979c-130">Javascript</span><span class="sxs-lookup"><span data-stu-id="1979c-130">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-version-contents-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="1979c-131">目的-C</span><span class="sxs-lookup"><span data-stu-id="1979c-131">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get-version-contents-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]


## <a name="remarks"></a><span data-ttu-id="1979c-132">備考</span><span class="sxs-lookup"><span data-stu-id="1979c-132">Remarks</span></span>

<span data-ttu-id="1979c-133">OneDrive は、ファイルの旧バージョンの完全なメタデータを保持しません。</span><span class="sxs-lookup"><span data-stu-id="1979c-133">OneDrive does not preserve the complete metadata for previous versions of a file.</span></span>

<span data-ttu-id="1979c-134">アプリでファイルの利用可能なバージョンの一覧を取得すると、特定のバージョンに関する情報を提供する、 [Drive itemversion](../resources/driveitemversion.md)リソースが返されます。</span><span class="sxs-lookup"><span data-stu-id="1979c-134">When your app retrieves the list of available versions for a file, a [driveItemVersion](../resources/driveitemversion.md) resource is returned that provides the available information about the specific version.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history",
  "suppressions": [
    "Error: /api-reference/beta/api/driveitemversion-get-contents.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/driveitemversion-get-contents.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/driveitemversion-get-contents.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
