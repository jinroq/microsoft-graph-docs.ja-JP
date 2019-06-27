---
title: チャネル内のメッセージに返信する
description: チャネル内の既存メッセージに返信します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: db20e13328fbc2867ae594cd7c8a81403a4f6c97
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35262074"
---
# <a name="reply-to-a-message-in-a-channel"></a><span data-ttu-id="dadc4-103">チャネル内のメッセージに返信する</span><span class="sxs-lookup"><span data-stu-id="dadc4-103">Reply to a message in a channel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dadc4-104">指定した[チャネル](../resources/channel.md)内の[メッセージ](../resources/chatmessage.md)に対する新しい返信を作成します。</span><span class="sxs-lookup"><span data-stu-id="dadc4-104">Create a new reply to a [message](../resources/chatmessage.md) in a specified [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="dadc4-105">**注**: データ移行にこの API を使用することはお勧めしません。</span><span class="sxs-lookup"><span data-stu-id="dadc4-105">**Note**: We don't recommend that you use this API for data migration.</span></span> <span data-ttu-id="dadc4-106">標準的な移行に必要なスループットはありません。</span><span class="sxs-lookup"><span data-stu-id="dadc4-106">It does not have the throughput necessary for a typical migration.</span></span>

## <a name="permissions"></a><span data-ttu-id="dadc4-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="dadc4-107">Permissions</span></span>
<span data-ttu-id="dadc4-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dadc4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dadc4-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="dadc4-110">Permission type</span></span>      | <span data-ttu-id="dadc4-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="dadc4-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dadc4-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="dadc4-112">Delegated (work or school account)</span></span> | <span data-ttu-id="dadc4-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dadc4-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="dadc4-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="dadc4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dadc4-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dadc4-115">Not supported.</span></span>    |
|<span data-ttu-id="dadc4-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="dadc4-116">Application</span></span> | <span data-ttu-id="dadc4-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dadc4-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dadc4-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="dadc4-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels/{id}/messages/{id}/replies
```
## <a name="request-headers"></a><span data-ttu-id="dadc4-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dadc4-119">Request headers</span></span>
| <span data-ttu-id="dadc4-120">名前</span><span class="sxs-lookup"><span data-stu-id="dadc4-120">Name</span></span>       | <span data-ttu-id="dadc4-121">型</span><span class="sxs-lookup"><span data-stu-id="dadc4-121">Type</span></span> | <span data-ttu-id="dadc4-122">説明</span><span class="sxs-lookup"><span data-stu-id="dadc4-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="dadc4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="dadc4-123">Authorization</span></span>  | <span data-ttu-id="dadc4-124">string</span><span class="sxs-lookup"><span data-stu-id="dadc4-124">string</span></span>  | <span data-ttu-id="dadc4-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="dadc4-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dadc4-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="dadc4-127">Request body</span></span>
<span data-ttu-id="dadc4-128">要求本文で、[メッセージ](../resources/chatmessage.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="dadc4-128">In the request body, supply a JSON representation of a [message](../resources/chatmessage.md) object.</span></span> <span data-ttu-id="dadc4-129">Body プロパティのみが必須で、その他のプロパティはオプションです。</span><span class="sxs-lookup"><span data-stu-id="dadc4-129">Only the body property is mandatory, other properties are optional.</span></span>

## <a name="response"></a><span data-ttu-id="dadc4-130">応答</span><span class="sxs-lookup"><span data-stu-id="dadc4-130">Response</span></span>

<span data-ttu-id="dadc4-131">成功した場合、この`201 Created`メソッドは作成された[メッセージ](../resources/chatmessage.md)で応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="dadc4-131">If successful, this method returns `201 Created` response code with the [message](../resources/chatmessage.md) that was created.</span></span>

## <a name="example"></a><span data-ttu-id="dadc4-132">例</span><span class="sxs-lookup"><span data-stu-id="dadc4-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dadc4-133">要求</span><span class="sxs-lookup"><span data-stu-id="dadc4-133">Request</span></span>
<span data-ttu-id="dadc4-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="dadc4-134">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="dadc4-135">応答</span><span class="sxs-lookup"><span data-stu-id="dadc4-135">Response</span></span>

<span data-ttu-id="dadc4-136">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="dadc4-136">Here is an example of the response.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="dadc4-137">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="dadc4-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="dadc4-138">C#</span><span class="sxs-lookup"><span data-stu-id="dadc4-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/post_reply_message-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dadc4-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="dadc4-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/post_reply_message-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="dadc4-140">目的-C</span><span class="sxs-lookup"><span data-stu-id="dadc4-140">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/post_reply_message-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/channel-post-messagereply.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/channel-post-messagereply.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/channel-post-messagereply.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
