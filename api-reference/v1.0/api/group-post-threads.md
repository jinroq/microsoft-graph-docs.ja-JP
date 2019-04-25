---
title: 会話スレッドを作成する
description: '最初にスレッドを作成して、新しいグループ会話を開始します。 '
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 34a38c0700eeb9ab1074a2f7cb2b396168266c97
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32572907"
---
# <a name="create-conversation-thread"></a><span data-ttu-id="701f6-103">会話スレッドを作成する</span><span class="sxs-lookup"><span data-stu-id="701f6-103">Create conversation thread</span></span>
<span data-ttu-id="701f6-104">最初にスレッドを作成して、新しいグループ会話を開始します。</span><span class="sxs-lookup"><span data-stu-id="701f6-104">Start a new group conversation by first creating a thread.</span></span> 

<span data-ttu-id="701f6-p101">グループには、新しい会話、会話スレッド、および投稿が作成されます。[スレッドに返信](conversationthread-reply.md) または [投稿に返信](post-reply.md) を使い、そのスレッドへの投稿を続けます。</span><span class="sxs-lookup"><span data-stu-id="701f6-p101">A new conversation, conversation thread, and post are created in the group. Use [reply thread](conversationthread-reply.md) or [reply post](post-reply.md) to further post to that thread.</span></span>

<span data-ttu-id="701f6-107">注:[既存の会話内に新しいスレッドを開始する](conversation-post-threads.md) こともできます。</span><span class="sxs-lookup"><span data-stu-id="701f6-107">Note: You can also [start a new thread in an existing conversation](conversation-post-threads.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="701f6-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="701f6-108">Permissions</span></span>
<span data-ttu-id="701f6-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="701f6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="701f6-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="701f6-111">Permission type</span></span>      | <span data-ttu-id="701f6-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="701f6-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="701f6-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="701f6-113">Delegated (work or school account)</span></span> | <span data-ttu-id="701f6-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="701f6-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="701f6-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="701f6-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="701f6-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="701f6-116">Not supported.</span></span>    |
|<span data-ttu-id="701f6-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="701f6-117">Application</span></span> | <span data-ttu-id="701f6-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="701f6-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="701f6-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="701f6-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads
```
## <a name="request-headers"></a><span data-ttu-id="701f6-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="701f6-120">Request headers</span></span>
| <span data-ttu-id="701f6-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="701f6-121">Header</span></span>       | <span data-ttu-id="701f6-122">値</span><span class="sxs-lookup"><span data-stu-id="701f6-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="701f6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="701f6-123">Authorization</span></span>  | <span data-ttu-id="701f6-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="701f6-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="701f6-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="701f6-126">Content-Type</span></span>  | <span data-ttu-id="701f6-127">application/json</span><span class="sxs-lookup"><span data-stu-id="701f6-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="701f6-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="701f6-128">Request body</span></span>
<span data-ttu-id="701f6-129">要求の本文に、[投稿](../resources/post.md) を含む[conversationThread](../resources/conversationthread.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="701f6-129">In the request body, supply a JSON representation of [conversationThread](../resources/conversationthread.md) object containing a [post](../resources/post.md).</span></span>

## <a name="response"></a><span data-ttu-id="701f6-130">応答</span><span class="sxs-lookup"><span data-stu-id="701f6-130">Response</span></span>
<span data-ttu-id="701f6-131">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [conversationThread](../resources/conversationthread.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="701f6-131">If successful, this method returns `201 Created` response code and [conversationThread](../resources/conversationthread.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="701f6-132">例</span><span class="sxs-lookup"><span data-stu-id="701f6-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="701f6-133">要求</span><span class="sxs-lookup"><span data-stu-id="701f6-133">Request</span></span>
<span data-ttu-id="701f6-134">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="701f6-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_conversationthread_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/threads
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
#### <a name="response"></a><span data-ttu-id="701f6-135">応答</span><span class="sxs-lookup"><span data-stu-id="701f6-135">Response</span></span>
<span data-ttu-id="701f6-136">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="701f6-136">The following is an example of the response.</span></span>
><span data-ttu-id="701f6-137">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="701f6-137">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="701f6-138">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="701f6-138">All the properties will be returned from an actual call.</span></span>
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
  "lastDeliveredDateTime": "datetime-value",
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
