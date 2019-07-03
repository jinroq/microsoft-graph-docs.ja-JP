---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 前のバージョンを復元する
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 43d46caf83a028b751a0c21c3bffe69ee0983c11
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35436187"
---
# <a name="restore-a-previous-version-of-a-driveitem"></a><span data-ttu-id="4dfeb-102">DriveItem の旧バージョンを復元する</span><span class="sxs-lookup"><span data-stu-id="4dfeb-102">Restore a previous version of a DriveItem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4dfeb-103">DriveItem の旧バージョンを現在のバージョンに復元します。</span><span class="sxs-lookup"><span data-stu-id="4dfeb-103">Restore a previous version of a DriveItem to be the current version.</span></span> <span data-ttu-id="4dfeb-104">旧バージョンのコンテンツを持つ新しいバージョンを作成します。しかし、ファイルの既存のバージョンはすべて保持されます。</span><span class="sxs-lookup"><span data-stu-id="4dfeb-104">This will create a new version with the contents of the previous version, but preserves all existing versions of the file.</span></span>

## <a name="permissions"></a><span data-ttu-id="4dfeb-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4dfeb-105">Permissions</span></span>

<span data-ttu-id="4dfeb-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4dfeb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4dfeb-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4dfeb-108">Permission type</span></span>      | <span data-ttu-id="4dfeb-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4dfeb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4dfeb-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4dfeb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4dfeb-111">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4dfeb-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="4dfeb-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4dfeb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4dfeb-113">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4dfeb-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="4dfeb-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4dfeb-114">Application</span></span> | <span data-ttu-id="4dfeb-115">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4dfeb-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4dfeb-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4dfeb-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/versions/{version-id}/restoreVersion
POST /groups/{groupId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /me/drive/items/{item-id}/versions/{version-id}/restoreVersion
POST /sites/{siteId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /users/{userId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
```

### <a name="request-body"></a><span data-ttu-id="4dfeb-117">要求本文</span><span class="sxs-lookup"><span data-stu-id="4dfeb-117">Request body</span></span>

<span data-ttu-id="4dfeb-118">要求の本文は必要ありません。</span><span class="sxs-lookup"><span data-stu-id="4dfeb-118">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="4dfeb-119">例</span><span class="sxs-lookup"><span data-stu-id="4dfeb-119">Example</span></span>

<span data-ttu-id="4dfeb-120">この例では、`{item-id}` と `{version-id}` で指定されたファイルのバージョンを復元します。</span><span class="sxs-lookup"><span data-stu-id="4dfeb-120">This example restores a version of a file identified by `{item-id}` and `{version-id}`.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="4dfeb-121">プロトコル</span><span class="sxs-lookup"><span data-stu-id="4dfeb-121">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "restore-item-version", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/versions/{version-id}/restoreVersion
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4dfeb-122">C#</span><span class="sxs-lookup"><span data-stu-id="4dfeb-122">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/restore-item-version-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4dfeb-123">Javascript</span><span class="sxs-lookup"><span data-stu-id="4dfeb-123">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/restore-item-version-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4dfeb-124">目的-C</span><span class="sxs-lookup"><span data-stu-id="4dfeb-124">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/restore-item-version-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="4dfeb-125">応答</span><span class="sxs-lookup"><span data-stu-id="4dfeb-125">Response</span></span>

<span data-ttu-id="4dfeb-126">成功すると、API 呼び出しは `204 No content` を返します。</span><span class="sxs-lookup"><span data-stu-id="4dfeb-126">If successful, the API call returns a `204 No content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```

[item-resource]: ../resources/driveitem.md

<!--
{
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy",
  "suppressions": [
  ]
}
-->
