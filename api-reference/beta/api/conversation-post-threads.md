---
title: スレッドを作成する
description: 指定した会話に新しいスレッドを作成します。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 7915637c4e19c56abbd076f5041500348b58b5d7
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35261139"
---
# <a name="create-thread"></a><span data-ttu-id="d5614-103">スレッドを作成する</span><span class="sxs-lookup"><span data-stu-id="d5614-103">Create thread</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d5614-104">指定した会話に新しいスレッドを作成します。</span><span class="sxs-lookup"><span data-stu-id="d5614-104">Create a new thread in the specified conversation.</span></span>

<span data-ttu-id="d5614-p101">指定したとおりにスレッドと投稿を作成します。[スレッドに返信](conversationthread-reply.md) を使用して、そのスレッドへの投稿を続けます。また、投稿 ID を取得している場合は、そのスレッドのその投稿にも[返信](post-reply.md)できます。</span><span class="sxs-lookup"><span data-stu-id="d5614-p101">A thread and post are created as specified. Use [reply thread](conversationthread-reply.md) to further post to that thread. Or, if you get the post ID, you can also [reply](post-reply.md) to that post in that thread.</span></span>

<span data-ttu-id="d5614-108">注:[最初にスレッドを作成して、新しい会話を開始](group-post-threads.md)することもできます。</span><span class="sxs-lookup"><span data-stu-id="d5614-108">Note: You can also [start a new conversation by first creating a thread](group-post-threads.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d5614-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d5614-109">Permissions</span></span>
<span data-ttu-id="d5614-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d5614-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5614-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d5614-112">Permission type</span></span>      | <span data-ttu-id="d5614-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d5614-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d5614-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d5614-114">Delegated (work or school account)</span></span> | <span data-ttu-id="d5614-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5614-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d5614-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d5614-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d5614-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d5614-117">Not supported.</span></span>    |
|<span data-ttu-id="d5614-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d5614-118">Application</span></span> | <span data-ttu-id="d5614-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d5614-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d5614-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d5614-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/conversations/{id}/threads
```
## <a name="request-headers"></a><span data-ttu-id="d5614-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d5614-121">Request headers</span></span>
| <span data-ttu-id="d5614-122">名前</span><span class="sxs-lookup"><span data-stu-id="d5614-122">Name</span></span>       | <span data-ttu-id="d5614-123">型</span><span class="sxs-lookup"><span data-stu-id="d5614-123">Type</span></span> | <span data-ttu-id="d5614-124">説明</span><span class="sxs-lookup"><span data-stu-id="d5614-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d5614-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="d5614-125">Authorization</span></span>  | <span data-ttu-id="d5614-126">string</span><span class="sxs-lookup"><span data-stu-id="d5614-126">string</span></span>  | <span data-ttu-id="d5614-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d5614-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d5614-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="d5614-129">Request body</span></span>
<span data-ttu-id="d5614-130">要求の本文に、[ConversationThread](../resources/conversationthread.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="d5614-130">In the request body, supply a JSON representation of [ConversationThread](../resources/conversationthread.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="d5614-131">応答</span><span class="sxs-lookup"><span data-stu-id="d5614-131">Response</span></span>

<span data-ttu-id="d5614-132">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [conversationThread](../resources/conversationthread.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d5614-132">If successful, this method returns `201 Created` response code and [ConversationThread](../resources/conversationthread.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d5614-133">例</span><span class="sxs-lookup"><span data-stu-id="d5614-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d5614-134">要求</span><span class="sxs-lookup"><span data-stu-id="d5614-134">Request</span></span>
<span data-ttu-id="d5614-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d5614-135">Here is an example of the request.</span></span>
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
<span data-ttu-id="d5614-136">要求の本文に、[conversationThread](../resources/conversationthread.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="d5614-136">In the request body, supply a JSON representation of [conversationThread](../resources/conversationthread.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="d5614-137">応答</span><span class="sxs-lookup"><span data-stu-id="d5614-137">Response</span></span>

<span data-ttu-id="d5614-p104">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で新しいスレッドの `id` を返します。以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="d5614-p104">If successful, this method returns `201 Created` response code and the `id` of the new thread in the response body. Here is an example of the response.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="d5614-140">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="d5614-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d5614-141">C#</span><span class="sxs-lookup"><span data-stu-id="d5614-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_conversationthread_from_conversation-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d5614-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="d5614-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_conversationthread_from_conversation-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="d5614-143">目的-C</span><span class="sxs-lookup"><span data-stu-id="d5614-143">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_conversationthread_from_conversation-Objective-C-snippets.md)]
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
    "Error: /api-reference/beta/api/conversation-post-threads.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/conversation-post-threads.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/conversation-post-threads.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
