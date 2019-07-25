---
title: 会話スレッドを削除する
description: thread オブジェクトを削除します。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 4f6963504523b1f0cf80092fa2a742d7483279b1
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35858725"
---
# <a name="delete-conversation-thread"></a><span data-ttu-id="78505-103">会話スレッドを削除する</span><span class="sxs-lookup"><span data-stu-id="78505-103">Delete conversation thread</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="78505-104">[thread](../resources/conversationthread.md) オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="78505-104">Delete a [thread](../resources/conversationthread.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="78505-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="78505-105">Permissions</span></span>
<span data-ttu-id="78505-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="78505-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="78505-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="78505-108">Permission type</span></span>      | <span data-ttu-id="78505-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="78505-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="78505-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="78505-110">Delegated (work or school account)</span></span> | <span data-ttu-id="78505-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78505-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="78505-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="78505-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="78505-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="78505-113">Not supported.</span></span>    |
|<span data-ttu-id="78505-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="78505-114">Application</span></span> | <span data-ttu-id="78505-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="78505-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="78505-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="78505-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/threads/{id}
```

## <a name="request-headers"></a><span data-ttu-id="78505-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="78505-117">Request headers</span></span>
| <span data-ttu-id="78505-118">名前</span><span class="sxs-lookup"><span data-stu-id="78505-118">Name</span></span>       | <span data-ttu-id="78505-119">型</span><span class="sxs-lookup"><span data-stu-id="78505-119">Type</span></span> | <span data-ttu-id="78505-120">説明</span><span class="sxs-lookup"><span data-stu-id="78505-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="78505-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="78505-121">Authorization</span></span>  | <span data-ttu-id="78505-122">string</span><span class="sxs-lookup"><span data-stu-id="78505-122">string</span></span>  | <span data-ttu-id="78505-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="78505-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="78505-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="78505-125">Request body</span></span>
<span data-ttu-id="78505-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="78505-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="78505-127">応答</span><span class="sxs-lookup"><span data-stu-id="78505-127">Response</span></span>
<span data-ttu-id="78505-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="78505-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="78505-130">例</span><span class="sxs-lookup"><span data-stu-id="78505-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="78505-131">要求</span><span class="sxs-lookup"><span data-stu-id="78505-131">Request</span></span>
<span data-ttu-id="78505-132">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="78505-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="78505-133">プロトコル</span><span class="sxs-lookup"><span data-stu-id="78505-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_group_thread"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/threads/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q==
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="78505-134">C#</span><span class="sxs-lookup"><span data-stu-id="78505-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-group-thread-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="78505-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="78505-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-group-thread-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="78505-136">目的-C</span><span class="sxs-lookup"><span data-stu-id="78505-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-group-thread-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="78505-137">Java</span><span class="sxs-lookup"><span data-stu-id="78505-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-group-thread-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="78505-138">応答</span><span class="sxs-lookup"><span data-stu-id="78505-138">Response</span></span>
<span data-ttu-id="78505-139">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="78505-139">The following is an example of the response.</span></span> 
><span data-ttu-id="78505-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="78505-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Delete conversation thread",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
