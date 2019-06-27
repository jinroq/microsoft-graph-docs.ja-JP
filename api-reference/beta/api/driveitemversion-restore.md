---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 前のバージョンを復元する
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: ede7eb6275a4d23c715a3c981686355fc20aa369
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35259949"
---
# <a name="restore-a-previous-version-of-a-driveitem"></a><span data-ttu-id="a891b-102">DriveItem の旧バージョンを復元する</span><span class="sxs-lookup"><span data-stu-id="a891b-102">Restore a previous version of a DriveItem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a891b-103">DriveItem の旧バージョンを現在のバージョンに復元します。</span><span class="sxs-lookup"><span data-stu-id="a891b-103">Restore a previous version of a DriveItem to be the current version.</span></span> <span data-ttu-id="a891b-104">旧バージョンのコンテンツを持つ新しいバージョンを作成します。しかし、ファイルの既存のバージョンはすべて保持されます。</span><span class="sxs-lookup"><span data-stu-id="a891b-104">This will create a new version with the contents of the previous version, but preserves all existing versions of the file.</span></span>

## <a name="permissions"></a><span data-ttu-id="a891b-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a891b-105">Permissions</span></span>

<span data-ttu-id="a891b-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a891b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a891b-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a891b-108">Permission type</span></span>      | <span data-ttu-id="a891b-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a891b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a891b-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a891b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a891b-111">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a891b-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="a891b-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a891b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a891b-113">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a891b-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="a891b-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a891b-114">Application</span></span> | <span data-ttu-id="a891b-115">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a891b-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a891b-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a891b-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/versions/{version-id}/restoreVersion
POST /groups/{groupId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /me/drive/items/{item-id}/versions/{version-id}/restoreVersion
POST /sites/{siteId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /users/{userId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
```

### <a name="request-body"></a><span data-ttu-id="a891b-117">要求本文</span><span class="sxs-lookup"><span data-stu-id="a891b-117">Request body</span></span>

<span data-ttu-id="a891b-118">要求の本文は必要ありません。</span><span class="sxs-lookup"><span data-stu-id="a891b-118">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="a891b-119">例</span><span class="sxs-lookup"><span data-stu-id="a891b-119">Example</span></span>

<span data-ttu-id="a891b-120">この例では、`{item-id}` と `{version-id}` で指定されたファイルのバージョンを復元します。</span><span class="sxs-lookup"><span data-stu-id="a891b-120">This example restores a version of a file identified by `{item-id}` and `{version-id}`.</span></span>

<!-- { "blockType": "request", "name": "restore-item-version", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

## <a name="response"></a><span data-ttu-id="a891b-121">応答</span><span class="sxs-lookup"><span data-stu-id="a891b-121">Response</span></span>

<span data-ttu-id="a891b-122">成功すると、API 呼び出しは `204 No content` を返します。</span><span class="sxs-lookup"><span data-stu-id="a891b-122">If successful, the API call returns a `204 No content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="a891b-123">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="a891b-123">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="a891b-124">C#</span><span class="sxs-lookup"><span data-stu-id="a891b-124">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/restore-item-version-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a891b-125">Javascript</span><span class="sxs-lookup"><span data-stu-id="a891b-125">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/restore-item-version-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="a891b-126">目的-C</span><span class="sxs-lookup"><span data-stu-id="a891b-126">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/restore-item-version-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

[item-resource]: ../resources/driveitem.md

<!--
{
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy",
  "suppressions": [
    "Error: /api-reference/beta/api/driveitemversion-restore.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/driveitemversion-restore.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/driveitemversion-restore.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
