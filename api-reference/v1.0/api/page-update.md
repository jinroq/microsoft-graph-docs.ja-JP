---
title: ページを更新する
description: OneNote ページのコンテンツを更新します。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: e1fb7a0feb748bf32f778da255cece67e4d3fc35
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33611398"
---
# <a name="update-page"></a><span data-ttu-id="91baa-103">ページを更新する</span><span class="sxs-lookup"><span data-stu-id="91baa-103">Update page</span></span>

<span data-ttu-id="91baa-104">OneNote ページのコンテンツを更新します。</span><span class="sxs-lookup"><span data-stu-id="91baa-104">Update the content of a OneNote page.</span></span>
## <a name="permissions"></a><span data-ttu-id="91baa-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="91baa-105">Permissions</span></span>
<span data-ttu-id="91baa-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="91baa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91baa-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="91baa-108">Permission type</span></span>      | <span data-ttu-id="91baa-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="91baa-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="91baa-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="91baa-110">Delegated (work or school account)</span></span> | <span data-ttu-id="91baa-111">メモ書き込み、メモ (すべて)</span><span class="sxs-lookup"><span data-stu-id="91baa-111">Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="91baa-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="91baa-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="91baa-113">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="91baa-113">Notes.ReadWrite</span></span>    |
|<span data-ttu-id="91baa-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="91baa-114">Application</span></span> | <span data-ttu-id="91baa-115">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91baa-115">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="91baa-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="91baa-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/onenote/pages/{id}/content
PATCH /users/{id | userPrincipalName}/onenote/pages/{id}/content
PATCH /groups/{id}/onenote/pages/{id}/content
PATCH /sites/{id}/onenote/pages/{id}/content
```
## <a name="request-headers"></a><span data-ttu-id="91baa-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="91baa-117">Request headers</span></span>
| <span data-ttu-id="91baa-118">名前</span><span class="sxs-lookup"><span data-stu-id="91baa-118">Name</span></span>       | <span data-ttu-id="91baa-119">型</span><span class="sxs-lookup"><span data-stu-id="91baa-119">Type</span></span> | <span data-ttu-id="91baa-120">説明</span><span class="sxs-lookup"><span data-stu-id="91baa-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="91baa-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="91baa-121">Authorization</span></span>  | <span data-ttu-id="91baa-122">string</span><span class="sxs-lookup"><span data-stu-id="91baa-122">string</span></span>  | <span data-ttu-id="91baa-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="91baa-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="91baa-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="91baa-125">Content-Type</span></span> | <span data-ttu-id="91baa-126">string</span><span class="sxs-lookup"><span data-stu-id="91baa-126">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="91baa-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="91baa-127">Request body</span></span>
<span data-ttu-id="91baa-128">要求本文で、ページへの変更を[](../resources/patchcontentcommand.md)表す、オブジェクトの配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="91baa-128">In the request body, supply an array of [patchContentCommand](../resources/patchcontentcommand.md) objects that represent the changes to the page.</span></span> <span data-ttu-id="91baa-129">詳細と例については、「 <a href="https://msdn.microsoft.com/office/office365/howto/onenote-update-page">OneNote ページを更新</a>する」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="91baa-129">For more information and examples, see <a href="https://msdn.microsoft.com/office/office365/howto/onenote-update-page">Update OneNote pages</a>.</span></span>

## <a name="response"></a><span data-ttu-id="91baa-130">応答</span><span class="sxs-lookup"><span data-stu-id="91baa-130">Response</span></span>

<span data-ttu-id="91baa-131">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="91baa-131">If successful, this method returns a `204 No Content` response code.</span></span>  <span data-ttu-id="91baa-132">PATCH 要求に対して JSON データは返されません。</span><span class="sxs-lookup"><span data-stu-id="91baa-132">No JSON data is returned for a PATCH request.</span></span>
## <a name="example"></a><span data-ttu-id="91baa-133">例</span><span class="sxs-lookup"><span data-stu-id="91baa-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="91baa-134">要求</span><span class="sxs-lookup"><span data-stu-id="91baa-134">Request</span></span>
<span data-ttu-id="91baa-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="91baa-135">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="91baa-136">応答</span><span class="sxs-lookup"><span data-stu-id="91baa-136">Response</span></span>
<span data-ttu-id="91baa-137">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="91baa-137">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenotePage"
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="91baa-138">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="91baa-138">SDK sample code</span></span>

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="91baa-139">Java</span><span class="sxs-lookup"><span data-stu-id="91baa-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_page-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update page",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/page-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
