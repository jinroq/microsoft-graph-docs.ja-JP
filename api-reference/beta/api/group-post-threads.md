---
title: 会話スレッドを作成する
description: '最初にスレッドを作成して、新しいグループ会話を開始します。 '
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 3d87c07325dc5f191b45db96fc95521fdd85d430
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35262903"
---
# <a name="create-conversation-thread"></a><span data-ttu-id="c7600-103">会話スレッドを作成する</span><span class="sxs-lookup"><span data-stu-id="c7600-103">Create conversation thread</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c7600-104">最初にスレッドを作成して、新しいグループ会話を開始します。</span><span class="sxs-lookup"><span data-stu-id="c7600-104">Start a new group conversation by first creating a thread.</span></span> 

<span data-ttu-id="c7600-p101">グループには、新しい会話、会話スレッド、および投稿が作成されます。[スレッドに返信](conversationthread-reply.md) または [投稿に返信](post-reply.md) を使い、そのスレッドへの投稿を続けます。</span><span class="sxs-lookup"><span data-stu-id="c7600-p101">A new conversation, conversation thread, and post are created in the group. Use [reply thread](conversationthread-reply.md) or [reply post](post-reply.md) to further post to that thread.</span></span>

<span data-ttu-id="c7600-107">注:[既存の会話内に新しいスレッドを開始する](conversation-post-threads.md) こともできます。</span><span class="sxs-lookup"><span data-stu-id="c7600-107">Note: You can also [start a new thread in an existing conversation](conversation-post-threads.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="c7600-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c7600-108">Permissions</span></span>
<span data-ttu-id="c7600-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c7600-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7600-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c7600-111">Permission type</span></span>      | <span data-ttu-id="c7600-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c7600-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c7600-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c7600-113">Delegated (work or school account)</span></span> | <span data-ttu-id="c7600-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7600-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="c7600-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c7600-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c7600-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c7600-116">Not supported.</span></span>    |
|<span data-ttu-id="c7600-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c7600-117">Application</span></span> | <span data-ttu-id="c7600-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c7600-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c7600-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c7600-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads
```
## <a name="request-headers"></a><span data-ttu-id="c7600-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c7600-120">Request headers</span></span>
| <span data-ttu-id="c7600-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c7600-121">Header</span></span>       | <span data-ttu-id="c7600-122">値</span><span class="sxs-lookup"><span data-stu-id="c7600-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c7600-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c7600-123">Authorization</span></span>  | <span data-ttu-id="c7600-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c7600-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c7600-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c7600-126">Content-Type</span></span>  | <span data-ttu-id="c7600-127">application/json</span><span class="sxs-lookup"><span data-stu-id="c7600-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c7600-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="c7600-128">Request body</span></span>
<span data-ttu-id="c7600-129">要求の本文に、[投稿](../resources/post.md) を含む[conversationThread](../resources/conversationthread.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="c7600-129">In the request body, supply a JSON representation of [conversationThread](../resources/conversationthread.md) object containing a [post](../resources/post.md).</span></span>

## <a name="response"></a><span data-ttu-id="c7600-130">応答</span><span class="sxs-lookup"><span data-stu-id="c7600-130">Response</span></span>
<span data-ttu-id="c7600-131">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [conversationThread](../resources/conversationthread.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c7600-131">If successful, this method returns `201 Created` response code and [conversationThread](../resources/conversationthread.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c7600-132">例</span><span class="sxs-lookup"><span data-stu-id="c7600-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="c7600-133">要求</span><span class="sxs-lookup"><span data-stu-id="c7600-133">Request</span></span>
<span data-ttu-id="c7600-134">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c7600-134">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="c7600-135">応答</span><span class="sxs-lookup"><span data-stu-id="c7600-135">Response</span></span>
<span data-ttu-id="c7600-136">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c7600-136">The following is an example of the response.</span></span>
><span data-ttu-id="c7600-137">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="c7600-137">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c7600-138">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="c7600-138">All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="c7600-139">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="c7600-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c7600-140">C#</span><span class="sxs-lookup"><span data-stu-id="c7600-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_conversationthread_from_group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c7600-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="c7600-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_conversationthread_from_group-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="c7600-142">目的-C</span><span class="sxs-lookup"><span data-stu-id="c7600-142">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_conversationthread_from_group-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create thread",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-post-threads.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/group-post-threads.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/group-post-threads.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
