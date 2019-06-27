---
title: ページを削除する
description: OneNote ページを削除します。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: f8dea5fcd299426545510c6f2d024e51617c243e
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35274278"
---
# <a name="delete-page"></a><span data-ttu-id="1c4d4-103">ページを削除する</span><span class="sxs-lookup"><span data-stu-id="1c4d4-103">Delete page</span></span>

<span data-ttu-id="1c4d4-104">OneNote ページを削除します。</span><span class="sxs-lookup"><span data-stu-id="1c4d4-104">Delete a OneNote page.</span></span>
## <a name="permissions"></a><span data-ttu-id="1c4d4-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1c4d4-105">Permissions</span></span>
<span data-ttu-id="1c4d4-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1c4d4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c4d4-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1c4d4-108">Permission type</span></span>      | <span data-ttu-id="1c4d4-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1c4d4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1c4d4-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1c4d4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1c4d4-111">メモ書き込み、メモ (すべて)</span><span class="sxs-lookup"><span data-stu-id="1c4d4-111">Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="1c4d4-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1c4d4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1c4d4-113">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1c4d4-113">Notes.ReadWrite</span></span>    |
|<span data-ttu-id="1c4d4-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1c4d4-114">Application</span></span> | <span data-ttu-id="1c4d4-115">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c4d4-115">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1c4d4-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1c4d4-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/onenote/pages/{id}
DELETE /users/{id | userPrincipalName}/onenote/pages/{id}
DELETE /groups/{id}/onenote/pages/{id}
DELETE /sites/{id}/onenote/pages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="1c4d4-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1c4d4-117">Request headers</span></span>
| <span data-ttu-id="1c4d4-118">名前</span><span class="sxs-lookup"><span data-stu-id="1c4d4-118">Name</span></span>       | <span data-ttu-id="1c4d4-119">型</span><span class="sxs-lookup"><span data-stu-id="1c4d4-119">Type</span></span> | <span data-ttu-id="1c4d4-120">説明</span><span class="sxs-lookup"><span data-stu-id="1c4d4-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1c4d4-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1c4d4-121">Authorization</span></span>  | <span data-ttu-id="1c4d4-122">string</span><span class="sxs-lookup"><span data-stu-id="1c4d4-122">string</span></span>  | <span data-ttu-id="1c4d4-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="1c4d4-p102">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="1c4d4-125">応答</span><span class="sxs-lookup"><span data-stu-id="1c4d4-125">Response</span></span>

<span data-ttu-id="1c4d4-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="1c4d4-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1c4d4-128">例</span><span class="sxs-lookup"><span data-stu-id="1c4d4-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1c4d4-129">要求</span><span class="sxs-lookup"><span data-stu-id="1c4d4-129">Request</span></span>
<span data-ttu-id="1c4d4-130">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1c4d4-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_page"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/onenote/pages/{id}
```
##### <a name="response"></a><span data-ttu-id="1c4d4-131">応答</span><span class="sxs-lookup"><span data-stu-id="1c4d4-131">Response</span></span>
<span data-ttu-id="1c4d4-132">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="1c4d4-132">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="1c4d4-133">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="1c4d4-133">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="1c4d4-134">C#</span><span class="sxs-lookup"><span data-stu-id="1c4d4-134">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_page-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1c4d4-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="1c4d4-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_page-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="1c4d4-136">目的-C</span><span class="sxs-lookup"><span data-stu-id="1c4d4-136">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_page-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete page",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/page-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/page-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/page-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
