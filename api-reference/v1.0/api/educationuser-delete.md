---
title: educationUser を削除する
description: ユーザーを削除します。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 862dc5dff342fa1b5510a830d09e8244380deaf4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36015132"
---
# <a name="delete-educationuser"></a><span data-ttu-id="5582e-103">educationUser を削除する</span><span class="sxs-lookup"><span data-stu-id="5582e-103">Delete educationUser</span></span>

<span data-ttu-id="5582e-104">ユーザーを削除します。</span><span class="sxs-lookup"><span data-stu-id="5582e-104">Delete a user.</span></span>


## <a name="permissions"></a><span data-ttu-id="5582e-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5582e-105">Permissions</span></span>
<span data-ttu-id="5582e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5582e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5582e-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5582e-108">Permission type</span></span>      | <span data-ttu-id="5582e-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5582e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5582e-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5582e-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="5582e-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5582e-111">Not supported.</span></span>  |
|<span data-ttu-id="5582e-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5582e-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="5582e-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5582e-113">Not supported.</span></span>  |
|<span data-ttu-id="5582e-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5582e-114">Application</span></span> | <span data-ttu-id="5582e-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5582e-115">EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5582e-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5582e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/users/{id}
```
## <a name="request-headers"></a><span data-ttu-id="5582e-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5582e-117">Request headers</span></span>
| <span data-ttu-id="5582e-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5582e-118">Header</span></span>       | <span data-ttu-id="5582e-119">値</span><span class="sxs-lookup"><span data-stu-id="5582e-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5582e-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="5582e-120">Authorization</span></span>  | <span data-ttu-id="5582e-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5582e-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5582e-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="5582e-123">Request body</span></span>
<span data-ttu-id="5582e-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="5582e-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="5582e-125">応答</span><span class="sxs-lookup"><span data-stu-id="5582e-125">Response</span></span>
<span data-ttu-id="5582e-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="5582e-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5582e-128">例</span><span class="sxs-lookup"><span data-stu-id="5582e-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5582e-129">要求</span><span class="sxs-lookup"><span data-stu-id="5582e-129">Request</span></span>
<span data-ttu-id="5582e-130">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5582e-130">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="5582e-131">プロトコル</span><span class="sxs-lookup"><span data-stu-id="5582e-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationuser"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/users/{user-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5582e-132">C#</span><span class="sxs-lookup"><span data-stu-id="5582e-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5582e-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="5582e-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5582e-134">目的-C</span><span class="sxs-lookup"><span data-stu-id="5582e-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="5582e-135">Java</span><span class="sxs-lookup"><span data-stu-id="5582e-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-educationuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5582e-136">応答</span><span class="sxs-lookup"><span data-stu-id="5582e-136">Response</span></span>
<span data-ttu-id="5582e-137">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5582e-137">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete educationUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
