---
title: ページを更新する
description: OneNote ページのコンテンツを更新します。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 95022c80220349176289fd2d0797571cee45c5bd
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36349601"
---
# <a name="update-page"></a><span data-ttu-id="ce45b-103">ページを更新する</span><span class="sxs-lookup"><span data-stu-id="ce45b-103">Update page</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce45b-104">OneNote ページのコンテンツを更新します。</span><span class="sxs-lookup"><span data-stu-id="ce45b-104">Update the content of a OneNote page.</span></span>
## <a name="permissions"></a><span data-ttu-id="ce45b-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ce45b-105">Permissions</span></span>
<span data-ttu-id="ce45b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ce45b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ce45b-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ce45b-108">Permission type</span></span>      | <span data-ttu-id="ce45b-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ce45b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ce45b-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ce45b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ce45b-111">メモ書き込み、メモ (すべて)</span><span class="sxs-lookup"><span data-stu-id="ce45b-111">Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="ce45b-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ce45b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ce45b-113">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ce45b-113">Notes.ReadWrite</span></span>    |
|<span data-ttu-id="ce45b-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ce45b-114">Application</span></span> | <span data-ttu-id="ce45b-115">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce45b-115">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ce45b-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ce45b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/onenote/pages/{id}/content
PATCH /users/{id | userPrincipalName}/onenote/pages/{id}/content
PATCH /groups/{id}/onenote/pages/{id}/content
PATCH /sites/{id}/onenote/pages/{id}/content
```
## <a name="request-headers"></a><span data-ttu-id="ce45b-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ce45b-117">Request headers</span></span>
| <span data-ttu-id="ce45b-118">名前</span><span class="sxs-lookup"><span data-stu-id="ce45b-118">Name</span></span>       | <span data-ttu-id="ce45b-119">型</span><span class="sxs-lookup"><span data-stu-id="ce45b-119">Type</span></span> | <span data-ttu-id="ce45b-120">説明</span><span class="sxs-lookup"><span data-stu-id="ce45b-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ce45b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ce45b-121">Authorization</span></span>  | <span data-ttu-id="ce45b-122">string</span><span class="sxs-lookup"><span data-stu-id="ce45b-122">string</span></span>  | <span data-ttu-id="ce45b-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ce45b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ce45b-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ce45b-125">Content-Type</span></span> | <span data-ttu-id="ce45b-126">string</span><span class="sxs-lookup"><span data-stu-id="ce45b-126">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="ce45b-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="ce45b-127">Request body</span></span>
<span data-ttu-id="ce45b-128">要求本文で、ページへの変更を[](../resources/patchcontentcommand.md)表す、オブジェクトの配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="ce45b-128">In the request body, supply an array of [patchContentCommand](../resources/patchcontentcommand.md) objects that represent the changes to the page.</span></span> <span data-ttu-id="ce45b-129">詳細と例については、「 [OneNote ページコンテンツを更新](/graph/onenote-update-page)する」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ce45b-129">For more information and examples, see [Update OneNote page content](/graph/onenote-update-page).</span></span>

## <a name="response"></a><span data-ttu-id="ce45b-130">応答</span><span class="sxs-lookup"><span data-stu-id="ce45b-130">Response</span></span>

<span data-ttu-id="ce45b-131">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="ce45b-131">If successful, this method returns a `204 No Content` response code.</span></span>  <span data-ttu-id="ce45b-132">PATCH 要求に対して JSON データは返されません。</span><span class="sxs-lookup"><span data-stu-id="ce45b-132">No JSON data is returned for a PATCH request.</span></span>
## <a name="example"></a><span data-ttu-id="ce45b-133">例</span><span class="sxs-lookup"><span data-stu-id="ce45b-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ce45b-134">要求</span><span class="sxs-lookup"><span data-stu-id="ce45b-134">Request</span></span>
<span data-ttu-id="ce45b-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ce45b-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ce45b-136">プロトコル</span><span class="sxs-lookup"><span data-stu-id="ce45b-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_page"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/onenote/pages/{id}/content
Content-type: application/json
Content-length: 312

[
   {
    'target':'#para-id',
    'action':'insert',
    'position':'before',
    'content':'<img src="image-url-or-part-name" alt="image-alt-text" />'
  }, 
  {
    'target':'#list-id',
    'action':'append',
    'content':'<li>new-page-content</li>'
  }
]
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ce45b-137">C#</span><span class="sxs-lookup"><span data-stu-id="ce45b-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-page-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ce45b-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ce45b-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-page-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ce45b-139">目的-C</span><span class="sxs-lookup"><span data-stu-id="ce45b-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-page-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="ce45b-140">Java</span><span class="sxs-lookup"><span data-stu-id="ce45b-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-page-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ce45b-141">応答</span><span class="sxs-lookup"><span data-stu-id="ce45b-141">Response</span></span>
<span data-ttu-id="ce45b-142">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="ce45b-142">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenotePage"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update page",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
