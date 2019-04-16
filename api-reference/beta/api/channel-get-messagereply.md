---
title: チャネルメッセージへの返信を取得する
description: チームのチャネル内のメッセージに対して1回の返信を取得します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: e61996d8f23e2606598954ce73ce0a4270308126
ms.sourcegitcommit: a39db1154a07aa0dd7e96fb6f9d7e891a812207e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/16/2019
ms.locfileid: "31889969"
---
# <a name="get-a-reply-to-a-channel-message"></a><span data-ttu-id="cdfcd-103">チャネルメッセージへの返信を取得する</span><span class="sxs-lookup"><span data-stu-id="cdfcd-103">Get a reply to a channel message</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cdfcd-104">チームの[チャネル](../resources/channel.md)内の[メッセージ](../resources/chatmessage.md)に対して1回の返信を取得します。</span><span class="sxs-lookup"><span data-stu-id="cdfcd-104">Get a single reply to a [message](../resources/chatmessage.md) in a [channel](../resources/channel.md) of a team.</span></span>

## <a name="permissions"></a><span data-ttu-id="cdfcd-105">権限</span><span class="sxs-lookup"><span data-stu-id="cdfcd-105">Permissions</span></span>
<span data-ttu-id="cdfcd-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cdfcd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cdfcd-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cdfcd-108">Permission Type</span></span>|<span data-ttu-id="cdfcd-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="cdfcd-109">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="cdfcd-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cdfcd-110">Delegated (work or school account)</span></span>|<span data-ttu-id="cdfcd-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cdfcd-111">Group.Read.All,Group.ReadWrite.All</span></span>|
|<span data-ttu-id="cdfcd-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cdfcd-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cdfcd-113">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="cdfcd-113">Not supported</span></span>|
|<span data-ttu-id="cdfcd-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cdfcd-114">Application</span></span>| <span data-ttu-id="cdfcd-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cdfcd-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cdfcd-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cdfcd-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/messages/{id}/replies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cdfcd-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="cdfcd-117">Optional query parameters</span></span>
<span data-ttu-id="cdfcd-118">[OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)は現在サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cdfcd-118">The [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) are not currently supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cdfcd-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cdfcd-119">Request headers</span></span>
| <span data-ttu-id="cdfcd-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cdfcd-120">Header</span></span>       | <span data-ttu-id="cdfcd-121">値</span><span class="sxs-lookup"><span data-stu-id="cdfcd-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cdfcd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="cdfcd-122">Authorization</span></span>  | <span data-ttu-id="cdfcd-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="cdfcd-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cdfcd-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="cdfcd-125">Request body</span></span>
<span data-ttu-id="cdfcd-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="cdfcd-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cdfcd-127">応答</span><span class="sxs-lookup"><span data-stu-id="cdfcd-127">Response</span></span>
<span data-ttu-id="cdfcd-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [chatmessage](../resources/chatmessage.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="cdfcd-128">If successful, this method returns a `200 OK` response code and a collection of [chatmessage](../resources/chatmessage.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="cdfcd-129">例</span><span class="sxs-lookup"><span data-stu-id="cdfcd-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cdfcd-130">要求</span><span class="sxs-lookup"><span data-stu-id="cdfcd-130">Request</span></span>
<span data-ttu-id="cdfcd-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="cdfcd-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_channel_message_reply"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}/messages/{id}/replies/{id}
```
##### <a name="response"></a><span data-ttu-id="cdfcd-132">応答</span><span class="sxs-lookup"><span data-stu-id="cdfcd-132">Response</span></span>
<span data-ttu-id="cdfcd-133">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="cdfcd-133">Here is an example of the response.</span></span> 

><span data-ttu-id="cdfcd-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="cdfcd-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
            "id": "5e32f195-168a-474f-a273-12312312312",
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
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/channel-get-messagereply.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
