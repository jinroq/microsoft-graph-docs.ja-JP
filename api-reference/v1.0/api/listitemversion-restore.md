---
title: 旧バージョンのリスト アイテムを復元する
description: 旧バージョンのリスト アイテムを現在のバージョンに復元します。 旧バージョンのコンテンツを持つ新しいバージョンを作成します。しかし、アイテムの既存のバージョンはすべて保持されます。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: ff3a9149113ee03aade7c7e2ea943a2bd6446a9a
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35271982"
---
# <a name="restore-a-previous-version-of-a-listitem"></a><span data-ttu-id="d5ab7-104">旧バージョンのリスト アイテムを復元する</span><span class="sxs-lookup"><span data-stu-id="d5ab7-104">Restore a previous version of a ListItem</span></span>

<span data-ttu-id="d5ab7-105">旧バージョンのリスト アイテムを現在のバージョンに復元します。</span><span class="sxs-lookup"><span data-stu-id="d5ab7-105">Restore a previous version of a ListItem to be the current version.</span></span> <span data-ttu-id="d5ab7-106">旧バージョンのコンテンツを持つ新しいバージョンを作成します。しかし、アイテムの既存のバージョンはすべて保持されます。</span><span class="sxs-lookup"><span data-stu-id="d5ab7-106">This will create a new version with the contents of the previous version, but preserves all existing versions of the item.</span></span>

## <a name="permissions"></a><span data-ttu-id="d5ab7-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d5ab7-107">Permissions</span></span>

<span data-ttu-id="d5ab7-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d5ab7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="d5ab7-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d5ab7-110">Permission type</span></span>             |         <span data-ttu-id="d5ab7-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d5ab7-111">Permissions (from least to most privileged)</span></span>          |
| :------------------------------------- | :----------------------------------------------------------- |
| <span data-ttu-id="d5ab7-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d5ab7-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="d5ab7-113">Sites.ReadWrite.All、Sites.Manage.All、Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="d5ab7-113">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |
| <span data-ttu-id="d5ab7-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d5ab7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d5ab7-115">該当なし</span><span class="sxs-lookup"><span data-stu-id="d5ab7-115">n/a</span></span>                                                          |
| <span data-ttu-id="d5ab7-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d5ab7-116">Application</span></span>                            | <span data-ttu-id="d5ab7-117">Sites.ReadWrite.All、Sites.Manage.All、Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="d5ab7-117">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d5ab7-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d5ab7-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /sites/{site-id}/items/{item-id}/versions/{version-id}/restoreVersion
POST /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

### <a name="request-body"></a><span data-ttu-id="d5ab7-119">要求本文</span><span class="sxs-lookup"><span data-stu-id="d5ab7-119">Request body</span></span>

<span data-ttu-id="d5ab7-120">要求の本文は必要ありません。</span><span class="sxs-lookup"><span data-stu-id="d5ab7-120">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="d5ab7-121">例</span><span class="sxs-lookup"><span data-stu-id="d5ab7-121">Example</span></span>

<span data-ttu-id="d5ab7-122">この例では、`{item-id}` と `{version-id}` で識別されるリスト アイテムのバージョンを復元します。</span><span class="sxs-lookup"><span data-stu-id="d5ab7-122">This example restores a version of a listItem identified by `{item-id}` and `{version-id}`.</span></span>

<!-- { "blockType": "request", "name": "restore-item-version-listItem", "scopes": "files.readwrite sites.readwrite.all", "target": "action", "tags": "service.graph service.sharepoint" } -->

```http
POST /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

## <a name="response"></a><span data-ttu-id="d5ab7-123">応答</span><span class="sxs-lookup"><span data-stu-id="d5ab7-123">Response</span></span>

<span data-ttu-id="d5ab7-124">成功すると、API 呼び出しは `204 No Content` を返します。</span><span class="sxs-lookup"><span data-stu-id="d5ab7-124">If successful, the API call returns a `204 No Content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="d5ab7-125">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="d5ab7-125">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d5ab7-126">C#</span><span class="sxs-lookup"><span data-stu-id="d5ab7-126">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/restore-item-version-listItem-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d5ab7-127">Javascript</span><span class="sxs-lookup"><span data-stu-id="d5ab7-127">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/restore-item-version-listItem-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="d5ab7-128">目的-C</span><span class="sxs-lookup"><span data-stu-id="d5ab7-128">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/restore-item-version-listItem-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- {
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy",
  "suppressions": [
    "Error: /api-reference/v1.0/api/listitemversion-restore.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/listitemversion-restore.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/listitemversion-restore.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->
