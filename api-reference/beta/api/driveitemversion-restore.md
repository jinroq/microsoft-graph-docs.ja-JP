---
author: JeremyKelley
description: DriveItem の旧バージョンを現在のバージョンに復元します。 旧バージョンのコンテンツを持つ新しいバージョンを作成します。しかし、ファイルの既存のバージョンはすべて保持されます。
ms.date: 09/10/2017
title: 前のバージョンを復元する
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: c3c83c695aad0ca184725d8c99783cded24ecadc
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36416570"
---
# <a name="restore-a-previous-version-of-a-driveitem"></a><span data-ttu-id="a9b25-104">DriveItem の旧バージョンを復元する</span><span class="sxs-lookup"><span data-stu-id="a9b25-104">Restore a previous version of a DriveItem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a9b25-105">DriveItem の旧バージョンを現在のバージョンに復元します。</span><span class="sxs-lookup"><span data-stu-id="a9b25-105">Restore a previous version of a DriveItem to be the current version.</span></span> <span data-ttu-id="a9b25-106">旧バージョンのコンテンツを持つ新しいバージョンを作成します。しかし、ファイルの既存のバージョンはすべて保持されます。</span><span class="sxs-lookup"><span data-stu-id="a9b25-106">This will create a new version with the contents of the previous version, but preserves all existing versions of the file.</span></span>

## <a name="permissions"></a><span data-ttu-id="a9b25-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a9b25-107">Permissions</span></span>

<span data-ttu-id="a9b25-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a9b25-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a9b25-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a9b25-110">Permission type</span></span>      | <span data-ttu-id="a9b25-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a9b25-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a9b25-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a9b25-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a9b25-113">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9b25-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="a9b25-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a9b25-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a9b25-115">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9b25-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="a9b25-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a9b25-116">Application</span></span> | <span data-ttu-id="a9b25-117">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9b25-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a9b25-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a9b25-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/versions/{version-id}/restoreVersion
POST /groups/{groupId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /me/drive/items/{item-id}/versions/{version-id}/restoreVersion
POST /sites/{siteId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /users/{userId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
```

### <a name="request-body"></a><span data-ttu-id="a9b25-119">要求本文</span><span class="sxs-lookup"><span data-stu-id="a9b25-119">Request body</span></span>

<span data-ttu-id="a9b25-120">要求の本文は必要ありません。</span><span class="sxs-lookup"><span data-stu-id="a9b25-120">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="a9b25-121">例</span><span class="sxs-lookup"><span data-stu-id="a9b25-121">Example</span></span>

<span data-ttu-id="a9b25-122">この例では、`{item-id}` と `{version-id}` で指定されたファイルのバージョンを復元します。</span><span class="sxs-lookup"><span data-stu-id="a9b25-122">This example restores a version of a file identified by `{item-id}` and `{version-id}`.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="a9b25-123">プロトコル</span><span class="sxs-lookup"><span data-stu-id="a9b25-123">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "restore-item-version", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/versions/{version-id}/restoreVersion
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a9b25-124">C#</span><span class="sxs-lookup"><span data-stu-id="a9b25-124">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/restore-item-version-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a9b25-125">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a9b25-125">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/restore-item-version-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a9b25-126">目的-C</span><span class="sxs-lookup"><span data-stu-id="a9b25-126">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/restore-item-version-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="a9b25-127">応答</span><span class="sxs-lookup"><span data-stu-id="a9b25-127">Response</span></span>

<span data-ttu-id="a9b25-128">成功すると、API 呼び出しは `204 No content` を返します。</span><span class="sxs-lookup"><span data-stu-id="a9b25-128">If successful, the API call returns a `204 No content`.</span></span>

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
