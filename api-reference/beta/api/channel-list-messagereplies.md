---
title: チャネルメッセージの返信を一覧表示する
description: チームのチャネル内のメッセージのすべての返信を一覧表示します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 5a8968561b0ec6d4bdb38b531d8ce286c1857b11
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35262105"
---
# <a name="list-channel-message-replies"></a><span data-ttu-id="8cd0c-103">チャネルメッセージの返信を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="8cd0c-103">List channel message replies</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8cd0c-104">チームの[チャネル](../resources/channel.md)内の[メッセージ](../resources/chatmessage.md)のすべての返信を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="8cd0c-104">List all the replies of a [message](../resources/chatmessage.md) in a [channel](../resources/channel.md) of a team.</span></span>

<span data-ttu-id="8cd0c-105">このメソッドは、指定されたメッセージの返信のみを一覧表示します (存在する場合)。</span><span class="sxs-lookup"><span data-stu-id="8cd0c-105">This method lists only the replies of the specified message, if any.</span></span> <span data-ttu-id="8cd0c-106">メッセージ自体を取得するには、単に [[チャネルの取得] メッセージ](channel-get-message.md)を呼び出します。</span><span class="sxs-lookup"><span data-stu-id="8cd0c-106">To get the message itself, simply call [get channel message](channel-get-message.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8cd0c-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8cd0c-107">Permissions</span></span>
<span data-ttu-id="8cd0c-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8cd0c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8cd0c-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8cd0c-110">Permission Type</span></span>|<span data-ttu-id="8cd0c-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8cd0c-111">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="8cd0c-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8cd0c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8cd0c-113">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8cd0c-113">Group.Read.All,Group.ReadWrite.All</span></span>|
|<span data-ttu-id="8cd0c-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8cd0c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8cd0c-115">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="8cd0c-115">Not supported</span></span>|
|<span data-ttu-id="8cd0c-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8cd0c-116">Application</span></span>| <span data-ttu-id="8cd0c-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8cd0c-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8cd0c-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8cd0c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/messages/{id}/replies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8cd0c-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="8cd0c-119">Optional query parameters</span></span>

<span data-ttu-id="8cd0c-120">[$top](/graph/query-parameters#top-parameter)クエリ パラメーターで応答ごとのアイテム数を制御することができます。</span><span class="sxs-lookup"><span data-stu-id="8cd0c-120">You can use the [$top](/graph/query-parameters#top-parameter) query parameter to control the number of items per response.</span></span> <span data-ttu-id="8cd0c-121">その他の[OData クエリ パラメーター](/graph/query-parameters)は現在サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8cd0c-121">The other [OData query parameters](/graph/query-parameters) are not currently supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8cd0c-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8cd0c-122">Request headers</span></span>
| <span data-ttu-id="8cd0c-123">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8cd0c-123">Header</span></span>       | <span data-ttu-id="8cd0c-124">値</span><span class="sxs-lookup"><span data-stu-id="8cd0c-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8cd0c-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="8cd0c-125">Authorization</span></span>  | <span data-ttu-id="8cd0c-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8cd0c-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8cd0c-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="8cd0c-128">Request body</span></span>
<span data-ttu-id="8cd0c-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="8cd0c-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8cd0c-130">応答</span><span class="sxs-lookup"><span data-stu-id="8cd0c-130">Response</span></span>
<span data-ttu-id="8cd0c-131">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [chatmessage](../resources/channel.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="8cd0c-131">If successful, this method returns a `200 OK` response code and a collection of [chatmessage](../resources/channel.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8cd0c-132">例</span><span class="sxs-lookup"><span data-stu-id="8cd0c-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8cd0c-133">要求</span><span class="sxs-lookup"><span data-stu-id="8cd0c-133">Request</span></span>
<span data-ttu-id="8cd0c-134">この例では、指定されたメッセージに2つの応答があります。</span><span class="sxs-lookup"><span data-stu-id="8cd0c-134">In this example, the specified message has two replies.</span></span> <span data-ttu-id="8cd0c-135">各返信には、1つ以上の[chatMessageMention](../resources/chatmessagemention.md)オブジェクトがあります。</span><span class="sxs-lookup"><span data-stu-id="8cd0c-135">Each reply has one or more [chatMessageMention](../resources/chatmessagemention.md) objects.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["303d2c1c-f1c5-40ce-b68e-544343d7f42b", "19:fec4b0f2825d4c8c82abc09027a64184@thread.skype", "1555375673184"],
  "name": "get_channel_message_replies"
}-->
```http
GET https://graph.microsoft.com/beta/teams/303d2c1c-f1c5-40ce-b68e-544343d7f42b/channels/19:fec4b0f2825d4c8c82abc09027a64184@thread.skype/messages/1555375673184/replies
```
##### <a name="response"></a><span data-ttu-id="8cd0c-136">応答</span><span class="sxs-lookup"><span data-stu-id="8cd0c-136">Response</span></span>
<span data-ttu-id="8cd0c-137">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="8cd0c-137">Here is an example of the response.</span></span> 

><span data-ttu-id="8cd0c-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="8cd0c-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('303d2c1c-f1c5-40ce-b68e-544343d7f42b')/channels('19%3Afec4b0f2825d4c8c82abc09027a64184%40thread.skype')/messages('1555375673184')/replies",
    "@odata.count": 2,
    "value": [
        {
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
        },
        {
            "id": "1555375848360",
            "replyToId": "1555375673184",
            "etag": "1555375848360",
            "messageType": "message",
            "createdDateTime": "2019-04-16T00:50:48.36Z",
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
                "content": "<div><div>And, <at id=\"0\">Alex Wilber</at>, can we see the February report as well?</div>\n</div>"
            },
            "attachments": [],
            "mentions": [
                {
                    "id": 0,
                    "mentionText": "Alex Wilber",
                    "mentioned": {
                        "application": null,
                        "device": null,
                        "conversation": null,
                        "user": {
                            "id": "be178404-260a-4f80-b7e5-d52c1e6fdc71",
                            "displayName": "Alex Wilber",
                            "userIdentityType": "aadUser"
                        }
                    }
                }
            ],
            "reactions": []
        }
    ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="8cd0c-140">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="8cd0c-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="8cd0c-141">C#</span><span class="sxs-lookup"><span data-stu-id="8cd0c-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_channel_message_replies-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8cd0c-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="8cd0c-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_channel_message_replies-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="8cd0c-143">目的-C</span><span class="sxs-lookup"><span data-stu-id="8cd0c-143">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_channel_message_replies-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List channel message replies",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/channel-list-messagereplies.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/channel-list-messagereplies.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/channel-list-messagereplies.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
