---
title: ドライブ Itemversion リソースを取得する
description: DriveItem の特定のバージョンのメタデータを取得します。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: ed11ef061fad293885df8f5269898ddc5df80f10
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35886472"
---
# <a name="get-a-driveitemversion-resource"></a><span data-ttu-id="3faee-103">ドライブ Itemversion リソースを取得する</span><span class="sxs-lookup"><span data-stu-id="3faee-103">Get a DriveItemVersion resource</span></span>

<span data-ttu-id="3faee-104">[DriveItem](../resources/driveitem.md) の特定のバージョンのメタデータを取得します。</span><span class="sxs-lookup"><span data-stu-id="3faee-104">Retrieve the metadata for a specific version of a [DriveItem](../resources/driveitem.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3faee-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3faee-105">Permissions</span></span>

<span data-ttu-id="3faee-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3faee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3faee-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3faee-108">Permission type</span></span>      | <span data-ttu-id="3faee-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3faee-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3faee-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3faee-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3faee-111">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3faee-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="3faee-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3faee-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3faee-113">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3faee-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="3faee-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3faee-114">Application</span></span> | <span data-ttu-id="3faee-115">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3faee-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="3faee-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3faee-116">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /drives/{drive-id}/items/{item-id}/versions/{version-id}
GET /groups/{group-id}/drive/{item-id}/versions/{version-id}
GET /me/drive/items/{item-id}/versions/{version-id}
GET /sites/{site-id}/drive/items/{item-id}/versions/{version-id}
GET /users/{user-id}/drive/items/{item-id}/versions/{version-id}
```

## <a name="response"></a><span data-ttu-id="3faee-117">応答</span><span class="sxs-lookup"><span data-stu-id="3faee-117">Response</span></span>

<span data-ttu-id="3faee-118">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [DriveItemVersion](../resources/driveitemversion.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="3faee-118">If successful, this method returns a `200 OK` response code and a [DriveItemVersion](../resources/driveitemversion.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="3faee-119">例</span><span class="sxs-lookup"><span data-stu-id="3faee-119">Example</span></span>

<span data-ttu-id="3faee-120">この例では、現在のユーザーのドライブ内のファイルのバージョンを取得します。</span><span class="sxs-lookup"><span data-stu-id="3faee-120">This example retrieves a version of a file in the current user's drive.</span></span>

### <a name="http-request"></a><span data-ttu-id="3faee-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3faee-121">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="3faee-122">プロトコル</span><span class="sxs-lookup"><span data-stu-id="3faee-122">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-single-version", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive/items/{item-id}/versions/{version-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3faee-123">C#</span><span class="sxs-lookup"><span data-stu-id="3faee-123">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-single-version-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3faee-124">Javascript</span><span class="sxs-lookup"><span data-stu-id="3faee-124">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-single-version-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3faee-125">目的-C</span><span class="sxs-lookup"><span data-stu-id="3faee-125">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-single-version-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="3faee-126">Java</span><span class="sxs-lookup"><span data-stu-id="3faee-126">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-single-version-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3faee-127">応答</span><span class="sxs-lookup"><span data-stu-id="3faee-127">Response</span></span>

<span data-ttu-id="3faee-128">バージョンのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="3faee-128">This returns a collection of versions:</span></span>

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

## <a name="remarks"></a><span data-ttu-id="3faee-129">備考</span><span class="sxs-lookup"><span data-stu-id="3faee-129">Remarks</span></span>

<span data-ttu-id="3faee-130">OneDrive は、ファイルの旧バージョンの完全なメタデータを保持しません。</span><span class="sxs-lookup"><span data-stu-id="3faee-130">OneDrive does not preserve the complete metadata for previous versions of a file.</span></span>

<span data-ttu-id="3faee-131">アプリがファイルの利用可能なバージョンのリストを取得すると、[DriveItemVersion](../resources/driveitemversion.md) リソースが返され、特定のバージョンに関する利用可能な情報が提供されます。</span><span class="sxs-lookup"><span data-stu-id="3faee-131">When your app retrieves the list of available versions for a file, a [DriveItemVersion](../resources/driveitemversion.md) resource is returned that provides the available information about the specific version.</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history",
  "suppressions": [
  ]
} -->
