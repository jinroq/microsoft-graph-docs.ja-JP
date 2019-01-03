---
title: ページを更新する
description: OneNote ページの内容を更新します。
ms.openlocfilehash: 862271da69985b7386f5025d630227b6222cd64a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071639"
---
# <a name="update-page"></a><span data-ttu-id="15107-103">ページを更新する</span><span class="sxs-lookup"><span data-stu-id="15107-103">Update page</span></span>

> <span data-ttu-id="15107-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="15107-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="15107-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="15107-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="15107-106">OneNote ページの内容を更新します。</span><span class="sxs-lookup"><span data-stu-id="15107-106">Update the content of a OneNote page.</span></span>
## <a name="permissions"></a><span data-ttu-id="15107-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="15107-107">Permissions</span></span>
<span data-ttu-id="15107-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="15107-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15107-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="15107-110">Permission type</span></span>      | <span data-ttu-id="15107-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="15107-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="15107-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="15107-112">Delegated (work or school account)</span></span> | <span data-ttu-id="15107-113">Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15107-113">Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="15107-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="15107-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="15107-115">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="15107-115">Notes.ReadWrite</span></span>    |
|<span data-ttu-id="15107-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="15107-116">Application</span></span> | <span data-ttu-id="15107-117">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15107-117">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="15107-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="15107-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/onenote/pages/{id}/content
PATCH /users/{id | userPrincipalName}/onenote/pages/{id}/content
PATCH /groups/{id}/onenote/pages/{id}/content
PATCH /sites/{id}/onenote/pages/{id}/content
```
## <a name="request-headers"></a><span data-ttu-id="15107-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="15107-119">Request headers</span></span>
| <span data-ttu-id="15107-120">名前</span><span class="sxs-lookup"><span data-stu-id="15107-120">Name</span></span>       | <span data-ttu-id="15107-121">型</span><span class="sxs-lookup"><span data-stu-id="15107-121">Type</span></span> | <span data-ttu-id="15107-122">説明</span><span class="sxs-lookup"><span data-stu-id="15107-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="15107-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="15107-123">Authorization</span></span>  | <span data-ttu-id="15107-124">string</span><span class="sxs-lookup"><span data-stu-id="15107-124">string</span></span>  | <span data-ttu-id="15107-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="15107-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="15107-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="15107-127">Content-Type</span></span> | <span data-ttu-id="15107-128">string</span><span class="sxs-lookup"><span data-stu-id="15107-128">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="15107-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="15107-129">Request body</span></span>
<span data-ttu-id="15107-130">要求の本文には、ページへの変更を表す[patchContentCommand](../resources/patchcontentcommand.md)オブジェクトの配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="15107-130">In the request body, supply an array of [patchContentCommand](../resources/patchcontentcommand.md) objects that represent the changes to the page.</span></span> <span data-ttu-id="15107-131">詳細と例については、[更新プログラムの OneNote ページのコンテンツ](/graph/onenote-update-page)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="15107-131">For more information and examples, see [Update OneNote page content](/graph/onenote-update-page).</span></span>

## <a name="response"></a><span data-ttu-id="15107-132">応答</span><span class="sxs-lookup"><span data-stu-id="15107-132">Response</span></span>

<span data-ttu-id="15107-p105">成功した場合、このメソッドは `204 No Content` 応答コードを返します。PATCH 要求に対して JSON データは返されません。</span><span class="sxs-lookup"><span data-stu-id="15107-p105">If successful, this method returns a `204 No Content` response code.  No JSON data is returned for a PATCH request.</span></span>
## <a name="example"></a><span data-ttu-id="15107-135">例</span><span class="sxs-lookup"><span data-stu-id="15107-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="15107-136">要求</span><span class="sxs-lookup"><span data-stu-id="15107-136">Request</span></span>
<span data-ttu-id="15107-137">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="15107-137">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="15107-138">応答</span><span class="sxs-lookup"><span data-stu-id="15107-138">Response</span></span>
<span data-ttu-id="15107-139">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="15107-139">Here is an example of the response.</span></span> 
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
  "tocPath": ""
}-->