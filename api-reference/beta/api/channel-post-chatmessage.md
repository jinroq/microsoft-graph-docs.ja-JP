---
title: チャネル内でメッセージを送信する
description: 指定したチャネルで新しいメッセージを送信します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 960c5d8164f2681b71bb2c3b46383bb210240bb2
ms.sourcegitcommit: 3410e1b8dcf62a7b0e4d6b11920912479f21feb2
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/26/2019
ms.locfileid: "30799985"
---
# <a name="send-a-message-to-a-channel"></a><span data-ttu-id="af35e-103">メッセージをチャネルに送信する</span><span class="sxs-lookup"><span data-stu-id="af35e-103">Send a message to a channel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="af35e-104">指定した[チャネル](../resources/channel.md)で新しい[メッセージ](../resources/chatmessage.md)を作成します。</span><span class="sxs-lookup"><span data-stu-id="af35e-104">Create a new [message](../resources/chatmessage.md) in the specified [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="af35e-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="af35e-105">Permissions</span></span>
<span data-ttu-id="af35e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="af35e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="af35e-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="af35e-108">Permission type</span></span>      | <span data-ttu-id="af35e-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="af35e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="af35e-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="af35e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="af35e-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af35e-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="af35e-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="af35e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="af35e-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="af35e-113">Not supported.</span></span>    |
|<span data-ttu-id="af35e-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="af35e-114">Application</span></span> | <span data-ttu-id="af35e-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="af35e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="af35e-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="af35e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels/{id}/messages
```

## <a name="request-headers"></a><span data-ttu-id="af35e-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="af35e-117">Request headers</span></span>
| <span data-ttu-id="af35e-118">名前</span><span class="sxs-lookup"><span data-stu-id="af35e-118">Name</span></span>       | <span data-ttu-id="af35e-119">種類</span><span class="sxs-lookup"><span data-stu-id="af35e-119">Type</span></span> | <span data-ttu-id="af35e-120">説明</span><span class="sxs-lookup"><span data-stu-id="af35e-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="af35e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="af35e-121">Authorization</span></span>  | <span data-ttu-id="af35e-122">string</span><span class="sxs-lookup"><span data-stu-id="af35e-122">string</span></span>  | <span data-ttu-id="af35e-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="af35e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="af35e-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="af35e-125">Request body</span></span>
<span data-ttu-id="af35e-126">要求本文で、[メッセージ](../resources/chatmessage.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="af35e-126">In the request body, supply a JSON representation of a [message](../resources/chatmessage.md) object.</span></span> <span data-ttu-id="af35e-127">body プロパティのみが必須で、その他のプロパティはオプションです。</span><span class="sxs-lookup"><span data-stu-id="af35e-127">Only the body property is mandatory, other properties are optional.</span></span>

> <span data-ttu-id="af35e-128">注: 添付ファイルと画像を使用したメッセージの送信はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="af35e-128">Note: Sending messages with attachments and images is not supported.</span></span>

## <a name="response"></a><span data-ttu-id="af35e-129">応答</span><span class="sxs-lookup"><span data-stu-id="af35e-129">Response</span></span>

<span data-ttu-id="af35e-130">成功した場合、この`201 Created`メソッドは作成された[メッセージ](../resources/chatmessage.md)で応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="af35e-130">If successful, this method returns `201 Created` response code with the [message](../resources/chatmessage.md) that was created.</span></span>

## <a name="examples"></a><span data-ttu-id="af35e-131">例</span><span class="sxs-lookup"><span data-stu-id="af35e-131">Examples</span></span> 

### <a name="example-1-hello-world"></a><span data-ttu-id="af35e-132">例 1: Hello World</span><span class="sxs-lookup"><span data-stu-id="af35e-132">Example 1: Hello World</span></span>

##### <a name="request"></a><span data-ttu-id="af35e-133">要求</span><span class="sxs-lookup"><span data-stu-id="af35e-133">Request</span></span>
<span data-ttu-id="af35e-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="af35e-134">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="af35e-135">応答</span><span class="sxs-lookup"><span data-stu-id="af35e-135">Response</span></span>

<span data-ttu-id="af35e-136">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="af35e-136">Here is an example of the response.</span></span>
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

### <a name="example-2-mentions"></a><span data-ttu-id="af35e-137">例 2: @mentions</span><span class="sxs-lookup"><span data-stu-id="af35e-137">Example 2: @mentions</span></span>

##### <a name="request"></a><span data-ttu-id="af35e-138">要求</span><span class="sxs-lookup"><span data-stu-id="af35e-138">Request</span></span>
<span data-ttu-id="af35e-139">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="af35e-139">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="af35e-140">応答</span><span class="sxs-lookup"><span data-stu-id="af35e-140">Response</span></span>

<span data-ttu-id="af35e-141">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="af35e-141">Here is an example of the response.</span></span>
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
