---
title: スレッドを作成する
description: 指定した会話に新しいスレッドを作成します。
author: dkershaw10
ms.openlocfilehash: 5fafbcae4a7dcf451d8bb707dd19456cc9da3f90
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27313847"
---
# <a name="create-thread"></a><span data-ttu-id="00cf0-103">スレッドを作成する</span><span class="sxs-lookup"><span data-stu-id="00cf0-103">Create thread</span></span>

> <span data-ttu-id="00cf0-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="00cf0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="00cf0-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="00cf0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="00cf0-106">指定した会話に新しいスレッドを作成します。</span><span class="sxs-lookup"><span data-stu-id="00cf0-106">Create a new thread in the specified conversation.</span></span>

<span data-ttu-id="00cf0-p102">指定したとおりにスレッドと投稿を作成します。[スレッドに返信](conversationthread-reply.md) を使用して、そのスレッドへの投稿を続けます。また、投稿 ID を取得している場合は、そのスレッドのその投稿にも[返信](post-reply.md)できます。</span><span class="sxs-lookup"><span data-stu-id="00cf0-p102">A thread and post are created as specified. Use [reply thread](conversationthread-reply.md) to further post to that thread. Or, if you get the post ID, you can also [reply](post-reply.md) to that post in that thread.</span></span>

<span data-ttu-id="00cf0-110">注:[最初にスレッドを作成して、新しい会話を開始](group-post-threads.md)することもできます。</span><span class="sxs-lookup"><span data-stu-id="00cf0-110">Note: You can also [start a new conversation by first creating a thread](group-post-threads.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="00cf0-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="00cf0-111">Permissions</span></span>
<span data-ttu-id="00cf0-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="00cf0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="00cf0-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="00cf0-114">Permission type</span></span>      | <span data-ttu-id="00cf0-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="00cf0-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="00cf0-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="00cf0-116">Delegated (work or school account)</span></span> | <span data-ttu-id="00cf0-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00cf0-117">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="00cf0-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="00cf0-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="00cf0-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="00cf0-119">Not supported.</span></span>    |
|<span data-ttu-id="00cf0-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="00cf0-120">Application</span></span> | <span data-ttu-id="00cf0-121">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00cf0-121">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="00cf0-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="00cf0-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/conversations/{id}/threads
```
## <a name="request-headers"></a><span data-ttu-id="00cf0-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="00cf0-123">Request headers</span></span>
| <span data-ttu-id="00cf0-124">名前</span><span class="sxs-lookup"><span data-stu-id="00cf0-124">Name</span></span>       | <span data-ttu-id="00cf0-125">種類</span><span class="sxs-lookup"><span data-stu-id="00cf0-125">Type</span></span> | <span data-ttu-id="00cf0-126">説明</span><span class="sxs-lookup"><span data-stu-id="00cf0-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="00cf0-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="00cf0-127">Authorization</span></span>  | <span data-ttu-id="00cf0-128">string</span><span class="sxs-lookup"><span data-stu-id="00cf0-128">string</span></span>  | <span data-ttu-id="00cf0-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="00cf0-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="00cf0-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="00cf0-131">Request body</span></span>
<span data-ttu-id="00cf0-132">要求の本文に、[ConversationThread](../resources/conversationthread.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="00cf0-132">In the request body, supply a JSON representation of [ConversationThread](../resources/conversationthread.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="00cf0-133">応答</span><span class="sxs-lookup"><span data-stu-id="00cf0-133">Response</span></span>

<span data-ttu-id="00cf0-134">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [conversationThread](../resources/conversationthread.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="00cf0-134">If successful, this method returns `201 Created` response code and [ConversationThread](../resources/conversationthread.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="00cf0-135">例</span><span class="sxs-lookup"><span data-stu-id="00cf0-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="00cf0-136">要求</span><span class="sxs-lookup"><span data-stu-id="00cf0-136">Request</span></span>
<span data-ttu-id="00cf0-137">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="00cf0-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_conversationthread_from_conversation"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/conversations/{id}/threads
Content-type: application/json

{
  "topic": "topic-value",
  "posts": [{
      "body": {
        "contentType": "html",
        "content": "this is body content"
      }
  }]
}
```
<span data-ttu-id="00cf0-138">要求の本文に、[conversationThread](../resources/conversationthread.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="00cf0-138">In the request body, supply a JSON representation of [conversationThread](../resources/conversationthread.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="00cf0-139">応答</span><span class="sxs-lookup"><span data-stu-id="00cf0-139">Response</span></span>

<span data-ttu-id="00cf0-p105">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で新しいスレッドの `id` を返します。以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="00cf0-p105">If successful, this method returns `201 Created` response code and the `id` of the new thread in the response body. Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 346

{
  "id": "thread-id-value"
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
