---
title: チャネルメッセージへの返信を取得する
description: チームのチャネル内のメッセージに対して1回の返信を取得します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 991adbdef3ded60726d3e3531507547db918b1cf
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32456662"
---
# <a name="get-a-reply-to-a-channel-message"></a><span data-ttu-id="e74bd-103">チャネルメッセージへの返信を取得する</span><span class="sxs-lookup"><span data-stu-id="e74bd-103">Get a reply to a channel message</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e74bd-104">チームの[チャネル](../resources/channel.md)内の[メッセージ](../resources/chatmessage.md)に対して1回の返信を取得します。</span><span class="sxs-lookup"><span data-stu-id="e74bd-104">Get a single reply to a [message](../resources/chatmessage.md) in a [channel](../resources/channel.md) of a team.</span></span>

## <a name="permissions"></a><span data-ttu-id="e74bd-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e74bd-105">Permissions</span></span>
<span data-ttu-id="e74bd-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e74bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e74bd-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e74bd-108">Permission Type</span></span>|<span data-ttu-id="e74bd-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e74bd-109">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="e74bd-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e74bd-110">Delegated (work or school account)</span></span>|<span data-ttu-id="e74bd-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e74bd-111">Group.Read.All,Group.ReadWrite.All</span></span>|
|<span data-ttu-id="e74bd-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e74bd-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e74bd-113">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="e74bd-113">Not supported</span></span>|
|<span data-ttu-id="e74bd-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e74bd-114">Application</span></span>| <span data-ttu-id="e74bd-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e74bd-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e74bd-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e74bd-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/messages/{id}/replies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e74bd-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="e74bd-117">Optional query parameters</span></span>
<span data-ttu-id="e74bd-118">[OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)は現在サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e74bd-118">The [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) are not currently supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e74bd-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e74bd-119">Request headers</span></span>
| <span data-ttu-id="e74bd-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e74bd-120">Header</span></span>       | <span data-ttu-id="e74bd-121">値</span><span class="sxs-lookup"><span data-stu-id="e74bd-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e74bd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e74bd-122">Authorization</span></span>  | <span data-ttu-id="e74bd-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e74bd-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e74bd-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="e74bd-125">Request body</span></span>
<span data-ttu-id="e74bd-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e74bd-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e74bd-127">応答</span><span class="sxs-lookup"><span data-stu-id="e74bd-127">Response</span></span>
<span data-ttu-id="e74bd-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [chatmessage](../resources/chatmessage.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="e74bd-128">If successful, this method returns a `200 OK` response code and a collection of [chatmessage](../resources/chatmessage.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e74bd-129">例</span><span class="sxs-lookup"><span data-stu-id="e74bd-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e74bd-130">要求</span><span class="sxs-lookup"><span data-stu-id="e74bd-130">Request</span></span>
<span data-ttu-id="e74bd-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e74bd-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["303d2c1c-f1c5-40ce-b68e-544343d7f42b", "19:fec4b0f2825d4c8c82abc09027a64184@thread.skype", "1555375673184", "1555377090002"],
  "name": "get_channel_message_reply"
}-->
```http
GET https://graph.microsoft.com/beta/teams/303d2c1c-f1c5-40ce-b68e-544343d7f42b/channels/19:fec4b0f2825d4c8c82abc09027a64184@thread.skype/messages/1555375673184/replies/1555377090002
```
##### <a name="response"></a><span data-ttu-id="e74bd-132">応答</span><span class="sxs-lookup"><span data-stu-id="e74bd-132">Response</span></span>
<span data-ttu-id="e74bd-133">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="e74bd-133">Here is an example of the response.</span></span> 

><span data-ttu-id="e74bd-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="e74bd-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/channel-get-messagereply.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
