---
title: チャネルのメッセージを取得します。
description: チームのチャネルで (返信) せずに 1 つのメッセージを取得します。
author: nkramer
ms.openlocfilehash: 2da10f4151cc1ddaaa1bddfe376f4035a6baa180
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27309227"
---
# <a name="get-channel-message"></a><span data-ttu-id="2ee4a-103">チャネルのメッセージを取得します。</span><span class="sxs-lookup"><span data-stu-id="2ee4a-103">Get channel message</span></span>

> <span data-ttu-id="2ee4a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2ee4a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2ee4a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2ee4a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2ee4a-106">1 つの[メッセージ](../resources/chatmessage.md)(返信) なしでチームの[チャネル](../resources/channel.md)を取得します。</span><span class="sxs-lookup"><span data-stu-id="2ee4a-106">Retrieve a single [message](../resources/chatmessage.md) (without its replies) in a [channel](../resources/channel.md) of a team.</span></span>

## <a name="permissions"></a><span data-ttu-id="2ee4a-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2ee4a-107">Permissions</span></span>
<span data-ttu-id="2ee4a-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2ee4a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ee4a-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2ee4a-110">Permission Type</span></span>|<span data-ttu-id="2ee4a-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2ee4a-111">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="2ee4a-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2ee4a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2ee4a-113">Group.Read.All,Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ee4a-113">Group.Read.All,Group.ReadWrite.All</span></span>|
|<span data-ttu-id="2ee4a-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2ee4a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2ee4a-115">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="2ee4a-115">Not supported</span></span>|
|<span data-ttu-id="2ee4a-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2ee4a-116">Application</span></span>| <span data-ttu-id="2ee4a-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2ee4a-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2ee4a-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2ee4a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/messages/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2ee4a-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="2ee4a-119">Optional query parameters</span></span>
<span data-ttu-id="2ee4a-120">[OData クエリのパラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)は現在サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2ee4a-120">The [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) are not currently supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2ee4a-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2ee4a-121">Request headers</span></span>
| <span data-ttu-id="2ee4a-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2ee4a-122">Header</span></span>       | <span data-ttu-id="2ee4a-123">値</span><span class="sxs-lookup"><span data-stu-id="2ee4a-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2ee4a-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="2ee4a-124">Authorization</span></span>  | <span data-ttu-id="2ee4a-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="2ee4a-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2ee4a-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="2ee4a-127">Request body</span></span>
<span data-ttu-id="2ee4a-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="2ee4a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2ee4a-129">応答</span><span class="sxs-lookup"><span data-stu-id="2ee4a-129">Response</span></span>

<span data-ttu-id="2ee4a-130">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[chatmessage](../resources/chatmessage.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="2ee4a-130">If successful, this method returns a `200 OK` response code and a collection of [chatmessage](../resources/chatmessage.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2ee4a-131">例</span><span class="sxs-lookup"><span data-stu-id="2ee4a-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2ee4a-132">要求</span><span class="sxs-lookup"><span data-stu-id="2ee4a-132">Request</span></span>
<span data-ttu-id="2ee4a-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2ee4a-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_channel_message"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}/messages/{id}
```
##### <a name="response"></a><span data-ttu-id="2ee4a-134">応答</span><span class="sxs-lookup"><span data-stu-id="2ee4a-134">Response</span></span>
<span data-ttu-id="2ee4a-135">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="2ee4a-135">Here is an example of the response.</span></span> 

><span data-ttu-id="2ee4a-136">**注:** 読みやすさの応答オブジェクトを次のように短縮されます。</span><span class="sxs-lookup"><span data-stu-id="2ee4a-136">**Note:** The response object shown here are shortened for readability.</span></span> <span data-ttu-id="2ee4a-137">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="2ee4a-137">All the properties will be returned from an actual call.</span></span>
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
  "id": "id-value",
  "replyToId": "id-value",
  "from": {
      "user": { 
        "id": "id-value",
        "displayName": "John Doe"
      }  
  },
  "etag": "id-value",
  "messageType": "message",
  "createdDateTime": "2018-07-09T07:40:20.152Z",
  "lastModifiedDateTime": "2018-07-09T07:40:20.152Z",
  "body": {
      "content": "Hello World",
      "contentType": "text"
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
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get channel message",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
