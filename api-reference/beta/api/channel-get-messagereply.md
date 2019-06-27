---
title: チャネルメッセージへの返信を取得する
description: チームのチャネル内のメッセージに対して1回の返信を取得します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 4d0ec855b2b91ce9ee912725140e7222c32ff630
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35262112"
---
# <a name="get-a-reply-to-a-channel-message"></a><span data-ttu-id="0884b-103">チャネルメッセージへの返信を取得する</span><span class="sxs-lookup"><span data-stu-id="0884b-103">Get a reply to a channel message</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0884b-104">チームの[チャネル](../resources/channel.md)内の[メッセージ](../resources/chatmessage.md)に対して1回の返信を取得します。</span><span class="sxs-lookup"><span data-stu-id="0884b-104">Get a single reply to a [message](../resources/chatmessage.md) in a [channel](../resources/channel.md) of a team.</span></span>

## <a name="permissions"></a><span data-ttu-id="0884b-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0884b-105">Permissions</span></span>

<span data-ttu-id="0884b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0884b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0884b-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0884b-108">Permission Type</span></span>|<span data-ttu-id="0884b-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0884b-109">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="0884b-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0884b-110">Delegated (work or school account)</span></span>|<span data-ttu-id="0884b-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0884b-111">Group.Read.All,Group.ReadWrite.All</span></span>|
|<span data-ttu-id="0884b-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0884b-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0884b-113">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="0884b-113">Not supported</span></span>|
|<span data-ttu-id="0884b-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0884b-114">Application</span></span>| <span data-ttu-id="0884b-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0884b-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0884b-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0884b-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/messages/{id}/replies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0884b-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="0884b-117">Optional query parameters</span></span>

<span data-ttu-id="0884b-118">[OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)は現在サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0884b-118">The [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) are not currently supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0884b-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0884b-119">Request headers</span></span>

| <span data-ttu-id="0884b-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0884b-120">Header</span></span>       | <span data-ttu-id="0884b-121">値</span><span class="sxs-lookup"><span data-stu-id="0884b-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0884b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0884b-122">Authorization</span></span>  | <span data-ttu-id="0884b-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="0884b-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0884b-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="0884b-125">Request body</span></span>

<span data-ttu-id="0884b-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="0884b-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0884b-127">応答</span><span class="sxs-lookup"><span data-stu-id="0884b-127">Response</span></span>

<span data-ttu-id="0884b-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [chatmessage](../resources/chatmessage.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0884b-128">If successful, this method returns a `200 OK` response code and a [chatmessage](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0884b-129">例</span><span class="sxs-lookup"><span data-stu-id="0884b-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="0884b-130">要求</span><span class="sxs-lookup"><span data-stu-id="0884b-130">Request</span></span>

<span data-ttu-id="0884b-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0884b-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["303d2c1c-f1c5-40ce-b68e-544343d7f42b", "19:fec4b0f2825d4c8c82abc09027a64184@thread.skype", "1555375673184", "1555377090002"],
  "name": "get_channel_message_reply"
}-->
```http
GET https://graph.microsoft.com/beta/teams/303d2c1c-f1c5-40ce-b68e-544343d7f42b/channels/19:fec4b0f2825d4c8c82abc09027a64184@thread.skype/messages/1555375673184/replies/1555377090002
```
##### <a name="response"></a><span data-ttu-id="0884b-132">応答</span><span class="sxs-lookup"><span data-stu-id="0884b-132">Response</span></span>
<span data-ttu-id="0884b-133">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="0884b-133">Here is an example of the response.</span></span> 

><span data-ttu-id="0884b-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="0884b-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('303d2c1c-f1c5-40ce-b68e-544343d7f42b')/channels('19%3Afec4b0f2825d4c8c82abc09027a64184%40thread.skype')/messages('1555375673184')/replies/$entity",
    "id": "1555377090002",
    "replyToId": "1555375673184",
    "etag": "1555377090002",
    "messageType": "message",
    "createdDateTime": "2019-04-16T01:11:30.002Z",
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
            "id": "bb8775a4-4d8c-42cf-a1d4-4d58c2bb668f",
            "displayName": "Adele Vance",
            "userIdentityType": "aadUser"
        }
    },
    "body": {
        "contentType": "html",
        "content": "<div><div>Ah, <at id=\"0\">Megan</at>, <at id=\"1\">Alex</at>, I saw them in a separate folder. Thanks!</div>\n</div>"
    },
    "attachments": [],
    "mentions": [
        {
            "id": 0,
            "mentionText": "Megan",
            "mentioned": {
                "application": null,
                "device": null,
                "conversation": null,
                "user": {
                    "id": "5d8d505c-864f-4804-88c7-4583c966cde8",
                    "displayName": "Megan",
                    "userIdentityType": "aadUser"
                }
            }
        },
        {
            "id": 1,
            "mentionText": "Alex",
            "mentioned": {
                "application": null,
                "device": null,
                "conversation": null,
                "user": {
                    "id": "be178404-260a-4f80-b7e5-d52c1e6fdc71",
                    "displayName": "Alex",
                    "userIdentityType": "aadUser"
                }
            }
        }
    ],
    "reactions": []
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="0884b-136">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="0884b-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="0884b-137">C#</span><span class="sxs-lookup"><span data-stu-id="0884b-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_channel_message_reply-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0884b-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="0884b-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_channel_message_reply-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="0884b-139">目的-C</span><span class="sxs-lookup"><span data-stu-id="0884b-139">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_channel_message_reply-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get a reply to a channel message",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/channel-get-messagereply.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/channel-get-messagereply.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/channel-get-messagereply.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
