---
title: ページを削除する
description: OneNote ページを削除します。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: eeec6fea8a4d4ca374af4f2503240534b2e378fa
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36413833"
---
# <a name="delete-page"></a><span data-ttu-id="03651-103">ページを削除する</span><span class="sxs-lookup"><span data-stu-id="03651-103">Delete page</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="03651-104">OneNote ページを削除します。</span><span class="sxs-lookup"><span data-stu-id="03651-104">Delete a OneNote page.</span></span>
## <a name="permissions"></a><span data-ttu-id="03651-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="03651-105">Permissions</span></span>
<span data-ttu-id="03651-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="03651-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03651-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="03651-108">Permission type</span></span>      | <span data-ttu-id="03651-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="03651-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="03651-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="03651-110">Delegated (work or school account)</span></span> | <span data-ttu-id="03651-111">メモ書き込み、メモ (すべて)</span><span class="sxs-lookup"><span data-stu-id="03651-111">Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="03651-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="03651-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="03651-113">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="03651-113">Notes.ReadWrite</span></span>    |
|<span data-ttu-id="03651-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="03651-114">Application</span></span> | <span data-ttu-id="03651-115">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03651-115">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="03651-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="03651-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/onenote/pages/{id}
DELETE /users/{id | userPrincipalName}/onenote/pages/{id}
DELETE /groups/{id}/onenote/pages/{id}
DELETE /sites/{id}/onenote/pages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="03651-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="03651-117">Request headers</span></span>
| <span data-ttu-id="03651-118">名前</span><span class="sxs-lookup"><span data-stu-id="03651-118">Name</span></span>       | <span data-ttu-id="03651-119">型</span><span class="sxs-lookup"><span data-stu-id="03651-119">Type</span></span> | <span data-ttu-id="03651-120">説明</span><span class="sxs-lookup"><span data-stu-id="03651-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="03651-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="03651-121">Authorization</span></span>  | <span data-ttu-id="03651-122">string</span><span class="sxs-lookup"><span data-stu-id="03651-122">string</span></span>  | <span data-ttu-id="03651-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="03651-p102">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="03651-125">応答</span><span class="sxs-lookup"><span data-stu-id="03651-125">Response</span></span>

<span data-ttu-id="03651-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="03651-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="03651-128">例</span><span class="sxs-lookup"><span data-stu-id="03651-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="03651-129">要求</span><span class="sxs-lookup"><span data-stu-id="03651-129">Request</span></span>
<span data-ttu-id="03651-130">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="03651-130">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="03651-131">プロトコル</span><span class="sxs-lookup"><span data-stu-id="03651-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_page"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/onenote/pages/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="03651-132">C#</span><span class="sxs-lookup"><span data-stu-id="03651-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-page-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="03651-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="03651-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-page-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="03651-134">目的-C</span><span class="sxs-lookup"><span data-stu-id="03651-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-page-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="03651-135">応答</span><span class="sxs-lookup"><span data-stu-id="03651-135">Response</span></span>
<span data-ttu-id="03651-136">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="03651-136">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete page",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
