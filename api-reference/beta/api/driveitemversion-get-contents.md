---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: 以前のバージョンをダウンロードします。
ms.openlocfilehash: 1d55a457060197cfd9a24a39506003518918d398
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067349"
---
# <a name="download-contents-of-a-driveitemversion-resource-preview"></a><span data-ttu-id="ad75e-102">DriveItemVersion リソースのコンテンツをダウンロードする (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="ad75e-102">Download contents of a DriveItemVersion resource (preview)</span></span>

> <span data-ttu-id="ad75e-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ad75e-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ad75e-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ad75e-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ad75e-105">の[driveItem](../resources/driveitem.md)の特定のバージョンの内容を取得します。</span><span class="sxs-lookup"><span data-stu-id="ad75e-105">Retrieve the contents of a specific version of a [driveItem](../resources/driveitem.md).</span></span> 

><span data-ttu-id="ad75e-106">**注:** 現在のバージョンのコンテンツを取得することはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ad75e-106">**Note:** Getting the content of the current version is not supported.</span></span> <span data-ttu-id="ad75e-107">[DriveItem コンテンツのエンドポイント](driveitem-get-content.md)を使用できます。</span><span class="sxs-lookup"><span data-stu-id="ad75e-107">Instead, use the [driveItem content endpoint](driveitem-get-content.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ad75e-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ad75e-108">Permissions</span></span>

<span data-ttu-id="ad75e-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ad75e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ad75e-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ad75e-111">Permission type</span></span>      | <span data-ttu-id="ad75e-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ad75e-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ad75e-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ad75e-113">Delegated (work or school account)</span></span> | <span data-ttu-id="ad75e-114">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad75e-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="ad75e-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ad75e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ad75e-116">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad75e-116">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="ad75e-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ad75e-117">Application</span></span> | <span data-ttu-id="ad75e-118">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad75e-118">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="ad75e-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ad75e-119">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /drives/{drive-id}/items/{item-id}/versions/{version-id}/content
GET /groups/{group-id}/drive/{item-id}/versions/{version-id}/content
GET /me/drive/items/{item-id}/versions/{version-id}/content
GET /sites/{site-id}/drive/items/{item-id}/versions/{version-id}/content
GET /users/{user-id}/drive/items/{item-id}/versions/{version-id}/content
```

## <a name="response"></a><span data-ttu-id="ad75e-120">応答</span><span class="sxs-lookup"><span data-stu-id="ad75e-120">Response</span></span>

<span data-ttu-id="ad75e-121">ファイルのバイトの事前認証されたダウンロード URL にリダイレクトする、`302 Found` 応答を返します。</span><span class="sxs-lookup"><span data-stu-id="ad75e-121">Returns a `302 Found` response redirecting to a pre-authenticated download URL for the bytes of the file.</span></span>

<span data-ttu-id="ad75e-p104">ファイルのコンテンツをダウンロードするには、アプリケーションで応答の `Location` ヘッダーに従う必要があります。多くの HTTP クライアント ライブラリは、自動的に 302 リダイレクションに従い、即座にファイルのダウンロードを開始します。</span><span class="sxs-lookup"><span data-stu-id="ad75e-p104">To download the contents of the file your application will need to follow the `Location` header in the response. Many HTTP client libraries will automatically follow the 302 redirection and start downloading the file immedately.</span></span>

<span data-ttu-id="ad75e-124">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、ダウンロードのために `Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="ad75e-124">Pre-authenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to download.</span></span>

## <a name="example"></a><span data-ttu-id="ad75e-125">例</span><span class="sxs-lookup"><span data-stu-id="ad75e-125">Example</span></span>

<span data-ttu-id="ad75e-126">この例では、現在のユーザーのドライブ内のファイルのバージョンを取得します。</span><span class="sxs-lookup"><span data-stu-id="ad75e-126">This example retrieves a version of a file in the current user's drive.</span></span>

### <a name="request"></a><span data-ttu-id="ad75e-127">要求</span><span class="sxs-lookup"><span data-stu-id="ad75e-127">Request</span></span>

<!-- { "blockType": "request", "name": "get-version-contents", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive/items/{item-id}/versions/{version-id}/content
```

### <a name="response"></a><span data-ttu-id="ad75e-128">応答</span><span class="sxs-lookup"><span data-stu-id="ad75e-128">Response</span></span>

<span data-ttu-id="ad75e-129">そのバージョンのコンテンツをダウンロードできる場所へのリダイレクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ad75e-129">This returns a redirect to where the contents of the version can be downloaded.</span></span>

<!-- { "blockType": "response", "isEmpty": true  } -->

```http
HTTP/1.1 302 Redirect
Location: https://onedrive.com/34FF49D6...
```


## <a name="remarks"></a><span data-ttu-id="ad75e-130">備考</span><span class="sxs-lookup"><span data-stu-id="ad75e-130">Remarks</span></span>

<span data-ttu-id="ad75e-131">OneDrive は、ファイルの旧バージョンの完全なメタデータを保持しません。</span><span class="sxs-lookup"><span data-stu-id="ad75e-131">OneDrive does not preserve the complete metadata for previous versions of a file.</span></span>

<span data-ttu-id="ad75e-132">アプリは、ファイルの利用可能なバージョンの一覧を取得、特定のバージョンに関する情報を提供する[driveItemVersion](../resources/driveitemversion.md)リソースが返されます。</span><span class="sxs-lookup"><span data-stu-id="ad75e-132">When your app retrieves the list of available versions for a file, a [driveItemVersion](../resources/driveitemversion.md) resource is returned that provides the available information about the specific version.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history"
} -->
