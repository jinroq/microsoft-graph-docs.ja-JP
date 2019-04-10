---
title: チャネル内でメッセージを送信する
description: 指定したチャネルで新しいメッセージを送信します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 56834a628465fc5721e0dc7ef7eb5e05065dccbc
ms.sourcegitcommit: bf3d0c94faeb206f9f986423a436fb355acd54c1
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/10/2019
ms.locfileid: "31751551"
---
# <a name="send-a-message-to-a-channel"></a><span data-ttu-id="96bf6-103">メッセージをチャネルに送信する</span><span class="sxs-lookup"><span data-stu-id="96bf6-103">Send a message to a channel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="96bf6-104">指定した[チャネル](../resources/channel.md)で新しい[メッセージ](../resources/chatmessage.md)を作成します。</span><span class="sxs-lookup"><span data-stu-id="96bf6-104">Create a new [message](../resources/chatmessage.md) in the specified [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="96bf6-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="96bf6-105">Permissions</span></span>
<span data-ttu-id="96bf6-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="96bf6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96bf6-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="96bf6-108">Permission type</span></span>      | <span data-ttu-id="96bf6-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="96bf6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="96bf6-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="96bf6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="96bf6-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96bf6-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="96bf6-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="96bf6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="96bf6-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="96bf6-113">Not supported.</span></span>    |
|<span data-ttu-id="96bf6-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="96bf6-114">Application</span></span> | <span data-ttu-id="96bf6-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="96bf6-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="96bf6-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="96bf6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels/{id}/messages
```

## <a name="request-headers"></a><span data-ttu-id="96bf6-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="96bf6-117">Request headers</span></span>
| <span data-ttu-id="96bf6-118">名前</span><span class="sxs-lookup"><span data-stu-id="96bf6-118">Name</span></span>       | <span data-ttu-id="96bf6-119">型</span><span class="sxs-lookup"><span data-stu-id="96bf6-119">Type</span></span> | <span data-ttu-id="96bf6-120">説明</span><span class="sxs-lookup"><span data-stu-id="96bf6-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="96bf6-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="96bf6-121">Authorization</span></span>  | <span data-ttu-id="96bf6-122">string</span><span class="sxs-lookup"><span data-stu-id="96bf6-122">string</span></span>  | <span data-ttu-id="96bf6-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="96bf6-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="96bf6-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="96bf6-125">Request body</span></span>
<span data-ttu-id="96bf6-126">要求本文で、[メッセージ](../resources/chatmessage.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="96bf6-126">In the request body, supply a JSON representation of a [message](../resources/chatmessage.md) object.</span></span> <span data-ttu-id="96bf6-127">body プロパティのみが必須で、その他のプロパティはオプションです。</span><span class="sxs-lookup"><span data-stu-id="96bf6-127">Only the body property is mandatory, other properties are optional.</span></span>

> <span data-ttu-id="96bf6-128">注: 添付ファイルと画像を使用したメッセージの送信はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="96bf6-128">Note: Sending messages with attachments and images is not supported.</span></span>

## <a name="response"></a><span data-ttu-id="96bf6-129">応答</span><span class="sxs-lookup"><span data-stu-id="96bf6-129">Response</span></span>

<span data-ttu-id="96bf6-130">成功した場合、この`201 Created`メソッドは作成された[メッセージ](../resources/chatmessage.md)で応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="96bf6-130">If successful, this method returns `201 Created` response code with the [message](../resources/chatmessage.md) that was created.</span></span>

## <a name="examples"></a><span data-ttu-id="96bf6-131">例</span><span class="sxs-lookup"><span data-stu-id="96bf6-131">Examples</span></span> 

### <a name="example-1-hello-world"></a><span data-ttu-id="96bf6-132">例 1: Hello World</span><span class="sxs-lookup"><span data-stu-id="96bf6-132">Example 1: Hello World</span></span>

##### <a name="request"></a><span data-ttu-id="96bf6-133">要求</span><span class="sxs-lookup"><span data-stu-id="96bf6-133">Request</span></span>
<span data-ttu-id="96bf6-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="96bf6-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_chatmessage_from_channel"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/channels/{id}/messages
Content-type: application/json

{
  "body": {
    "contentType": "html",
    "content": "Hello World"
  }
}
```

##### <a name="response"></a><span data-ttu-id="96bf6-135">応答</span><span class="sxs-lookup"><span data-stu-id="96bf6-135">Response</span></span>

<span data-ttu-id="96bf6-136">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="96bf6-136">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 160

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('123456-1234-1234-1234-123456789123')/channels('19%123456789012345678901236%40thread.skype')/messages/$entity",
    "id": "id-value",
    "replyToId": null,
    "etag": "id-value",
    "messageType": "message",
    "createdDateTime": "2019-02-04T19:58:15.511Z",
    "lastModifiedDateTime": null,
    "deleted": false,
    "subject": null,
    "summary": null,
    "importance": "normal",
    "locale": "en-us",
    "policyViolation": null,
    "from": {
        "application": null,
        "device": null,
        "conversation": null,
        "user": {
            "id": "id-value",
            "displayName": "Joh Doe",
            "userIdentityType": "aadUser"
        }
    },
    "body": {
        "contentType": "html",
        "content": "Hello World"
    },
    "attachments": [],
    "mentions": [],
    "reactions": []
}
```

### <a name="example-2-mentions"></a><span data-ttu-id="96bf6-137">例 2:@mentions</span><span class="sxs-lookup"><span data-stu-id="96bf6-137">Example 2: @mentions</span></span>

##### <a name="request"></a><span data-ttu-id="96bf6-138">要求</span><span class="sxs-lookup"><span data-stu-id="96bf6-138">Request</span></span>
<span data-ttu-id="96bf6-139">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="96bf6-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_chatmessage_from_channel"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/channels/{id}/messages
Content-type: application/json

{
  "body": {
    "contentType": "html",
    "content": "Hello World <at id=\"0\">Jane Smith</at>"
  },
  "mentions": [
    {
      "id": 0,
      "mentionText": "Jane Smith",
      "mentioned": {
        "user": {
          "displayName": "Jane Smith",
          "id": "ef1c916a-3135-4417-ba27-8eb7bd084193",
          "userIdentityType": "aadUser"
        }
      }
    }
  ]
}
```

##### <a name="response"></a><span data-ttu-id="96bf6-140">応答</span><span class="sxs-lookup"><span data-stu-id="96bf6-140">Response</span></span>

<span data-ttu-id="96bf6-141">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="96bf6-141">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 160

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('123456-1234-1234-1234-123456789123')/channels('19%123456789012345678901236%40thread.skype')/messages/$entity",
    "id": "id-value",
    "replyToId": null,
    "etag": "id-value",
    "messageType": "message",
    "createdDateTime": "2019-02-04T19:58:15.511Z",
    "lastModifiedDateTime": null,
    "deleted": false,
    "subject": null,
    "summary": null,
    "importance": "normal",
    "locale": "en-us",
    "policyViolation": null,
    "from": {
        "application": null,
        "device": null,
        "conversation": null,
        "user": {
            "id": "id-value",
            "displayName": "Joh Doe",
            "userIdentityType": "aadUser"
        }
    },
    "body": {
        "contentType": "html",
        "content": "Hello World <at id=\"0\">Jane Smith</at>"
    },
    "attachments": [],
    "mentions": [
        {
            "id": 0,
            "mentionText": "Jane Smith",
            "mentioned": {
                "application": null,
                "device": null,
                "conversation": null,
                "user": {
                    "id": "ef1c916a-3135-4417-ba27-8eb7bd084193",
                    "displayName": "Jane Smith",
                    "userIdentityType": "aadUser"
                }
            }
        }
    ],
    "reactions": []
}
```

### <a name="example-3-cards"></a><span data-ttu-id="96bf6-142">例 3: カード</span><span class="sxs-lookup"><span data-stu-id="96bf6-142">Example 3: Cards</span></span>

##### <a name="request"></a><span data-ttu-id="96bf6-143">要求</span><span class="sxs-lookup"><span data-stu-id="96bf6-143">Request</span></span>
<span data-ttu-id="96bf6-144">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="96bf6-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_chatmessage_from_channel"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/channels/{id}/messages
Content-type: application/json

{
    "subject": null,
    "body": {
        "contentType": "html",
        "content": "<attachment id=\"74d20c7f34aa4a7fb74e2b30004247c5\"></attachment>"
    },
    "attachments": [
        {
            "id": "74d20c7f34aa4a7fb74e2b30004247c5",
            "contentType": "application/vnd.microsoft.card.thumbnail",
            "contentUrl": null,
            "content": "{\r\n  \"title\": \"This is an example of posting a card\",\r\n  \"subtitle\": \"<h3>This is the subtitle</h3>\",\r\n  \"text\": \"Here is some body text. <br>\\r\\nAnd a <a href=\\\"http://microsoft.com/\\\">hyperlink</a>. <br>\\r\\nAnd below that is some buttons:\",\r\n  \"buttons\": [\r\n    {\r\n      \"type\": \"messageBack\",\r\n      \"title\": \"Login to FakeBot\",\r\n      \"text\": \"login\",\r\n      \"displayText\": \"login\",\r\n      \"value\": \"login\"\r\n    }\r\n  ]\r\n}",
            "name": null,
            "thumbnailUrl": null
        }
    ]
}
```

##### <a name="response"></a><span data-ttu-id="96bf6-145">応答</span><span class="sxs-lookup"><span data-stu-id="96bf6-145">Response</span></span>

<span data-ttu-id="96bf6-146">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="96bf6-146">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 160

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('bdb7bcda-9c3b-4341-b9a9-f52bf9a23407')/channels('19%3A786524f437c042b68bac5c0511ad6be2%40thread.skype')/messages/$entity",
    "id": "1554837297516",
    "replyToId": null,
    "etag": "1554837297516",
    "messageType": "message",
    "createdDateTime": "2019-04-09T19:14:57.516Z",
    "lastModifiedDateTime": null,
    "deletedDateTime": null,
    "subject": null,
    "summary": null,
    "importance": "normal",
    "locale": "en-us",
    "policyViolation": null,
    "from": {
        "application": null,
        "device": null,
        "conversation": null,
        "user": {
            "id": "id-value",
            "displayName": "Joh Doe",
            "userIdentityType": "aadUser"
        }
    },
    "body": {
        "contentType": "html",
        "content": "<attachment id=\"74d20c7f34aa4a7fb74e2b30004247c5\"></attachment>"
    },
    "attachments": [
        {
            "id": "74d20c7f34aa4a7fb74e2b30004247c5",
            "contentType": "application/vnd.microsoft.card.thumbnail",
            "contentUrl": null,
            "content": "{\r\n  \"title\": \"This is an example of posting a card\",\r\n  \"subtitle\": \"<h3>This is the subtitle</h3>\",\r\n  \"text\": \"Here is some body text. <br>\\r\\n\\r\\n\\r\\nAnd a <a href=\\\"http://microsoft.com/\\\">hyperlink</a>. <br>\\r\\n\\r\\n\\r\\nAnd below that is some buttons:\",\r\n  \"buttons\": [\r\n    {\r\n      \"type\": \"messageBack\",\r\n      \"title\": \"Login to FakeBot\",\r\n      \"text\": \"login\",\r\n      \"displayText\": \"login\",\r\n      \"value\": \"login\"\r\n    }\r\n  ]\r\n}",
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
  "description": "Send message",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/channel-post-chatmessage.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
