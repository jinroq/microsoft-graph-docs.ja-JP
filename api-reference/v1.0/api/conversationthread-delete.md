---
title: Delete conversationThread
description: conversationThread を削除します。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 2779ae7353976a73a675395c653439f4d58f143b
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35883657"
---
# <a name="delete-conversationthread"></a><span data-ttu-id="018d8-103">Delete conversationThread</span><span class="sxs-lookup"><span data-stu-id="018d8-103">Delete conversationThread</span></span>

<span data-ttu-id="018d8-104">conversationThread を削除します。</span><span class="sxs-lookup"><span data-stu-id="018d8-104">Delete conversationThread.</span></span>
## <a name="permissions"></a><span data-ttu-id="018d8-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="018d8-105">Permissions</span></span>
<span data-ttu-id="018d8-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="018d8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="018d8-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="018d8-108">Permission type</span></span>      | <span data-ttu-id="018d8-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="018d8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="018d8-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="018d8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="018d8-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="018d8-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="018d8-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="018d8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="018d8-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="018d8-113">Not supported.</span></span>    |
|<span data-ttu-id="018d8-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="018d8-114">Application</span></span> | <span data-ttu-id="018d8-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="018d8-115">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="018d8-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="018d8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/threads/{id}
DELETE /groups/{id}/conversations/{id}/threads/{id}

```
## <a name="request-headers"></a><span data-ttu-id="018d8-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="018d8-117">Request headers</span></span>
| <span data-ttu-id="018d8-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="018d8-118">Header</span></span>       | <span data-ttu-id="018d8-119">値</span><span class="sxs-lookup"><span data-stu-id="018d8-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="018d8-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="018d8-120">Authorization</span></span>  | <span data-ttu-id="018d8-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="018d8-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="018d8-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="018d8-123">Request body</span></span>
<span data-ttu-id="018d8-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="018d8-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="018d8-125">応答</span><span class="sxs-lookup"><span data-stu-id="018d8-125">Response</span></span>

<span data-ttu-id="018d8-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="018d8-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="018d8-128">例</span><span class="sxs-lookup"><span data-stu-id="018d8-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="018d8-129">要求</span><span class="sxs-lookup"><span data-stu-id="018d8-129">Request</span></span>
<span data-ttu-id="018d8-130">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="018d8-130">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="018d8-131">プロトコル</span><span class="sxs-lookup"><span data-stu-id="018d8-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_conversationthread"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="018d8-132">C#</span><span class="sxs-lookup"><span data-stu-id="018d8-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-conversationthread-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="018d8-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="018d8-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-conversationthread-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="018d8-134">目的-C</span><span class="sxs-lookup"><span data-stu-id="018d8-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-conversationthread-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="018d8-135">Java</span><span class="sxs-lookup"><span data-stu-id="018d8-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-conversationthread-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="018d8-136">応答</span><span class="sxs-lookup"><span data-stu-id="018d8-136">Response</span></span>
<span data-ttu-id="018d8-137">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="018d8-137">Here is an example of the response.</span></span> 
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
  "description": "Delete conversationThread",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
