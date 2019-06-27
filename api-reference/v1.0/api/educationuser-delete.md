---
title: educationUser を削除する
description: ユーザーを削除します。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 9bcbf055daa9e598cbeb13037a4fe49d6602685d
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35274866"
---
# <a name="delete-educationuser"></a><span data-ttu-id="bb5eb-103">educationUser を削除する</span><span class="sxs-lookup"><span data-stu-id="bb5eb-103">Delete educationUser</span></span>

<span data-ttu-id="bb5eb-104">ユーザーを削除します。</span><span class="sxs-lookup"><span data-stu-id="bb5eb-104">Delete a user.</span></span>


## <a name="permissions"></a><span data-ttu-id="bb5eb-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="bb5eb-105">Permissions</span></span>
<span data-ttu-id="bb5eb-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bb5eb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb5eb-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bb5eb-108">Permission type</span></span>      | <span data-ttu-id="bb5eb-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="bb5eb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bb5eb-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bb5eb-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="bb5eb-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bb5eb-111">Not supported.</span></span>  |
|<span data-ttu-id="bb5eb-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bb5eb-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="bb5eb-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bb5eb-113">Not supported.</span></span>  |
|<span data-ttu-id="bb5eb-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bb5eb-114">Application</span></span> | <span data-ttu-id="bb5eb-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb5eb-115">EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bb5eb-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bb5eb-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/users/{id}
```
## <a name="request-headers"></a><span data-ttu-id="bb5eb-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bb5eb-117">Request headers</span></span>
| <span data-ttu-id="bb5eb-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bb5eb-118">Header</span></span>       | <span data-ttu-id="bb5eb-119">値</span><span class="sxs-lookup"><span data-stu-id="bb5eb-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bb5eb-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="bb5eb-120">Authorization</span></span>  | <span data-ttu-id="bb5eb-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="bb5eb-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bb5eb-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="bb5eb-123">Request body</span></span>
<span data-ttu-id="bb5eb-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="bb5eb-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="bb5eb-125">応答</span><span class="sxs-lookup"><span data-stu-id="bb5eb-125">Response</span></span>
<span data-ttu-id="bb5eb-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="bb5eb-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb5eb-128">例</span><span class="sxs-lookup"><span data-stu-id="bb5eb-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bb5eb-129">要求</span><span class="sxs-lookup"><span data-stu-id="bb5eb-129">Request</span></span>
<span data-ttu-id="bb5eb-130">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="bb5eb-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationuser"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/users/{user-id}
```
##### <a name="response"></a><span data-ttu-id="bb5eb-131">応答</span><span class="sxs-lookup"><span data-stu-id="bb5eb-131">Response</span></span>
<span data-ttu-id="bb5eb-132">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="bb5eb-132">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="bb5eb-133">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="bb5eb-133">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="bb5eb-134">C#</span><span class="sxs-lookup"><span data-stu-id="bb5eb-134">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_educationuser-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bb5eb-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="bb5eb-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_educationuser-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="bb5eb-136">目的-C</span><span class="sxs-lookup"><span data-stu-id="bb5eb-136">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_educationuser-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete educationUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/educationuser-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/educationuser-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/educationuser-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
