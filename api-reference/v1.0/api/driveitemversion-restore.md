---
title: DriveItem の旧バージョンを復元する
description: DriveItem の旧バージョンを現在のバージョンに復元します。 旧バージョンのコンテンツを持つ新しいバージョンを作成します。しかし、ファイルの既存のバージョンはすべて保持されます。
localization_priority: Normal
ms.prod: sharepoint
author: ''
doc_type: apiPageType
ms.openlocfilehash: f6a0208526fcd48f5dffa78a073da2aa8191d851
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006893"
---
# <a name="restore-a-previous-version-of-a-driveitem"></a><span data-ttu-id="dbd7e-104">DriveItem の旧バージョンを復元する</span><span class="sxs-lookup"><span data-stu-id="dbd7e-104">Restore a previous version of a DriveItem</span></span>

<span data-ttu-id="dbd7e-105">DriveItem の旧バージョンを現在のバージョンに復元します。</span><span class="sxs-lookup"><span data-stu-id="dbd7e-105">Restore a previous version of a DriveItem to be the current version.</span></span> <span data-ttu-id="dbd7e-106">旧バージョンのコンテンツを持つ新しいバージョンを作成します。しかし、ファイルの既存のバージョンはすべて保持されます。</span><span class="sxs-lookup"><span data-stu-id="dbd7e-106">This will create a new version with the contents of the previous version, but preserves all existing versions of the file.</span></span>

## <a name="permissions"></a><span data-ttu-id="dbd7e-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="dbd7e-107">Permissions</span></span>

<span data-ttu-id="dbd7e-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dbd7e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dbd7e-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="dbd7e-110">Permission type</span></span>      | <span data-ttu-id="dbd7e-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="dbd7e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dbd7e-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="dbd7e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="dbd7e-113">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dbd7e-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="dbd7e-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="dbd7e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dbd7e-115">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dbd7e-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="dbd7e-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="dbd7e-116">Application</span></span> | <span data-ttu-id="dbd7e-117">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dbd7e-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dbd7e-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="dbd7e-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/versions/{version-id}/restoreVersion
POST /groups/{groupId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /me/drive/items/{item-id}/versions/{version-id}/restoreVersion
POST /sites/{siteId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /users/{userId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
```

### <a name="request-body"></a><span data-ttu-id="dbd7e-119">要求本文</span><span class="sxs-lookup"><span data-stu-id="dbd7e-119">Request body</span></span>

<span data-ttu-id="dbd7e-120">要求の本文は必要ありません。</span><span class="sxs-lookup"><span data-stu-id="dbd7e-120">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="dbd7e-121">例</span><span class="sxs-lookup"><span data-stu-id="dbd7e-121">Example</span></span>

<span data-ttu-id="dbd7e-122">この例では、`{item-id}` と `{version-id}` で指定されたファイルのバージョンを復元します。</span><span class="sxs-lookup"><span data-stu-id="dbd7e-122">This example restores a version of a file identified by `{item-id}` and `{version-id}`.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="dbd7e-123">プロトコル</span><span class="sxs-lookup"><span data-stu-id="dbd7e-123">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "restore-item-version", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/versions/{version-id}/restoreVersion
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="dbd7e-124">C#</span><span class="sxs-lookup"><span data-stu-id="dbd7e-124">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/restore-item-version-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dbd7e-125">Javascript</span><span class="sxs-lookup"><span data-stu-id="dbd7e-125">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/restore-item-version-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="dbd7e-126">目的-C</span><span class="sxs-lookup"><span data-stu-id="dbd7e-126">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/restore-item-version-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="dbd7e-127">Java</span><span class="sxs-lookup"><span data-stu-id="dbd7e-127">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/restore-item-version-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="dbd7e-128">応答</span><span class="sxs-lookup"><span data-stu-id="dbd7e-128">Response</span></span>

<span data-ttu-id="dbd7e-129">成功すると、API 呼び出しは `204 No Content` を返します。</span><span class="sxs-lookup"><span data-stu-id="dbd7e-129">If successful, the API call returns a `204 No Content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy",
  "suppressions": [
  ]
} -->
