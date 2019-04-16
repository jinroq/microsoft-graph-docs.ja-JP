---
title: チャネル メッセージを一覧表示する
description: 'チームのチャネルに含まれるメッセージの一覧を取得します (返信なし)。 メッセージの返信を取得するには、メッセージの返信一覧 API またはメッセージの返信取得 API を呼び出します。 '
localization_priority: Priority
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 000e85db202ea08677876a288e6a68dc2e20ed52
ms.sourcegitcommit: a39db1154a07aa0dd7e96fb6f9d7e891a812207e
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/16/2019
ms.locfileid: "31890004"
---
# <a name="list-channel-messages"></a><span data-ttu-id="5ef98-104">チャネル メッセージを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="5ef98-104">List channel messages</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5ef98-105">[チーム](../resources/team.md)の[チャネル](../resources/channel.md)で[メッセージ](../resources/chatmessage.md)の一覧を取得します (返信なし)。</span><span class="sxs-lookup"><span data-stu-id="5ef98-105">Retrieve the list of [messages](../resources/chatmessage.md) (without the replies) in a [channel](../resources/channel.md) of a [team](../resources/team.md).</span></span> <span data-ttu-id="5ef98-106">メッセージの返信を取得するには、[メッセージの返信一覧](channel-get-messagereply.md) API または [メッセージの返信取得](channel-list-messagereplies.md) API を呼び出します。</span><span class="sxs-lookup"><span data-stu-id="5ef98-106">To get the replies for a message, call the [list message replies](channel-get-messagereply.md) or the [get message reply](channel-list-messagereplies.md) API.</span></span> 

## <a name="permissions"></a><span data-ttu-id="5ef98-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5ef98-107">Permissions</span></span>
<span data-ttu-id="5ef98-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5ef98-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ef98-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5ef98-110">Permission Type</span></span>|<span data-ttu-id="5ef98-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5ef98-111">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="5ef98-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5ef98-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5ef98-113">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ef98-113">Group.Read.All,Group.ReadWrite.All</span></span>|
|<span data-ttu-id="5ef98-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5ef98-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5ef98-115">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="5ef98-115">Not supported</span></span>|
|<span data-ttu-id="5ef98-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5ef98-116">Application</span></span>| <span data-ttu-id="5ef98-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5ef98-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5ef98-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5ef98-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/messages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5ef98-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="5ef98-119">Optional query parameters</span></span>
<span data-ttu-id="5ef98-120">[OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)は現在サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5ef98-120">The [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) are not currently supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5ef98-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5ef98-121">Request headers</span></span>
| <span data-ttu-id="5ef98-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5ef98-122">Header</span></span>       | <span data-ttu-id="5ef98-123">値</span><span class="sxs-lookup"><span data-stu-id="5ef98-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5ef98-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="5ef98-124">Authorization</span></span>  | <span data-ttu-id="5ef98-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5ef98-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5ef98-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="5ef98-127">Request body</span></span>
<span data-ttu-id="5ef98-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="5ef98-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5ef98-129">応答</span><span class="sxs-lookup"><span data-stu-id="5ef98-129">Response</span></span>

<span data-ttu-id="5ef98-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [chatmessage](../resources/chatmessage.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="5ef98-130">If successful, this method returns a `200 OK` response code and a collection of [chatmessage](../resources/chatmessage.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5ef98-131">例</span><span class="sxs-lookup"><span data-stu-id="5ef98-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5ef98-132">要求</span><span class="sxs-lookup"><span data-stu-id="5ef98-132">Request</span></span>
<span data-ttu-id="5ef98-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5ef98-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_channel_messages"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}/messages
```
##### <a name="response"></a><span data-ttu-id="5ef98-134">応答</span><span class="sxs-lookup"><span data-stu-id="5ef98-134">Response</span></span>
<span data-ttu-id="5ef98-135">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="5ef98-135">Here is an example of the response.</span></span> 

><span data-ttu-id="5ef98-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="5ef98-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
                "id": "id-value ",
                "mentionText": "Test User",
                "mentioned": {
                "user": {
                    "id": "id-value",
                    "displayName: "string"
                }
            }
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
<!--
{
  "type": "#page.annotation",
  "description": "Get channel messages",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/channel-list-messages.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
