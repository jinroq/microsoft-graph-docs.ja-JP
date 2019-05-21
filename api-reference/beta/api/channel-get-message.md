---
title: チャネル メッセージを取得する
description: チームのチャネルで単一のメッセージを取得します (返信なしで)。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 48ff7af72e630973ef120808e407cce44d379f2b
ms.sourcegitcommit: abca7fcefeaa74b50f4600b35d816b626ba08468
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/21/2019
ms.locfileid: "34310812"
---
# <a name="get-channel-message"></a>チャネル メッセージを取得する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

チームの[チャネル](../resources/channel.md)で単一の[メッセージ](../resources/chatmessage.md)を取得します (返信なしで)。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類|アクセス許可 (特権の小さいものから大きいものへ)|
|---------|-------------|
|委任 (職場または学校のアカウント)|Group.Read.All、Group.ReadWrite.All|
|委任 (個人用 Microsoft アカウント)|サポートされていません|
|アプリケーション| サポートされていません。 |

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/messages/{id}
```

## <a name="optional-query-parameters"></a>オプションのクエリ パラメーター
[OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)は現在サポートされていません。

## <a name="request-headers"></a>要求ヘッダー
| ヘッダー       | 値 |
|:---------------|:--------|
| Authorization  | ベアラー {トークン}。必須。  |

## <a name="request-body"></a>要求本文
このメソッドには、要求本文を指定しません。

## <a name="response"></a>応答

成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [chatmessage](../resources/chatmessage.md) オブジェクトを返します。

## <a name="example"></a>例
##### <a name="request"></a>要求
以下は、要求の例です。
<!-- {
  "blockType": "request",
  "sampleKeys": ["303d2c1c-f1c5-40ce-b68e-544343d7f42b", "19:fec4b0f2825d4c8c82abc09027a64184@thread.skype", "1555375673184"],
  "name": "get_channel_message"
}-->
```http
GET https://graph.microsoft.com/beta/teams/303d2c1c-f1c5-40ce-b68e-544343d7f42b/channels/19:fec4b0f2825d4c8c82abc09027a64184@thread.skype/messages/1555375673184
```
##### <a name="response"></a>応答
以下は、応答の例です。 

>**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されています。 実際の呼び出しではすべてのプロパティが返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('303d2c1c-f1c5-40ce-b68e-544343d7f42b')/channels('19%3Afec4b0f2825d4c8c82abc09027a64184%40thread.skype')/messages/$entity",
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
    "webUrl": "https://teams.microsoft.com/l/message/19%3Afec4b0f2825d4c8c82abc09027a64184%40thread.skype/1555375673184?groupId=303d2c1c-f1c5-40ce-b68e-544343d7f42b&tenantId=123d12b3-1234-12ab-b1a2-123ba45c6789&createdTime=1555375673184&parentMessageId=1555375673188",       
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
    "reactions": [
      {
        "reactionType": "like",
        "user": {
            "id": "5d8d505c-864f-4804-88c7-4583c966cde8",
            "displayName": "Megan Bowen",
            "userIdentityType": "aadUser"
        },
        "createdDateTime": "2019-04-16T00:58:53.184Z"
      }
    ]
}
```
#### <a name="sdk-sample-code"></a>SDK サンプル コード
# <a name="ctabcs"></a>[C#](#tab/cs)
[!INCLUDE [sample-code](../includes/get_channel_message-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_channel_message-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get channel message",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/channel-get-message.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/channel-get-message.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
