---
title: 会話スレッドを作成する
description: '最初にスレッドを作成して、新しいグループ会話を開始します。 '
ms.openlocfilehash: a18c64b976562a609501c6c50c809b4d11e26866
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072624"
---
# <a name="create-conversation-thread"></a><span data-ttu-id="8674c-103">会話スレッドを作成する</span><span class="sxs-lookup"><span data-stu-id="8674c-103">Create conversation thread</span></span>

> <span data-ttu-id="8674c-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8674c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8674c-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8674c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8674c-106">最初にスレッドを作成して、新しいグループ会話を開始します。</span><span class="sxs-lookup"><span data-stu-id="8674c-106">Start a new group conversation by first creating a thread.</span></span> 

<span data-ttu-id="8674c-p102">グループには、新しい会話、会話スレッド、および投稿が作成されます。[スレッドに返信](conversationthread-reply.md) または [投稿に返信](post-reply.md) を使い、そのスレッドへの投稿を続けます。</span><span class="sxs-lookup"><span data-stu-id="8674c-p102">A new conversation, conversation thread, and post are created in the group. Use [reply thread](conversationthread-reply.md) or [reply post](post-reply.md) to further post to that thread.</span></span>

<span data-ttu-id="8674c-109">注:[既存の会話内に新しいスレッドを開始する](conversation-post-threads.md) こともできます。</span><span class="sxs-lookup"><span data-stu-id="8674c-109">Note: You can also [start a new thread in an existing conversation](conversation-post-threads.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="8674c-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8674c-110">Permissions</span></span>
<span data-ttu-id="8674c-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8674c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8674c-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8674c-113">Permission type</span></span>      | <span data-ttu-id="8674c-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8674c-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8674c-115">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8674c-115">Delegated (work or school account)</span></span> | <span data-ttu-id="8674c-116">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8674c-116">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="8674c-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8674c-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8674c-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8674c-118">Not supported.</span></span>    |
|<span data-ttu-id="8674c-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8674c-119">Application</span></span> | <span data-ttu-id="8674c-120">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8674c-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8674c-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8674c-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads
```
## <a name="request-headers"></a><span data-ttu-id="8674c-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8674c-122">Request headers</span></span>
| <span data-ttu-id="8674c-123">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8674c-123">Header</span></span>       | <span data-ttu-id="8674c-124">値</span><span class="sxs-lookup"><span data-stu-id="8674c-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8674c-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="8674c-125">Authorization</span></span>  | <span data-ttu-id="8674c-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8674c-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="8674c-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8674c-128">Content-Type</span></span>  | <span data-ttu-id="8674c-129">application/json</span><span class="sxs-lookup"><span data-stu-id="8674c-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8674c-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="8674c-130">Request body</span></span>
<span data-ttu-id="8674c-131">要求の本文に、[投稿](../resources/post.md) を含む[conversationThread](../resources/conversationthread.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="8674c-131">In the request body, supply a JSON representation of [conversationThread](../resources/conversationthread.md) object containing a [post](../resources/post.md).</span></span>

## <a name="response"></a><span data-ttu-id="8674c-132">応答</span><span class="sxs-lookup"><span data-stu-id="8674c-132">Response</span></span>
<span data-ttu-id="8674c-133">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [conversationThread](../resources/conversationthread.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="8674c-133">If successful, this method returns `201 Created` response code and [conversationThread](../resources/conversationthread.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8674c-134">例</span><span class="sxs-lookup"><span data-stu-id="8674c-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="8674c-135">要求</span><span class="sxs-lookup"><span data-stu-id="8674c-135">Request</span></span>
<span data-ttu-id="8674c-136">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8674c-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_conversationthread_from_group"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/threads
Content-type: application/json

{
  "topic": "New Conversation Thread Topic",
  "posts": [{
    "body": {
      "contentType": "html",
      "content": "this is body content"
    },
    "newParticipants": [{
      "emailAddress": {
        "name": "Alex Darrow",
        "address": "alexd@contoso.com"
      }
    }]
  }]
}
```

#### <a name="response"></a><span data-ttu-id="8674c-137">応答</span><span class="sxs-lookup"><span data-stu-id="8674c-137">Response</span></span>
<span data-ttu-id="8674c-138">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8674c-138">The following is an example of the response.</span></span>
><span data-ttu-id="8674c-139">**注:** ここに示す応答オブジェクトは、読みやすさの短縮される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="8674c-139">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="8674c-140">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="8674c-140">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread"
} -->
```http
HTTP/1.1 201 OK
Content-type: application/json
Content-length: 419

{
  "toRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ],
  "topic": "topic-value",
  "hasAttachments": true,
  "lastDeliveredDateTime": "2016-10-19T10:37:00Z",
  "uniqueSenders": [
    "uniqueSenders-value"
  ],
  "ccRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create thread",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
