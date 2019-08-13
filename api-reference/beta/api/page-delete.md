---
title: ページを削除する
description: OneNote ページを削除します。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 9189f4003d41163008afc9449f13c417e2141fbb
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36349671"
---
# <a name="delete-page"></a><span data-ttu-id="33282-103">ページを削除する</span><span class="sxs-lookup"><span data-stu-id="33282-103">Delete page</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="33282-104">OneNote ページを削除します。</span><span class="sxs-lookup"><span data-stu-id="33282-104">Delete a OneNote page.</span></span>
## <a name="permissions"></a><span data-ttu-id="33282-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="33282-105">Permissions</span></span>
<span data-ttu-id="33282-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="33282-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="33282-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="33282-108">Permission type</span></span>      | <span data-ttu-id="33282-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="33282-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="33282-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="33282-110">Delegated (work or school account)</span></span> | <span data-ttu-id="33282-111">メモ書き込み、メモ (すべて)</span><span class="sxs-lookup"><span data-stu-id="33282-111">Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="33282-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="33282-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="33282-113">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="33282-113">Notes.ReadWrite</span></span>    |
|<span data-ttu-id="33282-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="33282-114">Application</span></span> | <span data-ttu-id="33282-115">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33282-115">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="33282-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="33282-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/onenote/pages/{id}
DELETE /users/{id | userPrincipalName}/onenote/pages/{id}
DELETE /groups/{id}/onenote/pages/{id}
DELETE /sites/{id}/onenote/pages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="33282-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="33282-117">Request headers</span></span>
| <span data-ttu-id="33282-118">名前</span><span class="sxs-lookup"><span data-stu-id="33282-118">Name</span></span>       | <span data-ttu-id="33282-119">型</span><span class="sxs-lookup"><span data-stu-id="33282-119">Type</span></span> | <span data-ttu-id="33282-120">説明</span><span class="sxs-lookup"><span data-stu-id="33282-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="33282-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="33282-121">Authorization</span></span>  | <span data-ttu-id="33282-122">string</span><span class="sxs-lookup"><span data-stu-id="33282-122">string</span></span>  | <span data-ttu-id="33282-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="33282-p102">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="33282-125">応答</span><span class="sxs-lookup"><span data-stu-id="33282-125">Response</span></span>

<span data-ttu-id="33282-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="33282-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="33282-128">例</span><span class="sxs-lookup"><span data-stu-id="33282-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="33282-129">要求</span><span class="sxs-lookup"><span data-stu-id="33282-129">Request</span></span>
<span data-ttu-id="33282-130">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="33282-130">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="33282-131">プロトコル</span><span class="sxs-lookup"><span data-stu-id="33282-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_page"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/onenote/pages/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="33282-132">C#</span><span class="sxs-lookup"><span data-stu-id="33282-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-page-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="33282-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="33282-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-page-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="33282-134">目的-C</span><span class="sxs-lookup"><span data-stu-id="33282-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-page-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="33282-135">Java</span><span class="sxs-lookup"><span data-stu-id="33282-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-page-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="33282-136">応答</span><span class="sxs-lookup"><span data-stu-id="33282-136">Response</span></span>
<span data-ttu-id="33282-137">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="33282-137">Here is an example of the response.</span></span>
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
