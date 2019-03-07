---
title: チャネルでメッセージを送信する
description: 指定したチャネルで新しいメッセージを送信します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 42dcf26a5e67f58668f4bd321a68e684feef237f
ms.sourcegitcommit: d1a9e7c8e1376a99c5a5416257889ec113613a77
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/07/2019
ms.locfileid: "30458639"
---
# <a name="send-a-message-to-a-channel"></a><span data-ttu-id="50418-103">チャネルへのメッセージの送信</span><span class="sxs-lookup"><span data-stu-id="50418-103">Send a message to a channel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="50418-104">指定した[チャネル](../resources/channel.md)で新しい[メッセージ](../resources/chatmessage.md)を作成します。</span><span class="sxs-lookup"><span data-stu-id="50418-104">Create a new [message](../resources/chatmessage.md) in the specified [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="50418-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="50418-105">Permissions</span></span>
<span data-ttu-id="50418-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="50418-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50418-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="50418-108">Permission type</span></span>      | <span data-ttu-id="50418-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="50418-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="50418-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="50418-110">Delegated (work or school account)</span></span> | <span data-ttu-id="50418-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50418-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="50418-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="50418-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="50418-113">サポートされません。</span><span class="sxs-lookup"><span data-stu-id="50418-113">Not supported.</span></span>    |
|<span data-ttu-id="50418-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="50418-114">Application</span></span> | <span data-ttu-id="50418-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="50418-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="50418-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="50418-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels/{id}/messages
```

## <a name="request-headers"></a><span data-ttu-id="50418-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="50418-117">Request headers</span></span>
| <span data-ttu-id="50418-118">名前</span><span class="sxs-lookup"><span data-stu-id="50418-118">Name</span></span>       | <span data-ttu-id="50418-119">種類</span><span class="sxs-lookup"><span data-stu-id="50418-119">Type</span></span> | <span data-ttu-id="50418-120">説明</span><span class="sxs-lookup"><span data-stu-id="50418-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="50418-121">承認</span><span class="sxs-lookup"><span data-stu-id="50418-121">Authorization</span></span>  | <span data-ttu-id="50418-122">string</span><span class="sxs-lookup"><span data-stu-id="50418-122">string</span></span>  | <span data-ttu-id="50418-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="50418-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="50418-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="50418-125">Request body</span></span>
<span data-ttu-id="50418-126">要求本文で、[メッセージ](../resources/chatmessage.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="50418-126">In the request body, supply a JSON representation of a [message](../resources/chatmessage.md) object.</span></span> <span data-ttu-id="50418-127">body プロパティのみが必須で、その他のプロパティはオプションです。</span><span class="sxs-lookup"><span data-stu-id="50418-127">Only the body property is mandatory, other properties are optional.</span></span>

> <span data-ttu-id="50418-128">注: 添付ファイルと画像を使用したメッセージの送信はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="50418-128">Note: Sending messages with attachments and images is not supported.</span></span>

## <a name="response"></a><span data-ttu-id="50418-129">応答</span><span class="sxs-lookup"><span data-stu-id="50418-129">Response</span></span>

<span data-ttu-id="50418-130">成功した場合、この`201 Created`メソッドは作成された[メッセージ](../resources/chatmessage.md)で応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="50418-130">If successful, this method returns `201 Created` response code with the [message](../resources/chatmessage.md) that was created.</span></span>

## <a name="example"></a><span data-ttu-id="50418-131">例</span><span class="sxs-lookup"><span data-stu-id="50418-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="50418-132">要求</span><span class="sxs-lookup"><span data-stu-id="50418-132">Request</span></span>
<span data-ttu-id="50418-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="50418-133">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="50418-134">応答</span><span class="sxs-lookup"><span data-stu-id="50418-134">Response</span></span>

<span data-ttu-id="50418-135">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="50418-135">Here is an example of the response.</span></span>
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
