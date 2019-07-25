---
title: 会話を作成する
description: 'スレッドと投稿を含めて、新しい会話を作成します。 '
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 4fa3bb66978f049d490140c3a149eae63c8dc8bc
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35889591"
---
# <a name="create-conversation"></a><span data-ttu-id="c9b64-103">会話を作成する</span><span class="sxs-lookup"><span data-stu-id="c9b64-103">Create conversation</span></span>
<span data-ttu-id="c9b64-104">スレッドと投稿を含めて、新しい[会話](../resources/conversation.md)を作成します。</span><span class="sxs-lookup"><span data-stu-id="c9b64-104">Create a new [conversation](../resources/conversation.md) by including a thread and a post.</span></span> 

<span data-ttu-id="c9b64-105">[スレッドに返信](conversationthread-reply.md)または[投稿に返信](post-reply.md)を使い、その会話への投稿を続けます。</span><span class="sxs-lookup"><span data-stu-id="c9b64-105">Use [reply thread](conversationthread-reply.md) or [reply post](post-reply.md) to further post to that conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="c9b64-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c9b64-106">Permissions</span></span>
<span data-ttu-id="c9b64-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c9b64-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9b64-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c9b64-109">Permission type</span></span>      | <span data-ttu-id="c9b64-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c9b64-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c9b64-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c9b64-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c9b64-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9b64-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="c9b64-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c9b64-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c9b64-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c9b64-114">Not supported.</span></span>    |
|<span data-ttu-id="c9b64-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c9b64-115">Application</span></span> | <span data-ttu-id="c9b64-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c9b64-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c9b64-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c9b64-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/conversations
```

## <a name="request-headers"></a><span data-ttu-id="c9b64-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c9b64-118">Request headers</span></span>
| <span data-ttu-id="c9b64-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c9b64-119">Header</span></span>       | <span data-ttu-id="c9b64-120">値</span><span class="sxs-lookup"><span data-stu-id="c9b64-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c9b64-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c9b64-121">Authorization</span></span>  | <span data-ttu-id="c9b64-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c9b64-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c9b64-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c9b64-124">Content-Type</span></span>  | <span data-ttu-id="c9b64-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c9b64-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c9b64-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="c9b64-126">Request body</span></span>
<span data-ttu-id="c9b64-127">要求の本文に、[conversationThread](../resources/conversationthread.md) と [投稿](../resources/post.md) を含む [会話](../resources/conversation.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="c9b64-127">In the request body, supply a JSON representation of [conversation](../resources/conversation.md) object containing a [conversationThread](../resources/conversationthread.md) and a [post](../resources/post.md).</span></span>

## <a name="response"></a><span data-ttu-id="c9b64-128">応答</span><span class="sxs-lookup"><span data-stu-id="c9b64-128">Response</span></span>
<span data-ttu-id="c9b64-129">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で[会話](../resources/conversation.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c9b64-129">If successful, this method returns `201 Created` response code and [conversation](../resources/conversation.md) object in the response body.</span></span>

<span data-ttu-id="c9b64-130">応答には、新しい会話とスレッドの ID が含まれます。これらの ID は、[投稿の一覧表示](conversationthread-list-posts.md)の操作時の新しい投稿の取得に使用することもできます。</span><span class="sxs-lookup"><span data-stu-id="c9b64-130">The response includes the IDs for the new conversation and thread, which you can use in the [list posts](conversationthread-list-posts.md) operation to get the new post as well.</span></span>

## <a name="example"></a><span data-ttu-id="c9b64-131">例</span><span class="sxs-lookup"><span data-stu-id="c9b64-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="c9b64-132">要求</span><span class="sxs-lookup"><span data-stu-id="c9b64-132">Request</span></span>
<span data-ttu-id="c9b64-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c9b64-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c9b64-134">プロトコル</span><span class="sxs-lookup"><span data-stu-id="c9b64-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["29981b6a-0e57-42dc-94c9-cd24f5306196"],
  "name": "create_conversation_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/29981b6a-0e57-42dc-94c9-cd24f5306196/conversations
Content-type: application/json

{
    "topic":"New locations for this quarter",
    "threads":[
        {
            "posts":[
                {
                    "body":{
                        "contentType":"html",
                        "content":"What do we know so far?"
                    },
                    "newParticipants":[
                        {
                            "emailAddress":{
                                "name":"Adele Vance",
                                "address":"AdeleV@contoso.onmicrosoft.com"
                            }
                        }
                    ]
                }
            ]
        }
    ]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c9b64-135">C#</span><span class="sxs-lookup"><span data-stu-id="c9b64-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-conversation-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c9b64-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="c9b64-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-conversation-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c9b64-137">目的-C</span><span class="sxs-lookup"><span data-stu-id="c9b64-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-conversation-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c9b64-138">Java</span><span class="sxs-lookup"><span data-stu-id="c9b64-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-conversation-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c9b64-139">応答</span><span class="sxs-lookup"><span data-stu-id="c9b64-139">Response</span></span>
<span data-ttu-id="c9b64-140">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c9b64-140">The following is an example of the response.</span></span>
><span data-ttu-id="c9b64-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="c9b64-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversation"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups('29981b6a-0e57-42dc-94c9-cd24f5306196')/conversations/$entity",
    "id":"AAQkADDVKtMlRp4Txc6k=",
    "threads@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups('29981b6a-0e57-42dc-94c9-cd24f5306196')/conversations('AAQkADDVKtMlRp4Txc6k%3D')/threads",
    "threads":[
        {
            "id":"AAQkADQDarUNUq0yVGnhPFzqQ=="
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Conversation",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
