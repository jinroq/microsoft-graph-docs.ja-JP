---
title: chatMessage を取得する
description: チャット内の 1 つのメッセージを取得します。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 63d98dafc73242e321da2fea58df08fc2f76ee7f
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36418153"
---
# <a name="get-chatmessage"></a><span data-ttu-id="a5ca7-103">chatMessage を取得する</span><span class="sxs-lookup"><span data-stu-id="a5ca7-103">Get chatMessage</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a5ca7-104">[チャット](../resources/chat.md)内の 1 つの[メッセージ](../resources/chatmessage.md)を取得します。</span><span class="sxs-lookup"><span data-stu-id="a5ca7-104">Retrieve a single [message](../resources/chatmessage.md) in a [chat](../resources/chat.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a5ca7-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a5ca7-105">Permissions</span></span>

<span data-ttu-id="a5ca7-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a5ca7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a5ca7-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a5ca7-108">Permission type</span></span>      | <span data-ttu-id="a5ca7-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a5ca7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a5ca7-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a5ca7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a5ca7-111">Chat.Read、Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a5ca7-111">Chat.Read, Chat.ReadWrite</span></span>   |
|<span data-ttu-id="a5ca7-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a5ca7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a5ca7-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a5ca7-113">Not supported.</span></span>    |
|<span data-ttu-id="a5ca7-114">Application</span><span class="sxs-lookup"><span data-stu-id="a5ca7-114">Application</span></span> | <span data-ttu-id="a5ca7-115">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="a5ca7-115">Chat.Read.All</span></span>   |

> [!NOTE]
> <span data-ttu-id="a5ca7-116">この API をアプリケーションのアクセス許可で呼び出す前に、アクセスを要求する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a5ca7-116">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="a5ca7-117">詳細については、「[Microsoft Teams の保護された API](/graph/teams-protected-apis)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a5ca7-117">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="a5ca7-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a5ca7-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/chats/{id}/messages/{id}
GET /users/{id}/chats/{id}/messages/{id}
GET /chats/{id}/messages/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a5ca7-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="a5ca7-119">Optional query parameters</span></span>

<span data-ttu-id="a5ca7-120">この操作は現在、応答をカスタマイズする[OData クエリ パラメーター](/graph/query-parameters)をサポートしていません。</span><span class="sxs-lookup"><span data-stu-id="a5ca7-120">This operation does not currently support [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a5ca7-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a5ca7-121">Request headers</span></span>
| <span data-ttu-id="a5ca7-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a5ca7-122">Header</span></span>       | <span data-ttu-id="a5ca7-123">値</span><span class="sxs-lookup"><span data-stu-id="a5ca7-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a5ca7-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="a5ca7-124">Authorization</span></span>  | <span data-ttu-id="a5ca7-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a5ca7-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a5ca7-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="a5ca7-127">Request body</span></span>
<span data-ttu-id="a5ca7-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="a5ca7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a5ca7-129">応答</span><span class="sxs-lookup"><span data-stu-id="a5ca7-129">Response</span></span>

<span data-ttu-id="a5ca7-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [chatmessage](../resources/chatmessage.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a5ca7-130">If successful, this method returns a `200 OK` response code and a [chatmessage](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a5ca7-131">例</span><span class="sxs-lookup"><span data-stu-id="a5ca7-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a5ca7-132">要求</span><span class="sxs-lookup"><span data-stu-id="a5ca7-132">Request</span></span>
<span data-ttu-id="a5ca7-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a5ca7-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a5ca7-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="a5ca7-134">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chat_message"
}-->
```http
GET https://graph.microsoft.com/beta/me/chats/{id}/messages/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a5ca7-135">C#</span><span class="sxs-lookup"><span data-stu-id="a5ca7-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chat-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a5ca7-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a5ca7-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chat-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a5ca7-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a5ca7-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chat-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a5ca7-138">応答</span><span class="sxs-lookup"><span data-stu-id="a5ca7-138">Response</span></span>
<span data-ttu-id="a5ca7-139">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="a5ca7-139">Here is an example of the response.</span></span> 

><span data-ttu-id="a5ca7-140">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="a5ca7-140">**Note:** The response object shown here is shortened for readability.</span></span> <span data-ttu-id="a5ca7-141">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="a5ca7-141">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('8b081ef6-4792-4def-b2c9-c363a1bf41d5')/chats('19%3A8b081ef6-4792-4def-b2c9-c363a1bf41d5_877192bd-9183-47d3-a74c-8aa0426716cf%40unq.gbl.spaces')/messages/$entity",
    "id": "1555631722147",
    "replyToId": null,
    "etag": "1555631722147",
    "messageType": "message",
    "createdDateTime": "2019-04-18T23:55:22.147Z",
    "lastModifiedDateTime": null,
    "deletedDateTime": null,
    "subject": null,
    "summary": null,
    "importance": "normal",
    "locale": "en-us",
    "policyViolation": null,
    "from": {
        "device": null,
        "user": null,
        "conversation": null,
        "application": {
            "id": "877192bd-9183-47d3-a74c-8aa0426716cf",
            "displayName": "TestBot",
            "applicationIdentityType": "bot"
        }
    },
    "body": {
        "contentType": "html",
        "content": "<attachment id=\"bcb243ec589a4537b3c650356421e696\"></attachment>"
    },
    "attachments": [
        {
            "id": "bcb243ec589a4537b3c650356421e696",
            "contentType": "application/vnd.microsoft.card.signin",
            "contentUrl": null,
            "content": "{\r\n  \"text\": \"Please sign in to sample to proceed.\",\r\n  \"buttons\": [\r\n    {\r\n      \"type\": \"signin\",\r\n      \"title\": \"Sign In\",\r\n      \"value\": \"https://token.botframework.com/api/oauth/signin?signin=921d46120f7695632ce6ca4b0da2e3ae15fea54c47\"\r\n    }\r\n  ]\r\n}",
            "name": null,
            "thumbnailUrl": null
        }
    ],
    "mentions": [],
    "reactions": []
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get chatMessage",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
