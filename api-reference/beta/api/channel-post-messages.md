---
title: チャネルでの chatMessage の作成
description: 指定したチャネルで新しい chatMessage を作成します。
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 363201e1c1ad508fdc2b3926557fbd502834b58e
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35438399"
---
# <a name="create-chatmessage-in-a-channel"></a><span data-ttu-id="9665e-103">チャネルでの chatMessage の作成</span><span class="sxs-lookup"><span data-stu-id="9665e-103">Create chatMessage in a channel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9665e-104">指定した[チャネル](../resources/channel.md)で新しい[chatmessage](../resources/chatmessage.md)を作成します。</span><span class="sxs-lookup"><span data-stu-id="9665e-104">Create a new [chatMessage](../resources/chatmessage.md) in the specified [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="9665e-105">**注**: データ移行にこの API を使用することはお勧めしません。</span><span class="sxs-lookup"><span data-stu-id="9665e-105">**Note**: We don't recommend that you use this API for data migration.</span></span> <span data-ttu-id="9665e-106">標準的な移行に必要なスループットはありません。</span><span class="sxs-lookup"><span data-stu-id="9665e-106">It does not have the throughput necessary for a typical migration.</span></span>

## <a name="permissions"></a><span data-ttu-id="9665e-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9665e-107">Permissions</span></span>

<span data-ttu-id="9665e-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9665e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9665e-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9665e-110">Permission type</span></span>                        | <span data-ttu-id="9665e-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9665e-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9665e-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9665e-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="9665e-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9665e-113">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="9665e-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9665e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9665e-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9665e-115">Not supported.</span></span> |
| <span data-ttu-id="9665e-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9665e-116">Application</span></span>                            | <span data-ttu-id="9665e-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9665e-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9665e-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9665e-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{id}/channels/{id}/messages
```

## <a name="request-headers"></a><span data-ttu-id="9665e-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9665e-119">Request headers</span></span>

| <span data-ttu-id="9665e-120">名前</span><span class="sxs-lookup"><span data-stu-id="9665e-120">Name</span></span>          | <span data-ttu-id="9665e-121">説明</span><span class="sxs-lookup"><span data-stu-id="9665e-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="9665e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9665e-122">Authorization</span></span> | <span data-ttu-id="9665e-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="9665e-123">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="9665e-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="9665e-124">Request body</span></span>

<span data-ttu-id="9665e-125">要求本文で、[メッセージ](../resources/chatmessage.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="9665e-125">In the request body, supply a JSON representation of a [message](../resources/chatmessage.md) object.</span></span> <span data-ttu-id="9665e-126">Body プロパティのみが必須で、その他のプロパティはオプションです。</span><span class="sxs-lookup"><span data-stu-id="9665e-126">Only the body property is mandatory, other properties are optional.</span></span>

> <span data-ttu-id="9665e-127">注: 添付ファイルと画像を使用したメッセージの送信はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9665e-127">Note: Sending messages with attachments and images is not supported.</span></span>

## <a name="response"></a><span data-ttu-id="9665e-128">応答</span><span class="sxs-lookup"><span data-stu-id="9665e-128">Response</span></span>

<span data-ttu-id="9665e-129">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で新しい[chatmessage](../resources/chatmessage.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="9665e-129">If successful, this method returns a `201 Created` response code and a new [chatMessage](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9665e-130">例</span><span class="sxs-lookup"><span data-stu-id="9665e-130">Examples</span></span>

### <a name="example-1-hello-world"></a><span data-ttu-id="9665e-131">例 1: Hello World</span><span class="sxs-lookup"><span data-stu-id="9665e-131">Example 1: Hello World</span></span>

#### <a name="request"></a><span data-ttu-id="9665e-132">要求</span><span class="sxs-lookup"><span data-stu-id="9665e-132">Request</span></span>
<span data-ttu-id="9665e-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9665e-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9665e-134">プロトコル</span><span class="sxs-lookup"><span data-stu-id="9665e-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_chatmessage_from_channel"
}-->

```http
POST https://graph.microsoft.com/beta/teams/{id}/channels/{id}/messages
Content-type: application/json

{
  "body": {
    "content": "Hello World"
  }
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9665e-135">C#</span><span class="sxs-lookup"><span data-stu-id="9665e-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-chatmessage-from-channel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9665e-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="9665e-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-chatmessage-from-channel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9665e-137">目的-C</span><span class="sxs-lookup"><span data-stu-id="9665e-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-chatmessage-from-channel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9665e-138">応答</span><span class="sxs-lookup"><span data-stu-id="9665e-138">Response</span></span>

<span data-ttu-id="9665e-139">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9665e-139">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="9665e-140">ここに示す response オブジェクトは読みやすいように短縮される場合があります。</span><span class="sxs-lookup"><span data-stu-id="9665e-140">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="9665e-141">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="9665e-141">All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-mentions"></a><span data-ttu-id="9665e-142">例 2: @mentions</span><span class="sxs-lookup"><span data-stu-id="9665e-142">Example 2: @mentions</span></span>

#### <a name="request"></a><span data-ttu-id="9665e-143">要求</span><span class="sxs-lookup"><span data-stu-id="9665e-143">Request</span></span>
<span data-ttu-id="9665e-144">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9665e-144">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="9665e-145">応答</span><span class="sxs-lookup"><span data-stu-id="9665e-145">Response</span></span>

<span data-ttu-id="9665e-146">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9665e-146">The following is an example of the response.</span></span>
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

### <a name="example-3-cards"></a><span data-ttu-id="9665e-147">例 3: カード</span><span class="sxs-lookup"><span data-stu-id="9665e-147">Example 3: Cards</span></span>

#### <a name="request"></a><span data-ttu-id="9665e-148">要求</span><span class="sxs-lookup"><span data-stu-id="9665e-148">Request</span></span>
<span data-ttu-id="9665e-149">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9665e-149">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="9665e-150">応答</span><span class="sxs-lookup"><span data-stu-id="9665e-150">Response</span></span>

<span data-ttu-id="9665e-151">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9665e-151">The following is an example of the response.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="9665e-152">関連項目</span><span class="sxs-lookup"><span data-stu-id="9665e-152">See also</span></span>

- [<span data-ttu-id="9665e-153">カードリファレンス</span><span class="sxs-lookup"><span data-stu-id="9665e-153">Cards Reference</span></span>](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/cards/cards-reference)

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
  ]
}
-->
