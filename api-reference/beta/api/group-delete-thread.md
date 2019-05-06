---
title: 会話スレッドを削除する
description: thread オブジェクトを削除します。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 5a1c6501ec557744bfeb7a272c974b2cb2b3427e
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33593269"
---
# <a name="delete-conversation-thread"></a><span data-ttu-id="82b88-103">会話スレッドを削除する</span><span class="sxs-lookup"><span data-stu-id="82b88-103">Delete conversation thread</span></span>
<span data-ttu-id="82b88-104">[thread](../resources/conversationthread.md) オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="82b88-104">Delete a [thread](../resources/conversationthread.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="82b88-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="82b88-105">Permissions</span></span>
<span data-ttu-id="82b88-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="82b88-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82b88-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="82b88-108">Permission type</span></span>      | <span data-ttu-id="82b88-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="82b88-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="82b88-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="82b88-110">Delegated (work or school account)</span></span> | <span data-ttu-id="82b88-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82b88-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="82b88-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="82b88-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="82b88-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="82b88-113">Not supported.</span></span>    |
|<span data-ttu-id="82b88-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="82b88-114">Application</span></span> | <span data-ttu-id="82b88-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="82b88-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="82b88-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="82b88-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/threads/{id}
```

## <a name="request-headers"></a><span data-ttu-id="82b88-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="82b88-117">Request headers</span></span>
| <span data-ttu-id="82b88-118">名前</span><span class="sxs-lookup"><span data-stu-id="82b88-118">Name</span></span>       | <span data-ttu-id="82b88-119">型</span><span class="sxs-lookup"><span data-stu-id="82b88-119">Type</span></span> | <span data-ttu-id="82b88-120">説明</span><span class="sxs-lookup"><span data-stu-id="82b88-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="82b88-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="82b88-121">Authorization</span></span>  | <span data-ttu-id="82b88-122">string</span><span class="sxs-lookup"><span data-stu-id="82b88-122">string</span></span>  | <span data-ttu-id="82b88-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="82b88-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="82b88-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="82b88-125">Request body</span></span>
<span data-ttu-id="82b88-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="82b88-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="82b88-127">応答</span><span class="sxs-lookup"><span data-stu-id="82b88-127">Response</span></span>
<span data-ttu-id="82b88-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="82b88-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="82b88-130">例</span><span class="sxs-lookup"><span data-stu-id="82b88-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="82b88-131">要求</span><span class="sxs-lookup"><span data-stu-id="82b88-131">Request</span></span>
<span data-ttu-id="82b88-132">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="82b88-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["02bd9fd6-8f93-4758-87c3-1fb73740a315", "AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q=="],
  "name": "delete_group_thread"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/threads/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q==
```

#### <a name="response"></a><span data-ttu-id="82b88-133">応答</span><span class="sxs-lookup"><span data-stu-id="82b88-133">Response</span></span>
<span data-ttu-id="82b88-134">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="82b88-134">The following is an example of the response.</span></span> 
><span data-ttu-id="82b88-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="82b88-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="82b88-137">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="82b88-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="82b88-138">Visual</span><span class="sxs-lookup"><span data-stu-id="82b88-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_group_thread-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="82b88-139">Java</span><span class="sxs-lookup"><span data-stu-id="82b88-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_group_thread-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete conversation thread",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/group-delete-thread.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-delete-thread.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
