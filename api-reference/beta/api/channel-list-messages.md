---
title: リストからチャネルのメッセージ
description: '(返信) のないチームのチャネル内のメッセージの一覧を取得します。 メッセージの返信を取得するには、] ボックスの一覧のメッセージの返信または get メッセージ応答 API を呼び出します。 '
localization_priority: Priority
ms.openlocfilehash: c972b84b0ec4de9389f8a0e861cafb74d7b23020
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27867096"
---
# <a name="list-channel-messages"></a><span data-ttu-id="8a5cd-104">リストからチャネルのメッセージ</span><span class="sxs-lookup"><span data-stu-id="8a5cd-104">List channel messages</span></span>

> <span data-ttu-id="8a5cd-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8a5cd-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8a5cd-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8a5cd-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8a5cd-107">[チーム](../resources/team.md)の[チャネル](../resources/channel.md)で (せずに、応答)[メッセージ](../resources/chatmessage.md)の一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="8a5cd-107">Retrieve the list of [messages](../resources/chatmessage.md) (without the replies) in a [channel](../resources/channel.md) of a [team](../resources/team.md).</span></span> <span data-ttu-id="8a5cd-108">メッセージの返信を取得するには、[一覧のメッセージの返信](channel-get-messagereply.md)または、[メッセージの返信を取得する](channel-list-messagereplies.md)API を呼び出します。</span><span class="sxs-lookup"><span data-stu-id="8a5cd-108">To get the replies for a message, call the [list message replies](channel-get-messagereply.md) or the [get message reply](channel-list-messagereplies.md) API.</span></span> 

## <a name="permissions"></a><span data-ttu-id="8a5cd-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8a5cd-109">Permissions</span></span>
<span data-ttu-id="8a5cd-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8a5cd-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8a5cd-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8a5cd-112">Permission Type</span></span>|<span data-ttu-id="8a5cd-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8a5cd-113">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="8a5cd-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8a5cd-114">Delegated (work or school account)</span></span>|<span data-ttu-id="8a5cd-115">Group.Read.All,Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a5cd-115">Group.Read.All,Group.ReadWrite.All</span></span>|
|<span data-ttu-id="8a5cd-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8a5cd-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8a5cd-117">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="8a5cd-117">Not supported</span></span>|
|<span data-ttu-id="8a5cd-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8a5cd-118">Application</span></span>| <span data-ttu-id="8a5cd-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8a5cd-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8a5cd-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8a5cd-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/messages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8a5cd-121">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="8a5cd-121">Optional query parameters</span></span>
<span data-ttu-id="8a5cd-122">[OData クエリのパラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)は現在サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8a5cd-122">The [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) are not currently supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8a5cd-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8a5cd-123">Request headers</span></span>
| <span data-ttu-id="8a5cd-124">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8a5cd-124">Header</span></span>       | <span data-ttu-id="8a5cd-125">値</span><span class="sxs-lookup"><span data-stu-id="8a5cd-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8a5cd-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="8a5cd-126">Authorization</span></span>  | <span data-ttu-id="8a5cd-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8a5cd-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8a5cd-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="8a5cd-129">Request body</span></span>
<span data-ttu-id="8a5cd-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="8a5cd-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8a5cd-131">応答</span><span class="sxs-lookup"><span data-stu-id="8a5cd-131">Response</span></span>

<span data-ttu-id="8a5cd-132">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[chatmessage](../resources/channel.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="8a5cd-132">If successful, this method returns a `200 OK` response code and a collection of [chatmessage](../resources/channel.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8a5cd-133">例</span><span class="sxs-lookup"><span data-stu-id="8a5cd-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8a5cd-134">要求</span><span class="sxs-lookup"><span data-stu-id="8a5cd-134">Request</span></span>
<span data-ttu-id="8a5cd-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8a5cd-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_channel_messages"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}/messages
```
##### <a name="response"></a><span data-ttu-id="8a5cd-136">応答</span><span class="sxs-lookup"><span data-stu-id="8a5cd-136">Response</span></span>
<span data-ttu-id="8a5cd-137">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="8a5cd-137">Here is an example of the response.</span></span> 

><span data-ttu-id="8a5cd-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="8a5cd-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
            "content": "Hello World",
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
  "description": "Get channel messages",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
