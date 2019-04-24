---
title: チャネル内のメッセージに返信する
description: チャネル内の既存メッセージに返信します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 15e1bfffe7d7634092937a0605debfd5294b142b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32456466"
---
# <a name="reply-to-a-message-in-a-channel"></a><span data-ttu-id="a95a0-103">チャネル内のメッセージに返信する</span><span class="sxs-lookup"><span data-stu-id="a95a0-103">Reply to a message in a channel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a95a0-104">指定した[チャネル](../resources/channel.md)内の[メッセージ](../resources/chatmessage.md)に対する新しい返信を作成します。</span><span class="sxs-lookup"><span data-stu-id="a95a0-104">Create a new reply to a [message](../resources/chatmessage.md) in a specified [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a95a0-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a95a0-105">Permissions</span></span>
<span data-ttu-id="a95a0-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a95a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a95a0-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a95a0-108">Permission type</span></span>      | <span data-ttu-id="a95a0-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a95a0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a95a0-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a95a0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a95a0-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a95a0-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a95a0-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a95a0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a95a0-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a95a0-113">Not supported.</span></span>    |
|<span data-ttu-id="a95a0-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a95a0-114">Application</span></span> | <span data-ttu-id="a95a0-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a95a0-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a95a0-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a95a0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels/{id}/messages/{id}/replies
```
## <a name="request-headers"></a><span data-ttu-id="a95a0-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a95a0-117">Request headers</span></span>
| <span data-ttu-id="a95a0-118">名前</span><span class="sxs-lookup"><span data-stu-id="a95a0-118">Name</span></span>       | <span data-ttu-id="a95a0-119">型</span><span class="sxs-lookup"><span data-stu-id="a95a0-119">Type</span></span> | <span data-ttu-id="a95a0-120">説明</span><span class="sxs-lookup"><span data-stu-id="a95a0-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a95a0-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a95a0-121">Authorization</span></span>  | <span data-ttu-id="a95a0-122">string</span><span class="sxs-lookup"><span data-stu-id="a95a0-122">string</span></span>  | <span data-ttu-id="a95a0-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a95a0-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a95a0-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="a95a0-125">Request body</span></span>
<span data-ttu-id="a95a0-126">要求本文で、[メッセージ](../resources/chatmessage.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a95a0-126">In the request body, supply a JSON representation of a [message](../resources/chatmessage.md) object.</span></span> <span data-ttu-id="a95a0-127">body プロパティのみが必須で、その他のプロパティはオプションです。</span><span class="sxs-lookup"><span data-stu-id="a95a0-127">Only the body property is mandatory, other properties are optional.</span></span>

## <a name="response"></a><span data-ttu-id="a95a0-128">応答</span><span class="sxs-lookup"><span data-stu-id="a95a0-128">Response</span></span>

<span data-ttu-id="a95a0-129">成功した場合、この`201 Created`メソッドは作成された[メッセージ](../resources/chatmessage.md)で応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="a95a0-129">If successful, this method returns `201 Created` response code with the [message](../resources/chatmessage.md) that was created.</span></span>

## <a name="example"></a><span data-ttu-id="a95a0-130">例</span><span class="sxs-lookup"><span data-stu-id="a95a0-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a95a0-131">要求</span><span class="sxs-lookup"><span data-stu-id="a95a0-131">Request</span></span>
<span data-ttu-id="a95a0-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a95a0-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_reply_message"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/channels/{id}/messages/{id}/replies
Content-type: application/json

{
  "body": {
    "contentType": "html",
    "content": "Hello World"
  }
}
```

##### <a name="response"></a><span data-ttu-id="a95a0-133">応答</span><span class="sxs-lookup"><span data-stu-id="a95a0-133">Response</span></span>

<span data-ttu-id="a95a0-134">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="a95a0-134">Here is an example of the response.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('123456-1234-1234-1234-123456789123')/channels('19%123456789012345678901236%40thread.skype')/messages('id-value')/replies/$entity",
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
  "description": "Create a reply message",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/channel-post-reply_chatmessage.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
