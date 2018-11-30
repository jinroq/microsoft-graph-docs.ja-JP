---
title: リストのチャネル メッセージの返信
description: チームのチャネル内のメッセージの返信のすべてを一覧表示します。
ms.openlocfilehash: 7133f48233f2b164aa6643ba896dd0612645e7e8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066392"
---
# <a name="list-channel-message-replies"></a><span data-ttu-id="b1434-103">リストのチャネル メッセージの返信</span><span class="sxs-lookup"><span data-stu-id="b1434-103">List channel message replies</span></span>

> <span data-ttu-id="b1434-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b1434-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b1434-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b1434-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b1434-106">チームの[チャネル](../resources/channel.md)内の[メッセージ](../resources/chatmessage.md)の返信のすべてを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="b1434-106">List all the replies of a [message](../resources/chatmessage.md) in a [channel](../resources/channel.md) of a team.</span></span>

## <a name="permissions"></a><span data-ttu-id="b1434-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b1434-107">Permissions</span></span>
<span data-ttu-id="b1434-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b1434-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1434-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b1434-110">Permission Type</span></span>|<span data-ttu-id="b1434-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b1434-111">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="b1434-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b1434-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b1434-113">Group.Read.All,Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1434-113">Group.Read.All,Group.ReadWrite.All</span></span>|
|<span data-ttu-id="b1434-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b1434-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b1434-115">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="b1434-115">Not supported</span></span>|
|<span data-ttu-id="b1434-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b1434-116">Application</span></span>| <span data-ttu-id="b1434-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b1434-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b1434-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b1434-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/messages/{id}/replies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b1434-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="b1434-119">Optional query parameters</span></span>
<span data-ttu-id="b1434-120">[OData クエリのパラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)は現在サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b1434-120">The [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) are not currently supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b1434-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b1434-121">Request headers</span></span>
| <span data-ttu-id="b1434-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b1434-122">Header</span></span>       | <span data-ttu-id="b1434-123">値</span><span class="sxs-lookup"><span data-stu-id="b1434-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b1434-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b1434-124">Authorization</span></span>  | <span data-ttu-id="b1434-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b1434-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b1434-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="b1434-127">Request body</span></span>
<span data-ttu-id="b1434-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="b1434-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b1434-129">応答</span><span class="sxs-lookup"><span data-stu-id="b1434-129">Response</span></span>
<span data-ttu-id="b1434-130">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[chatmessage](../resources/channel.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="b1434-130">If successful, this method returns a `200 OK` response code and a collection of [chatmessage](../resources/channel.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b1434-131">例</span><span class="sxs-lookup"><span data-stu-id="b1434-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b1434-132">要求</span><span class="sxs-lookup"><span data-stu-id="b1434-132">Request</span></span>
<span data-ttu-id="b1434-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b1434-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_channel_message_replies"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}/messages/{id}/replies
```
##### <a name="response"></a><span data-ttu-id="b1434-134">応答</span><span class="sxs-lookup"><span data-stu-id="b1434-134">Response</span></span>
<span data-ttu-id="b1434-135">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="b1434-135">Here is an example of the response.</span></span> 

><span data-ttu-id="b1434-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="b1434-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "value": [
    {
        "id": "id-value",
        "replyToId": "id-value",
        "from" : {
            "user": { 
            "id":  "id-value",
            "displayName": "John Doe"
            }  
        },
        "etag": "id-value",
        "messageType": "message",
        "createdDateTime": "2018-07-09T07:40:20.152Z",
        "lastModifiedDateTime": "2018-07-09T07:40:20.152Z",
        "body": {
            "content": "This is a response to a message.",
            "contentType": "Text"
        },
        "attachments": [
          {
              "id": "5e32f195-168a-474f-a273-123123123",
              "contentType": "reference",
              "contentUrl": "https://test.sharepoint.com/sites/TestSite/Shared%20Documents/General/Test.txt",
              "content": null,
              "name": "Test.txt",
              "thumbnailUrl": null
          }
        ],
        "mentions": [
            {
                "type": "user",
                "id": "id-value ",
                "mentionText": "Test User"
            }
        ],
        "importance": "normal",
        "reactions": [
            {
                "reactionType": "like",
                "user": {
                    "id": "id-value",
                    "displayName": "John Doe"
                },
                "createdDateTime": "2018-07-09T07:40:20.152Z"
            }
        ],
        "locale": "en-us"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get channel message replies",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
