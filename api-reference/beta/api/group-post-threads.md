---
title: 会話スレッドを作成する
description: '最初にスレッドを作成して、新しいグループ会話を開始します。 '
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 3d52660f8395b63a9769447617adb119e180259a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36323193"
---
# <a name="create-conversation-thread"></a><span data-ttu-id="d7d18-103">会話スレッドを作成する</span><span class="sxs-lookup"><span data-stu-id="d7d18-103">Create conversation thread</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d7d18-104">最初にスレッドを作成して、新しいグループ会話を開始します。</span><span class="sxs-lookup"><span data-stu-id="d7d18-104">Start a new group conversation by first creating a thread.</span></span> 

<span data-ttu-id="d7d18-p101">グループには、新しい会話、会話スレッド、および投稿が作成されます。[スレッドに返信](conversationthread-reply.md) または [投稿に返信](post-reply.md) を使い、そのスレッドへの投稿を続けます。</span><span class="sxs-lookup"><span data-stu-id="d7d18-p101">A new conversation, conversation thread, and post are created in the group. Use [reply thread](conversationthread-reply.md) or [reply post](post-reply.md) to further post to that thread.</span></span>

<span data-ttu-id="d7d18-107">注:[既存の会話内に新しいスレッドを開始する](conversation-post-threads.md) こともできます。</span><span class="sxs-lookup"><span data-stu-id="d7d18-107">Note: You can also [start a new thread in an existing conversation](conversation-post-threads.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="d7d18-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d7d18-108">Permissions</span></span>
<span data-ttu-id="d7d18-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d7d18-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7d18-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d7d18-111">Permission type</span></span>      | <span data-ttu-id="d7d18-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d7d18-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d7d18-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d7d18-113">Delegated (work or school account)</span></span> | <span data-ttu-id="d7d18-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7d18-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d7d18-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d7d18-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d7d18-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d7d18-116">Not supported.</span></span>    |
|<span data-ttu-id="d7d18-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d7d18-117">Application</span></span> | <span data-ttu-id="d7d18-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d7d18-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d7d18-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d7d18-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads
```
## <a name="request-headers"></a><span data-ttu-id="d7d18-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d7d18-120">Request headers</span></span>
| <span data-ttu-id="d7d18-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d7d18-121">Header</span></span>       | <span data-ttu-id="d7d18-122">値</span><span class="sxs-lookup"><span data-stu-id="d7d18-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d7d18-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d7d18-123">Authorization</span></span>  | <span data-ttu-id="d7d18-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d7d18-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d7d18-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d7d18-126">Content-Type</span></span>  | <span data-ttu-id="d7d18-127">application/json</span><span class="sxs-lookup"><span data-stu-id="d7d18-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d7d18-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="d7d18-128">Request body</span></span>
<span data-ttu-id="d7d18-129">要求の本文に、[投稿](../resources/post.md) を含む[conversationThread](../resources/conversationthread.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="d7d18-129">In the request body, supply a JSON representation of [conversationThread](../resources/conversationthread.md) object containing a [post](../resources/post.md).</span></span>

## <a name="response"></a><span data-ttu-id="d7d18-130">応答</span><span class="sxs-lookup"><span data-stu-id="d7d18-130">Response</span></span>
<span data-ttu-id="d7d18-131">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [conversationThread](../resources/conversationthread.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d7d18-131">If successful, this method returns `201 Created` response code and [conversationThread](../resources/conversationthread.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d7d18-132">例</span><span class="sxs-lookup"><span data-stu-id="d7d18-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="d7d18-133">要求</span><span class="sxs-lookup"><span data-stu-id="d7d18-133">Request</span></span>
<span data-ttu-id="d7d18-134">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d7d18-134">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d7d18-135">プロトコル</span><span class="sxs-lookup"><span data-stu-id="d7d18-135">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="d7d18-136">C#</span><span class="sxs-lookup"><span data-stu-id="d7d18-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-conversationthread-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d7d18-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d7d18-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-conversationthread-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d7d18-138">目的-C</span><span class="sxs-lookup"><span data-stu-id="d7d18-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-conversationthread-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="d7d18-139">Java</span><span class="sxs-lookup"><span data-stu-id="d7d18-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-conversationthread-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d7d18-140">応答</span><span class="sxs-lookup"><span data-stu-id="d7d18-140">Response</span></span>
<span data-ttu-id="d7d18-141">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d7d18-141">The following is an example of the response.</span></span>
><span data-ttu-id="d7d18-142">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="d7d18-142">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d7d18-143">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="d7d18-143">All the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create thread",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
