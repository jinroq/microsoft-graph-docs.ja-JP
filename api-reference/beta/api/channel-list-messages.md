---
title: チャネル メッセージを一覧表示する
description: 'チームのチャネルに含まれるメッセージの一覧を取得します (返信なし)。 メッセージの返信を取得するには、メッセージの返信一覧 API またはメッセージの返信取得 API を呼び出します。 '
localization_priority: Priority
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: f482222d1eb6c672d97109a9cc7d6f6d9c838a5e
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33635597"
---
# <a name="list-channel-messages"></a><span data-ttu-id="d1ef3-104">チャネル メッセージを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="d1ef3-104">List channel messages</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d1ef3-105">[チーム](../resources/team.md)の[チャネル](../resources/channel.md)で[メッセージ](../resources/chatmessage.md)の一覧を取得します (返信なし)。</span><span class="sxs-lookup"><span data-stu-id="d1ef3-105">Retrieve the list of [messages](../resources/chatmessage.md) (without the replies) in a [channel](../resources/channel.md) of a [team](../resources/team.md).</span></span> 

<span data-ttu-id="d1ef3-106">メッセージの返信を取得するには、[メッセージの返信一覧](channel-get-messagereply.md) API または [メッセージの返信取得](channel-list-messagereplies.md) API を呼び出します。</span><span class="sxs-lookup"><span data-stu-id="d1ef3-106">To get the replies for a message, call the [list message replies](channel-get-messagereply.md) or the [get message reply](channel-list-messagereplies.md) API.</span></span> 

## <a name="permissions"></a><span data-ttu-id="d1ef3-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d1ef3-107">Permissions</span></span>

<span data-ttu-id="d1ef3-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d1ef3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1ef3-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d1ef3-110">Permission Type</span></span>|<span data-ttu-id="d1ef3-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d1ef3-111">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="d1ef3-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d1ef3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d1ef3-113">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1ef3-113">Group.Read.All,Group.ReadWrite.All</span></span>|
|<span data-ttu-id="d1ef3-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d1ef3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d1ef3-115">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="d1ef3-115">Not supported</span></span>|
|<span data-ttu-id="d1ef3-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d1ef3-116">Application</span></span>| <span data-ttu-id="d1ef3-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d1ef3-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d1ef3-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d1ef3-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/messages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d1ef3-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="d1ef3-119">Optional query parameters</span></span>

<span data-ttu-id="d1ef3-120">[$top](/graph/query-parameters#top-parameter)クエリ パラメーターで応答ごとのアイテム数を制御することができます。</span><span class="sxs-lookup"><span data-stu-id="d1ef3-120">You can use the [$top](/graph/query-parameters#top-parameter) query parameter to control the number of items per response.</span></span> <span data-ttu-id="d1ef3-121">その他の[OData クエリ パラメーター](/graph/query-parameters)は現在サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d1ef3-121">The other [OData query parameters](/graph/query-parameters) are not currently supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d1ef3-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d1ef3-122">Request headers</span></span>

| <span data-ttu-id="d1ef3-123">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d1ef3-123">Header</span></span>       | <span data-ttu-id="d1ef3-124">値</span><span class="sxs-lookup"><span data-stu-id="d1ef3-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d1ef3-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="d1ef3-125">Authorization</span></span>  | <span data-ttu-id="d1ef3-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d1ef3-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d1ef3-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="d1ef3-128">Request body</span></span>

<span data-ttu-id="d1ef3-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d1ef3-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d1ef3-130">応答</span><span class="sxs-lookup"><span data-stu-id="d1ef3-130">Response</span></span>

<span data-ttu-id="d1ef3-131">このメソッドは、成功すると `200 OK` 応答コードと [chatMessage](../resources/chatmessage.md) オブジェクトのコレクションを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="d1ef3-131">If successful, this method returns a `200 OK` response code and a collection of [chatMessage](../resources/chatmessage.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d1ef3-132">例</span><span class="sxs-lookup"><span data-stu-id="d1ef3-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d1ef3-133">要求</span><span class="sxs-lookup"><span data-stu-id="d1ef3-133">Request</span></span>

<span data-ttu-id="d1ef3-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d1ef3-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["303d2c1c-f1c5-40ce-b68e-544343d7f42b", "19:fec4b0f2825d4c8c82abc09027a64184@thread.skype"],
  "name": "get_channel_messages"
}-->
```http
GET https://graph.microsoft.com/beta/teams/303d2c1c-f1c5-40ce-b68e-544343d7f42b/channels/19:fec4b0f2825d4c8c82abc09027a64184@thread.skype/messages
```
##### <a name="response"></a><span data-ttu-id="d1ef3-135">応答</span><span class="sxs-lookup"><span data-stu-id="d1ef3-135">Response</span></span>
<span data-ttu-id="d1ef3-136">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="d1ef3-136">Here is an example of the response.</span></span> 

><span data-ttu-id="d1ef3-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="d1ef3-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('303d2c1c-f1c5-40ce-b68e-544343d7f42b')/channels('19%3Afec4b0f2825d4c8c82abc09027a64184%40thread.skype')/messages",
    "@odata.count": 3,
    "value": [
        {
            "id": "1555375673184",
            "replyToId": null,
            "etag": "1555375673184",
            "messageType": "message",
            "createdDateTime": "2019-04-16T00:47:53.184Z",
            "lastModifiedDateTime": null,
            "deletedDateTime": null,
            "subject": "",
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
                "content": "<div><div>Nice to join this team. <at id=\"0\">Megan Bowen</at>, have we got the March report ready please?</div>\n</div>"
            },
            "attachments": [],
            "mentions": [
                {
                    "id": 0,
                    "mentionText": "Megan Bowen",
                    "mentioned": {
                        "application": null,
                        "device": null,
                        "conversation": null,
                        "user": {
                            "id": "5d8d505c-864f-4804-88c7-4583c966cde8",
                            "displayName": "Megan Bowen",
                            "userIdentityType": "aadUser"
                        }
                    }
                }
            ],
            "reactions": []
        },
        {
            "id": "1548100551644",
            "replyToId": null,
            "etag": "1548100551893",
            "messageType": "message",
            "createdDateTime": "2019-01-21T19:55:51.644Z",
            "lastModifiedDateTime": null,
            "deletedDateTime": null,
            "subject": "",
            "summary": null,
            "importance": "normal",
            "locale": "en-us",
            "policyViolation": null,
            "from": {
                "application": null,
                "device": null,
                "conversation": null,
                "user": {
                    "id": "c651e5be-7631-42ad-99c6-12c59def11fb",
                    "displayName": "Miriam Graham",
                    "userIdentityType": "aadUser"
                }
            },
            "body": {
                "contentType": "html",
                "content": "<div>I've added an Excel tab to the channel containing the P&amp;L Summary. \r\n<div style=\"display:inline\"><at id=\"0\">Isaiah Langer</at></div> and team, please review the Sale Summary tab in particular, and make any necessary updates.</div>"
            },
            "attachments": [],
            "mentions": [
                {
                    "id": 0,
                    "mentionText": "Isaiah Langer",
                    "mentioned": {
                        "application": null,
                        "device": null,
                        "conversation": null,
                        "user": {
                            "id": "b525e831-bd00-45e5-860c-a4329ef5f5d8",
                            "displayName": "Isaiah Langer",
                            "userIdentityType": "aadUser"
                        }
                    }
                }
            ],
            "reactions": [
                {
                    "reactionType": "like",
                    "createdDateTime": "2019-01-21T19:55:51.893Z",
                    "user": {
                        "application": null,
                        "device": null,
                        "conversation": null,
                        "user": {
                            "id": "e1ecb745-c10f-40af-a9d4-cab946c80ac7",
                            "displayName": null,
                            "userIdentityType": "aadUser"
                        }
                    }
                }
            ]
        },
        {
            "id": "1548100547534",
            "replyToId": null,
            "etag": "1548100547534",
            "messageType": "message",
            "createdDateTime": "2019-01-21T19:55:47.534Z",
            "lastModifiedDateTime": null,
            "deletedDateTime": null,
            "subject": "",
            "summary": null,
            "importance": "high",
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
                "content": "<div>Just a reminder to everyone to please update your monthly reports by this Friday!</div>"
            },
            "attachments": [],
            "mentions": [],
            "reactions": []
        }
    ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="d1ef3-139">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="d1ef3-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d1ef3-140">C#</span><span class="sxs-lookup"><span data-stu-id="d1ef3-140">c</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_channel_messages-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d1ef3-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="d1ef3-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_channel_messages-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List channel messages",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/channel-list-messages.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/channel-list-messages.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
