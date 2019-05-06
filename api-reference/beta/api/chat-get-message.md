---
title: チャット メッセージの取得
description: チャット内の 1 つのメッセージを取得します。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 02c31f7df35821e7706cabe3852ae5f441edf15a
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33327653"
---
# <a name="get-chat-message"></a><span data-ttu-id="32bab-103">チャット メッセージの取得</span><span class="sxs-lookup"><span data-stu-id="32bab-103">Get chat message</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="32bab-104">[チャット](../resources/chat.md)内の 1 つの[メッセージ](../resources/chatmessage.md)を取得します。</span><span class="sxs-lookup"><span data-stu-id="32bab-104">Retrieve a single [message](../resources/chatmessage.md) in a [chat](../resources/chat.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="32bab-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="32bab-105">Permissions</span></span>

<span data-ttu-id="32bab-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="32bab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="32bab-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="32bab-108">Permission type</span></span>      | <span data-ttu-id="32bab-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="32bab-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="32bab-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="32bab-110">Delegated (work or school account)</span></span> | <span data-ttu-id="32bab-111">Chat.Read</span><span class="sxs-lookup"><span data-stu-id="32bab-111">Chat.Read</span></span>   |
|<span data-ttu-id="32bab-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="32bab-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="32bab-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="32bab-113">Not supported.</span></span>    |
|<span data-ttu-id="32bab-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="32bab-114">Application</span></span> | <span data-ttu-id="32bab-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="32bab-115">Not supported.</span></span>   |

## <a name="http-request"></a><span data-ttu-id="32bab-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="32bab-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/chats/{id}/messages/{id}
GET /users/{id}/chats/{id}/messages/{id}
GET /chats/{id}/messages/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="32bab-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="32bab-117">Optional query parameters</span></span>

<span data-ttu-id="32bab-118">この操作は現在、応答をカスタマイズする[OData クエリ パラメーター](/graph/query-parameters)をサポートしていません。</span><span class="sxs-lookup"><span data-stu-id="32bab-118">This operation does not currently support [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="32bab-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="32bab-119">Request headers</span></span>
| <span data-ttu-id="32bab-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="32bab-120">Header</span></span>       | <span data-ttu-id="32bab-121">値</span><span class="sxs-lookup"><span data-stu-id="32bab-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="32bab-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="32bab-122">Authorization</span></span>  | <span data-ttu-id="32bab-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="32bab-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="32bab-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="32bab-125">Request body</span></span>
<span data-ttu-id="32bab-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="32bab-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="32bab-127">応答</span><span class="sxs-lookup"><span data-stu-id="32bab-127">Response</span></span>

<span data-ttu-id="32bab-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [chatmessage](../resources/chatmessage.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="32bab-128">If successful, this method returns a `200 OK` response code and a [team](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="32bab-129">例</span><span class="sxs-lookup"><span data-stu-id="32bab-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="32bab-130">要求</span><span class="sxs-lookup"><span data-stu-id="32bab-130">Request</span></span>
<span data-ttu-id="32bab-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="32bab-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_chat_message"
}-->
```http
GET https://graph.microsoft.com/beta/me/chats/{id}/messages/{id}
```

##### <a name="response"></a><span data-ttu-id="32bab-132">応答</span><span class="sxs-lookup"><span data-stu-id="32bab-132">Response</span></span>
<span data-ttu-id="32bab-133">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="32bab-133">Here is an example of the response.</span></span> 

><span data-ttu-id="32bab-134">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="32bab-134">**Note:** The response object shown here are shortened for readability.</span></span> <span data-ttu-id="32bab-135">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="32bab-135">All the properties will be returned from an actual call.</span></span>
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
  "description": "Get chat message",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
