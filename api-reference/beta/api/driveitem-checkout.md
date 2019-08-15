---
author: JeremyKelley
description: driveItem リソースをチェックアウトして、他者がドキュメントを編集できないようにします。また、ドキュメントがチェックインされるまで、変更内容が表示されないようにします。
ms.date: 09/10/2017
title: ファイルをチェックアウトする
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: adde2c3deb03bf1f45a673ff6cc5d6d7a844544e
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36416864"
---
# <a name="check-out-a-driveitem-resource"></a><span data-ttu-id="bc62d-103">DriveItem リソースをチェックアウトする</span><span class="sxs-lookup"><span data-stu-id="bc62d-103">Check-out a DriveItem resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bc62d-104">driveItem リソースをチェックアウトして、他者がドキュメントを編集できないようにします。また、ドキュメントが[チェックイン](driveitem-checkin.md)されるまで、変更内容が表示されないようにします。</span><span class="sxs-lookup"><span data-stu-id="bc62d-104">Check-out a driveItem resource to prevent others from editing the document, and your changes from being visible until the documented is [checked-in](driveitem-checkin.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="bc62d-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="bc62d-105">Permissions</span></span>

<span data-ttu-id="bc62d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bc62d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bc62d-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bc62d-108">Permission type</span></span>      | <span data-ttu-id="bc62d-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="bc62d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bc62d-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bc62d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bc62d-111">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc62d-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="bc62d-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bc62d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bc62d-113">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc62d-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="bc62d-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bc62d-114">Application</span></span> | <span data-ttu-id="bc62d-115">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc62d-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bc62d-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bc62d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/checkout
POST /groups/{groupId}/drive/items/{itemId}/checkout
POST /me/drive/items/{item-id}/checkout
POST /sites/{siteId}/drive/items/{itemId}/checkout
POST /users/{userId}/drive/items/{itemId}/checkout
```

### <a name="request-body"></a><span data-ttu-id="bc62d-117">要求本文</span><span class="sxs-lookup"><span data-stu-id="bc62d-117">Request body</span></span>

<span data-ttu-id="bc62d-118">要求の本文は必要ありません。</span><span class="sxs-lookup"><span data-stu-id="bc62d-118">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="bc62d-119">例</span><span class="sxs-lookup"><span data-stu-id="bc62d-119">Example</span></span>

<span data-ttu-id="bc62d-120">この例では、`{item-id}` で識別されるファイルをチェックアウトします。</span><span class="sxs-lookup"><span data-stu-id="bc62d-120">This example checks out a file identified by `{item-id}`.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="bc62d-121">プロトコル</span><span class="sxs-lookup"><span data-stu-id="bc62d-121">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "checkout-item", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/checkout
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="bc62d-122">C#</span><span class="sxs-lookup"><span data-stu-id="bc62d-122">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/checkout-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bc62d-123">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bc62d-123">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/checkout-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="bc62d-124">目的-C</span><span class="sxs-lookup"><span data-stu-id="bc62d-124">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/checkout-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="bc62d-125">応答</span><span class="sxs-lookup"><span data-stu-id="bc62d-125">Response</span></span>

<span data-ttu-id="bc62d-126">成功すると、API 呼び出しは `204 No content` を返します。</span><span class="sxs-lookup"><span data-stu-id="bc62d-126">If successful, the API call returns a `204 No content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```

### <a name="remarks"></a><span data-ttu-id="bc62d-127">備考</span><span class="sxs-lookup"><span data-stu-id="bc62d-127">Remarks</span></span>


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
