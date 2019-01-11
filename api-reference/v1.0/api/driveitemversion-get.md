---
title: DriveItemVersion リソースを取得します。
description: DriveItem の特定のバージョンのメタデータを取得します。
localization_priority: Normal
ms.openlocfilehash: d16e6bf6a9fa797f952109a773cfd4227696e032
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27868342"
---
# <a name="get-a-driveitemversion-resource"></a><span data-ttu-id="abac1-103">DriveItemVersion リソースを取得します。</span><span class="sxs-lookup"><span data-stu-id="abac1-103">Get a DriveItemVersion resource</span></span>

<span data-ttu-id="abac1-104">[DriveItem](../resources/driveitem.md) の特定のバージョンのメタデータを取得します。</span><span class="sxs-lookup"><span data-stu-id="abac1-104">Retrieve the metadata for a specific version of a [DriveItem](../resources/driveitem.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="abac1-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="abac1-105">Permissions</span></span>

<span data-ttu-id="abac1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="abac1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="abac1-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="abac1-108">Permission type</span></span>      | <span data-ttu-id="abac1-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="abac1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="abac1-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="abac1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="abac1-111">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="abac1-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="abac1-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="abac1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="abac1-113">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="abac1-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="abac1-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="abac1-114">Application</span></span> | <span data-ttu-id="abac1-115">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="abac1-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="abac1-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="abac1-116">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /drives/{drive-id}/items/{item-id}/versions/{version-id}
GET /groups/{group-id}/drive/{item-id}/versions/{version-id}
GET /me/drive/items/{item-id}/versions/{version-id}
GET /sites/{site-id}/drive/items/{item-id}/versions/{version-id}
GET /users/{user-id}/drive/items/{item-id}/versions/{version-id}
```

## <a name="response"></a><span data-ttu-id="abac1-117">応答</span><span class="sxs-lookup"><span data-stu-id="abac1-117">Response</span></span>

<span data-ttu-id="abac1-118">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [DriveItemVersion](../resources/driveitemversion.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="abac1-118">If successful, this method returns a `200 OK` response code and a [DriveItemVersion](../resources/driveitemversion.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="abac1-119">例</span><span class="sxs-lookup"><span data-stu-id="abac1-119">Example</span></span>

<span data-ttu-id="abac1-120">この例では、現在のユーザーのドライブ内のファイルのバージョンを取得します。</span><span class="sxs-lookup"><span data-stu-id="abac1-120">This example retrieves a version of a file in the current user's drive.</span></span>

### <a name="http-request"></a><span data-ttu-id="abac1-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="abac1-121">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-single-version", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive/items/{item-id}/versions/{version-id}
```

### <a name="response"></a><span data-ttu-id="abac1-122">応答</span><span class="sxs-lookup"><span data-stu-id="abac1-122">Response</span></span>

<span data-ttu-id="abac1-123">バージョンのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="abac1-123">This returns a collection of versions:</span></span>

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

## <a name="remarks"></a><span data-ttu-id="abac1-124">備考</span><span class="sxs-lookup"><span data-stu-id="abac1-124">Remarks</span></span>

<span data-ttu-id="abac1-125">OneDrive は、ファイルの旧バージョンの完全なメタデータを保持しません。</span><span class="sxs-lookup"><span data-stu-id="abac1-125">OneDrive does not preserve the complete metadata for previous versions of a file.</span></span>

<span data-ttu-id="abac1-126">アプリがファイルの利用可能なバージョンのリストを取得すると、[DriveItemVersion](../resources/driveitemversion.md) リソースが返され、特定のバージョンに関する利用可能な情報が提供されます。</span><span class="sxs-lookup"><span data-stu-id="abac1-126">When your app retrieves the list of available versions for a file, a [DriveItemVersion](../resources/driveitemversion.md) resource is returned that provides the available information about the specific version.</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history"
} -->
