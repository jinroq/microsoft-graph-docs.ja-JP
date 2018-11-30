---
title: DriveItemVersion リソースを取得する (プレビュー)
description: DriveItem の特定のバージョンのメタデータを取得します。
ms.openlocfilehash: c78a81d1a5428bbb969f8761b238655ab7919e5a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068280"
---
# <a name="get-a-driveitemversion-resource-preview"></a><span data-ttu-id="1a011-103">DriveItemVersion リソースを取得する (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="1a011-103">Get a DriveItemVersion resource (preview)</span></span>

> <span data-ttu-id="1a011-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1a011-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1a011-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1a011-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1a011-106">[DriveItem](../resources/driveitem.md) の特定のバージョンのメタデータを取得します。</span><span class="sxs-lookup"><span data-stu-id="1a011-106">Retrieve the metadata for a specific version of a [DriveItem](../resources/driveitem.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1a011-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1a011-107">Permissions</span></span>

<span data-ttu-id="1a011-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1a011-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a011-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1a011-110">Permission type</span></span>      | <span data-ttu-id="1a011-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1a011-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1a011-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1a011-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1a011-113">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a011-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="1a011-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1a011-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1a011-115">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a011-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="1a011-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1a011-116">Application</span></span> | <span data-ttu-id="1a011-117">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a011-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="1a011-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1a011-118">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /drives/{drive-id}/items/{item-id}/versions/{version-id}
GET /groups/{group-id}/drive/{item-id}/versions/{version-id}
GET /me/drive/items/{item-id}/versions/{version-id}
GET /sites/{site-id}/drive/items/{item-id}/versions/{version-id}
GET /users/{user-id}/drive/items/{item-id}/versions/{version-id}
```

## <a name="response"></a><span data-ttu-id="1a011-119">応答</span><span class="sxs-lookup"><span data-stu-id="1a011-119">Response</span></span>

<span data-ttu-id="1a011-120">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [DriveItemVersion](../resources/driveitemversion.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="1a011-120">If successful, this method returns a `200 OK` response code and a [DriveItemVersion](../resources/driveitemversion.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="1a011-121">例</span><span class="sxs-lookup"><span data-stu-id="1a011-121">Example</span></span>

<span data-ttu-id="1a011-122">この例では、現在のユーザーのドライブ内のファイルのバージョンを取得します。</span><span class="sxs-lookup"><span data-stu-id="1a011-122">This example retrieves a version of a file in the current user's drive.</span></span>

### <a name="http-request"></a><span data-ttu-id="1a011-123">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1a011-123">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-single-version", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/versions/{version-id}
```

### <a name="response"></a><span data-ttu-id="1a011-124">応答</span><span class="sxs-lookup"><span data-stu-id="1a011-124">Response</span></span>

<span data-ttu-id="1a011-125">バージョンのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="1a011-125">This returns a collection of versions:</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItemVersion", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "id": "D4990684-58CE-4FAB-9B87-D6C49E74F298",
    "lastModifiedBy": {
    "user": {
        "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
        "displayName": "Ryan Gregg"
    }
    },
    "lastModifiedDateTime": "2017-09-14T12:34:53.912Z",
    "size": 123
}
```

## <a name="remarks"></a><span data-ttu-id="1a011-126">備考</span><span class="sxs-lookup"><span data-stu-id="1a011-126">Remarks</span></span>

<span data-ttu-id="1a011-127">OneDrive は、ファイルの旧バージョンの完全なメタデータを保持しません。</span><span class="sxs-lookup"><span data-stu-id="1a011-127">OneDrive does not preserve the complete metadata for previous versions of a file.</span></span>

<span data-ttu-id="1a011-128">アプリがファイルの利用可能なバージョンのリストを取得すると、[DriveItemVersion](../resources/driveitemversion.md) リソースが返され、特定のバージョンに関する利用可能な情報が提供されます。</span><span class="sxs-lookup"><span data-stu-id="1a011-128">When your app retrieves the list of available versions for a file, a [DriveItemVersion](../resources/driveitemversion.md) resource is returned that provides the available information about the specific version.</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history"
} -->
