---
title: ChatMessage の作成
description: この API を使用して、新しい chatMessage を作成します。
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: b4f63409ad2036e91496da941462717e3760eacc
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36321705"
---
# <a name="create-chatmessage"></a><span data-ttu-id="e33f5-103">ChatMessage の作成</span><span class="sxs-lookup"><span data-stu-id="e33f5-103">Create chatMessage</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e33f5-104">指定した[チャット](../resources/chat.md)で新しい[メッセージ](../resources/chatmessage.md)を作成します。</span><span class="sxs-lookup"><span data-stu-id="e33f5-104">Create a new [message](../resources/chatmessage.md) in the specified [chat](../resources/chat.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e33f5-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e33f5-105">Permissions</span></span>

<span data-ttu-id="e33f5-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e33f5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e33f5-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e33f5-108">Permission type</span></span>                        | <span data-ttu-id="e33f5-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e33f5-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e33f5-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e33f5-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="e33f5-111">チャットの読み取り/書き込み</span><span class="sxs-lookup"><span data-stu-id="e33f5-111">Chat.ReadWrite</span></span> |
| <span data-ttu-id="e33f5-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e33f5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e33f5-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e33f5-113">Not supported.</span></span> |
| <span data-ttu-id="e33f5-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e33f5-114">Application</span></span>                            | <span data-ttu-id="e33f5-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e33f5-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e33f5-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e33f5-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /chats/{id}/messages
POST /users/{id}/chats/{id}/messages
```

## <a name="request-headers"></a><span data-ttu-id="e33f5-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e33f5-117">Request headers</span></span>

| <span data-ttu-id="e33f5-118">名前</span><span class="sxs-lookup"><span data-stu-id="e33f5-118">Name</span></span>          | <span data-ttu-id="e33f5-119">説明</span><span class="sxs-lookup"><span data-stu-id="e33f5-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="e33f5-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="e33f5-120">Authorization</span></span> | <span data-ttu-id="e33f5-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="e33f5-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="e33f5-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="e33f5-122">Request body</span></span>

<span data-ttu-id="e33f5-123">要求本文で、 [Chatmessage](../resources/chatmessage.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="e33f5-123">In the request body, supply a JSON representation of [chatMessage](../resources/chatmessage.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e33f5-124">応答</span><span class="sxs-lookup"><span data-stu-id="e33f5-124">Response</span></span>

<span data-ttu-id="e33f5-125">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で新しい[chatmessage](../resources/chatmessage.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e33f5-125">If successful, this method returns a `201 Created` response code and a new [chatMessage](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e33f5-126">例</span><span class="sxs-lookup"><span data-stu-id="e33f5-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e33f5-127">要求</span><span class="sxs-lookup"><span data-stu-id="e33f5-127">Request</span></span>

<span data-ttu-id="e33f5-128">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e33f5-128">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e33f5-129">プロトコル</span><span class="sxs-lookup"><span data-stu-id="e33f5-129">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_chatmessage_from_chat"
}-->

```http
POST https://graph.microsoft.com/beta/teams/{id}/channels/{id}/messages
Content-type: application/json

{
  "body": {
     "content" : "Hello world"
  }
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e33f5-130">C#</span><span class="sxs-lookup"><span data-stu-id="e33f5-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-chatmessage-from-chat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e33f5-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e33f5-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-chatmessage-from-chat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e33f5-132">目的-C</span><span class="sxs-lookup"><span data-stu-id="e33f5-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-chatmessage-from-chat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e33f5-133">Java</span><span class="sxs-lookup"><span data-stu-id="e33f5-133">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-chatmessage-from-chat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e33f5-134">応答</span><span class="sxs-lookup"><span data-stu-id="e33f5-134">Response</span></span>

<span data-ttu-id="e33f5-135">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e33f5-135">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="e33f5-136">ここに示す response オブジェクトは読みやすいように短縮される場合があります。</span><span class="sxs-lookup"><span data-stu-id="e33f5-136">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e33f5-137">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="e33f5-137">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "replyToId": "replyToId-value",
  "from": {
    "application": null,
    "device": null,
    "user": {
      "id": "87ea812c-8816-40e9-b770-5c165fa31397",
      "displayName": "Test User"
    }
  },
  "messageType": "message",
  "body": {
     "content": "Hello world",
     "contentType": "text"
  }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create chatMessage",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
