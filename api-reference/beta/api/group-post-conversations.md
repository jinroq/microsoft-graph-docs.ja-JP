---
title: 会話を作成する
description: 'スレッドと投稿を含めて、新しい会話を作成します。 '
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: 8fe80c3a7d226aaa2bfa3e4834623a84aa91a940
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870099"
---
# <a name="create-conversation"></a><span data-ttu-id="8bb52-103">会話を作成する</span><span class="sxs-lookup"><span data-stu-id="8bb52-103">Create conversation</span></span>

> <span data-ttu-id="8bb52-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8bb52-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8bb52-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8bb52-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8bb52-106">スレッドと投稿を含めて、新しい[会話](../resources/conversation.md)を作成します。</span><span class="sxs-lookup"><span data-stu-id="8bb52-106">Create a new [conversation](../resources/conversation.md) by including a thread and a post.</span></span> 

<span data-ttu-id="8bb52-107">[スレッドに返信](conversationthread-reply.md)または[投稿に返信](post-reply.md)を使い、その会話への投稿を続けます。</span><span class="sxs-lookup"><span data-stu-id="8bb52-107">Use [reply thread](conversationthread-reply.md) or [reply post](post-reply.md) to further post to that conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="8bb52-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8bb52-108">Permissions</span></span>
<span data-ttu-id="8bb52-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8bb52-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8bb52-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8bb52-111">Permission type</span></span>      | <span data-ttu-id="8bb52-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8bb52-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8bb52-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8bb52-113">Delegated (work or school account)</span></span> | <span data-ttu-id="8bb52-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8bb52-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="8bb52-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8bb52-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8bb52-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8bb52-116">Not supported.</span></span>    |
|<span data-ttu-id="8bb52-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8bb52-117">Application</span></span> | <span data-ttu-id="8bb52-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8bb52-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8bb52-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8bb52-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/conversations
```

## <a name="request-headers"></a><span data-ttu-id="8bb52-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8bb52-120">Request headers</span></span>
| <span data-ttu-id="8bb52-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8bb52-121">Header</span></span>       | <span data-ttu-id="8bb52-122">値</span><span class="sxs-lookup"><span data-stu-id="8bb52-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8bb52-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8bb52-123">Authorization</span></span>  | <span data-ttu-id="8bb52-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8bb52-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="8bb52-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8bb52-126">Content-Type</span></span>  | <span data-ttu-id="8bb52-127">application/json</span><span class="sxs-lookup"><span data-stu-id="8bb52-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8bb52-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="8bb52-128">Request body</span></span>
<span data-ttu-id="8bb52-129">要求の本文に、[conversationThread](../resources/conversationthread.md) と [投稿](../resources/post.md) を含む [会話](../resources/conversation.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="8bb52-129">In the request body, supply a JSON representation of [conversation](../resources/conversation.md) object containing a [conversationThread](../resources/conversationthread.md) and a [post](../resources/post.md).</span></span>

## <a name="response"></a><span data-ttu-id="8bb52-130">応答</span><span class="sxs-lookup"><span data-stu-id="8bb52-130">Response</span></span>
<span data-ttu-id="8bb52-131">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で[会話](../resources/conversation.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="8bb52-131">If successful, this method returns `201 Created` response code and [conversation](../resources/conversation.md) object in the response body.</span></span> 

<span data-ttu-id="8bb52-132">応答には、新しい会話とスレッドの ID が含まれます。これらの ID は、[投稿の一覧表示](conversationthread-list-posts.md)の操作時の新しい投稿の取得に使用することもできます。</span><span class="sxs-lookup"><span data-stu-id="8bb52-132">The response includes the IDs for the new conversation and thread, which you can use in the [list posts](conversationthread-list-posts.md) operation to get the new post as well.</span></span>

## <a name="example"></a><span data-ttu-id="8bb52-133">例</span><span class="sxs-lookup"><span data-stu-id="8bb52-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="8bb52-134">要求</span><span class="sxs-lookup"><span data-stu-id="8bb52-134">Request</span></span>
<span data-ttu-id="8bb52-135">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8bb52-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_conversation_from_group"
}-->
```http
POST https://graph.microsoft.com/beta/groups('29981b6a-0e57-42dc-94c9-cd24f5306196')/conversations
Content-type: application/json

{
    "topic":"New head count",
    "threads":[
        {
            "posts":[
                {
                    "body":{
                        "contentType":"html",
                        "content":"The confirmation will come by the end of the week."
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

#### <a name="response"></a><span data-ttu-id="8bb52-136">応答</span><span class="sxs-lookup"><span data-stu-id="8bb52-136">Response</span></span>
<span data-ttu-id="8bb52-137">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8bb52-137">The following is an example of the response.</span></span>
><span data-ttu-id="8bb52-138">**注:** ここに示す応答オブジェクトは、読みやすさの短縮される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="8bb52-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="8bb52-139">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="8bb52-139">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversation"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups('29981b6a-0e57-42dc-94c9-cd24f5306196')/conversations/$entity",
    "id":"AAQkADPxBgqECsrFDTuM=",
    "threads@odata.context":"https://graph.microsoft.com/beta/$metadata#groups('29981b6a-0e57-42dc-94c9-cd24f5306196')/conversations('AAQkADPxBgqECsrFDTuM%3D')/threads",
    "threads":[
        {
            "id":"AAQkADUNO4xAAMbGA93Sw-EGCoQKysUNO4w=="
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
  "tocPath": ""
}-->
