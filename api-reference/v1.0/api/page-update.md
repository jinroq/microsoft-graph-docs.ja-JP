---
title: ページを更新する
description: OneNote ページのコンテンツを更新します。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 1c5b77ddbc236dc78242397702a9d43294bea0eb
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35886534"
---
# <a name="update-page"></a><span data-ttu-id="54d43-103">ページを更新する</span><span class="sxs-lookup"><span data-stu-id="54d43-103">Update page</span></span>

<span data-ttu-id="54d43-104">OneNote ページのコンテンツを更新します。</span><span class="sxs-lookup"><span data-stu-id="54d43-104">Update the content of a OneNote page.</span></span>
## <a name="permissions"></a><span data-ttu-id="54d43-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="54d43-105">Permissions</span></span>
<span data-ttu-id="54d43-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="54d43-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="54d43-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="54d43-108">Permission type</span></span>      | <span data-ttu-id="54d43-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="54d43-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="54d43-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="54d43-110">Delegated (work or school account)</span></span> | <span data-ttu-id="54d43-111">メモ書き込み、メモ (すべて)</span><span class="sxs-lookup"><span data-stu-id="54d43-111">Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="54d43-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="54d43-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="54d43-113">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="54d43-113">Notes.ReadWrite</span></span>    |
|<span data-ttu-id="54d43-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="54d43-114">Application</span></span> | <span data-ttu-id="54d43-115">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54d43-115">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="54d43-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="54d43-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/onenote/pages/{id}/content
PATCH /users/{id | userPrincipalName}/onenote/pages/{id}/content
PATCH /groups/{id}/onenote/pages/{id}/content
PATCH /sites/{id}/onenote/pages/{id}/content
```
## <a name="request-headers"></a><span data-ttu-id="54d43-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="54d43-117">Request headers</span></span>
| <span data-ttu-id="54d43-118">名前</span><span class="sxs-lookup"><span data-stu-id="54d43-118">Name</span></span>       | <span data-ttu-id="54d43-119">型</span><span class="sxs-lookup"><span data-stu-id="54d43-119">Type</span></span> | <span data-ttu-id="54d43-120">説明</span><span class="sxs-lookup"><span data-stu-id="54d43-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="54d43-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="54d43-121">Authorization</span></span>  | <span data-ttu-id="54d43-122">string</span><span class="sxs-lookup"><span data-stu-id="54d43-122">string</span></span>  | <span data-ttu-id="54d43-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="54d43-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="54d43-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="54d43-125">Content-Type</span></span> | <span data-ttu-id="54d43-126">string</span><span class="sxs-lookup"><span data-stu-id="54d43-126">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="54d43-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="54d43-127">Request body</span></span>
<span data-ttu-id="54d43-128">要求本文で、ページへの変更を[](../resources/patchcontentcommand.md)表す、オブジェクトの配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="54d43-128">In the request body, supply an array of [patchContentCommand](../resources/patchcontentcommand.md) objects that represent the changes to the page.</span></span> <span data-ttu-id="54d43-129">詳細と例については、「 <a href="https://msdn.microsoft.com/office/office365/howto/onenote-update-page">OneNote ページを更新</a>する」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="54d43-129">For more information and examples, see <a href="https://msdn.microsoft.com/office/office365/howto/onenote-update-page">Update OneNote pages</a>.</span></span>

## <a name="response"></a><span data-ttu-id="54d43-130">応答</span><span class="sxs-lookup"><span data-stu-id="54d43-130">Response</span></span>

<span data-ttu-id="54d43-131">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="54d43-131">If successful, this method returns a `204 No Content` response code.</span></span>  <span data-ttu-id="54d43-132">PATCH 要求に対して JSON データは返されません。</span><span class="sxs-lookup"><span data-stu-id="54d43-132">No JSON data is returned for a PATCH request.</span></span>
## <a name="example"></a><span data-ttu-id="54d43-133">例</span><span class="sxs-lookup"><span data-stu-id="54d43-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="54d43-134">要求</span><span class="sxs-lookup"><span data-stu-id="54d43-134">Request</span></span>
<span data-ttu-id="54d43-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="54d43-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="54d43-136">プロトコル</span><span class="sxs-lookup"><span data-stu-id="54d43-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_page"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/onenote/pages/{id}/content
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="54d43-137">C#</span><span class="sxs-lookup"><span data-stu-id="54d43-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-page-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="54d43-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="54d43-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-page-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="54d43-139">目的-C</span><span class="sxs-lookup"><span data-stu-id="54d43-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-page-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="54d43-140">Java</span><span class="sxs-lookup"><span data-stu-id="54d43-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-page-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="54d43-141">応答</span><span class="sxs-lookup"><span data-stu-id="54d43-141">Response</span></span>
<span data-ttu-id="54d43-142">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="54d43-142">Here is an example of the response.</span></span> 
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
<!-- {
  "type": "#page.annotation",
  "description": "Update page",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
