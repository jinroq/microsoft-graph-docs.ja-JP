---
title: DriveItem の旧バージョンを復元する
description: DriveItem の旧バージョンを現在のバージョンに復元します。 旧バージョンのコンテンツを持つ新しいバージョンを作成します。しかし、ファイルの既存のバージョンはすべて保持されます。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 53a8f5e40e06ef90662a55c44ca718bc82f4fb4b
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33616245"
---
# <a name="restore-a-previous-version-of-a-driveitem"></a><span data-ttu-id="bdd18-104">DriveItem の旧バージョンを復元する</span><span class="sxs-lookup"><span data-stu-id="bdd18-104">Restore a previous version of a DriveItem</span></span>

<span data-ttu-id="bdd18-105">DriveItem の旧バージョンを現在のバージョンに復元します。</span><span class="sxs-lookup"><span data-stu-id="bdd18-105">Restore a previous version of a DriveItem to be the current version.</span></span> <span data-ttu-id="bdd18-106">旧バージョンのコンテンツを持つ新しいバージョンを作成します。しかし、ファイルの既存のバージョンはすべて保持されます。</span><span class="sxs-lookup"><span data-stu-id="bdd18-106">This will create a new version with the contents of the previous version, but preserves all existing versions of the file.</span></span>

## <a name="permissions"></a><span data-ttu-id="bdd18-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="bdd18-107">Permissions</span></span>

<span data-ttu-id="bdd18-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bdd18-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bdd18-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bdd18-110">Permission type</span></span>      | <span data-ttu-id="bdd18-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="bdd18-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bdd18-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bdd18-112">Delegated (work or school account)</span></span> | <span data-ttu-id="bdd18-113">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bdd18-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="bdd18-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bdd18-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bdd18-115">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bdd18-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="bdd18-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bdd18-116">Application</span></span> | <span data-ttu-id="bdd18-117">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bdd18-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bdd18-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bdd18-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/versions/{version-id}/restoreVersion
POST /groups/{groupId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /me/drive/items/{item-id}/versions/{version-id}/restoreVersion
POST /sites/{siteId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /users/{userId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
```

### <a name="request-body"></a><span data-ttu-id="bdd18-119">要求本文</span><span class="sxs-lookup"><span data-stu-id="bdd18-119">Request body</span></span>

<span data-ttu-id="bdd18-120">要求の本文は必要ありません。</span><span class="sxs-lookup"><span data-stu-id="bdd18-120">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="bdd18-121">例</span><span class="sxs-lookup"><span data-stu-id="bdd18-121">Example</span></span>

<span data-ttu-id="bdd18-122">この例では、`{item-id}` と `{version-id}` で指定されたファイルのバージョンを復元します。</span><span class="sxs-lookup"><span data-stu-id="bdd18-122">This example restores a version of a file identified by `{item-id}` and `{version-id}`.</span></span>

<!-- { "blockType": "request", "name": "restore-item-version", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

## <a name="response"></a><span data-ttu-id="bdd18-123">応答</span><span class="sxs-lookup"><span data-stu-id="bdd18-123">Response</span></span>

<span data-ttu-id="bdd18-124">成功すると、API 呼び出しは `204 No Content` を返します。</span><span class="sxs-lookup"><span data-stu-id="bdd18-124">If successful, the API call returns a `204 No Content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="bdd18-125">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="bdd18-125">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="bdd18-126">Visual</span><span class="sxs-lookup"><span data-stu-id="bdd18-126">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/restore-item-version-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bdd18-127">Java</span><span class="sxs-lookup"><span data-stu-id="bdd18-127">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/restore-item-version-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy",
  "suppressions": [
    "Error: /api-reference/v1.0/api/driveitemversion-restore.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/driveitemversion-restore.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->
