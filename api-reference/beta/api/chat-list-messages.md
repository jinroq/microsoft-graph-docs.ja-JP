---
title: チャット メッセージの一覧表示
description: 'チャット内のメッセージのリストを取得します。 '
localization_priority: Priority
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 24f00282f7dcb9cb5a76272c4c58108263809964
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33327643"
---
# <a name="list-chat-messages"></a><span data-ttu-id="da1b9-103">チャット メッセージの一覧表示</span><span class="sxs-lookup"><span data-stu-id="da1b9-103">List chat messages</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="da1b9-104">[チャット](../resources/chat.md)内の[メッセージ](../resources/chatmessage.md)のリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="da1b9-104">Retrieve the list of [messages](../resources/chatmessage.md) in a [chat](../resources/chat.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="da1b9-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="da1b9-105">Permissions</span></span>

<span data-ttu-id="da1b9-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="da1b9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da1b9-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="da1b9-108">Permission type</span></span>      | <span data-ttu-id="da1b9-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="da1b9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="da1b9-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="da1b9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="da1b9-111">Chat.Read</span><span class="sxs-lookup"><span data-stu-id="da1b9-111">Chat.Read</span></span>   |
|<span data-ttu-id="da1b9-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="da1b9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="da1b9-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="da1b9-113">Not supported.</span></span>    |
|<span data-ttu-id="da1b9-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="da1b9-114">Application</span></span> | <span data-ttu-id="da1b9-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="da1b9-115">Not supported.</span></span>   |

## <a name="http-request"></a><span data-ttu-id="da1b9-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="da1b9-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/chats/{id}/messages
GET /users/{id}/chats/{id}/messages
GET /chats/{id}/messages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="da1b9-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="da1b9-117">Optional query parameters</span></span>

<span data-ttu-id="da1b9-118">この操作は現在、応答をカスタマイズする[OData クエリ パラメーター](/graph/query-parameters)をサポートしていません。</span><span class="sxs-lookup"><span data-stu-id="da1b9-118">This operation does not currently support [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="da1b9-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="da1b9-119">Request headers</span></span>

| <span data-ttu-id="da1b9-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="da1b9-120">Header</span></span>       | <span data-ttu-id="da1b9-121">値</span><span class="sxs-lookup"><span data-stu-id="da1b9-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="da1b9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="da1b9-122">Authorization</span></span>  | <span data-ttu-id="da1b9-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="da1b9-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="da1b9-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="da1b9-125">Request body</span></span>

<span data-ttu-id="da1b9-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="da1b9-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="da1b9-127">応答</span><span class="sxs-lookup"><span data-stu-id="da1b9-127">Response</span></span>

<span data-ttu-id="da1b9-128">このメソッドは、成功すると `200 OK` 応答コードと [chatMessage](../resources/chatmessage.md) オブジェクトのコレクションを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="da1b9-128">If successful, this method returns a `200 OK` response code and a collection of [chatmessage](../resources/chatmessage.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="da1b9-129">例</span><span class="sxs-lookup"><span data-stu-id="da1b9-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="da1b9-130">要求</span><span class="sxs-lookup"><span data-stu-id="da1b9-130">Request</span></span>

<span data-ttu-id="da1b9-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="da1b9-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_chat_messages"
}-->
```http
GET https://graph.microsoft.com/beta/chats/{id}/messages
```
##### <a name="response"></a><span data-ttu-id="da1b9-132">応答</span><span class="sxs-lookup"><span data-stu-id="da1b9-132">Response</span></span>
<span data-ttu-id="da1b9-133">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="da1b9-133">Here is an example of the response.</span></span> 

><span data-ttu-id="da1b9-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="da1b9-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('8b081ef6-4792-4def-b2c9-c363a1bf41d5')/chats('19%3A8b081ef6-4792-4def-b2c9-c363a1bf41d5_877192bd-9183-47d3-a74c-8aa0426716cf%40unq.gbl.spaces')/messages",
    "@odata.count": 4,
    "@odata.nextLink": "https://graph.microsoft.com/beta/me/chats/19:8b081ef6-4792-4def-b2c9-c363a1bf41d5_877192bd-9183-47d3-a74c-8aa0426716cf@unq.gbl.spaces/messages?$skiptoken=M2Y1YjAwMDAwMDMxMzkzYTM4NjIzMDM4MzE2NTY2MzYyZDM0MzczOTMyMmQzNDY0NjU2NjJkNjIzMjYzMzkyZDYzMzMzNjMzNjEzMTYyNjYzNDMxNjQzNTVmMzgzNzM3MzEzOTMyNjI2NDJkMzkzMTM4MzMyZDM0Mzc2NDMzMmQ2MTM3MzQ2MzJkMzg2MTYxMzAzNDMyMzYzNzMxMzY2MzY2NDA3NTZlNzEyZTY3NjI2YzJlNzM3MDYxNjM2NTczMDE5N2Y3ZGMzMjZhMDEwMDAwMDg1YjNmNGI2YTAxMDAwMDAwfDE1NTU2MzE3MjIxNDc%3d",
    "value": [
        {
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
                "content": "<attachment id=\"a7bda643d32b4541b74ec1f4ace7f391\"></attachment>"
            },
            "attachments": [
                {
                    "id": "a7bda643d32b4541b74ec1f4ace7f391",
                    "contentType": "application/vnd.microsoft.card.signin",
                    "contentUrl": null,
                    "content": "{\r\n  \"text\": \"Please sign in to sample to proceed.\",\r\n  \"buttons\": [\r\n    {\r\n      \"type\": \"signin\",\r\n      \"title\": \"Sign In\",\r\n      \"value\": \"https://token.botframework.com/api/oauth/signin?signin=921d46120f7695632ce6ca4b0da2e3ae15fea54c47\"\r\n    }\r\n  ]\r\n}",
                    "name": null,
                    "thumbnailUrl": null
                }
            ],
            "mentions": [],
            "reactions": []
        },
        {
            "id": "1555631540287",
            "replyToId": null,
            "etag": "1555631540287",
            "messageType": "message",
            "createdDateTime": "2019-04-18T23:52:20.287Z",
            "lastModifiedDateTime": null,
            "deletedDateTime": null,
            "subject": "",
            "summary": null,
            "importance": "normal",
            "locale": "en-us",
            "policyViolation": null,
            "from": {
                "application": null,
                "device": null,
                "conversation": null,
                "user": {
                    "id": "8b081ef6-4792-4def-b2c9-c363a1bf41d5",
                    "displayName": "MOD Administrator",
                    "userIdentityType": "aadUser"
                }
            },
            "body": {
                "contentType": "text",
                "content": "yo"
            },
            "attachments": [],
            "mentions": [],
            "reactions": []
        },
        {
            "id": "1555631512068",
            "replyToId": null,
            "etag": "1555631512068",
            "messageType": "message",
            "createdDateTime": "2019-04-18T23:51:52.068Z",
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
                "content": "<attachment id=\"6309ad5424a04c5899efd130342b165a\"></attachment>"
            },
            "attachments": [
                {
                    "id": "6309ad5424a04c5899efd130342b165a",
                    "contentType": "application/vnd.microsoft.card.signin",
                    "contentUrl": null,
                    "content": "{\r\n  \"text\": \"Please sign in to sample to proceed.\",\r\n  \"buttons\": [\r\n    {\r\n      \"type\": \"signin\",\r\n      \"title\": \"Sign In\",\r\n      \"value\": \"https://token.botframework.com/api/oauth/signin?signin=921d46120f978574f2993640bf9cbc5e438824a645\"\r\n    }\r\n  ]\r\n}",
                    "name": null,
                    "thumbnailUrl": null
                }
            ],
            "mentions": [],
            "reactions": []
        },
        {
            "id": "1555631511115",
            "replyToId": null,
            "etag": "1555631511115",
            "messageType": "message",
            "createdDateTime": "2019-04-18T23:51:51.115Z",
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
                "content": "<attachment id=\"9b6e6d3bde7741bcac561bb15ec2721b\"></attachment>"
            },
            "attachments": [
                {
                    "id": "9b6e6d3bde7741bcac561bb15ec2721b",
                    "contentType": "application/vnd.microsoft.card.signin",
                    "contentUrl": null,
                    "content": "{\r\n  \"text\": \"Please sign in to sample to proceed.\",\r\n  \"buttons\": [\r\n    {\r\n      \"type\": \"signin\",\r\n      \"title\": \"Sign In\",\r\n      \"value\": \"https://token.botframework.com/api/oauth/signin?signin=921d46120f01039912d88040739e2780ef54656557\"\r\n    }\r\n  ]\r\n}",
                    "name": null,
                    "thumbnailUrl": null
                }
            ],
            "mentions": [],
            "reactions": []
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get chat messages",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->