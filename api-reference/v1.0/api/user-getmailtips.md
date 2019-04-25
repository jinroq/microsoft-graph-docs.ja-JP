---
title: 'ユーザー: getmailtips ヒント'
description: サインインしているユーザーが使用できる1人以上の受信者のメールヒントを取得します。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4c931d6e7f3b7762534d773b647f7db68461a230
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32567866"
---
# <a name="user-getmailtips"></a>ユーザー: getmailtips ヒント

サインインしている[ユーザー](../resources/user.md)が使用できる1人以上の受信者のメールヒントを取得します。

`getMailTips`アクションを`POST`呼び出すことによって、複数の受信者に対して特定の種類のメールヒントが一度に返されるように要求することができることに注意してください。 要求されたメールヒントが[メールヒント](../resources/mailtips.md)コレクションに返されます。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | メール。読み取り、共有    |
|委任 (個人用 Microsoft アカウント) | Mail.Read    |
|アプリケーション | Mail.Read |

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMailTips
POST /users/{id|userPrincipalName}/getMailTips
```
## <a name="optional-query-parameters"></a>オプションのクエリ パラメーター
このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。
## <a name="request-headers"></a>要求ヘッダー
| ヘッダー       | 値|
|:-----------  |:------|
| Authorization | ベアラー {トークン}。必須。 |
| Content-Type  | application/json  |

## <a name="request-body"></a>要求本文
要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。

| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|EmailAddresses|String collection|メール ヒントを取得する受信者の SMTP アドレスのコレクションです。|
|MailTipsOptions|String|要求されたメールヒントを表すフラグの列挙。 可能な値は`automaticReplies`、 `customMailTip`、 `deliveryRestriction` `externalMemberCount` `mailboxFullStatus` `maxMessageSize` `moderationStatus` `recipientScope`、、、、、、、、および`totalMemberCount` `recipientSuggestions`です。|

## <a name="response"></a>応答

成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[メールヒント](../resources/mailtips.md)オブジェクトのコレクションを返します。
## <a name="example"></a>例
##### <a name="request"></a>要求
次の例では、指定された受信者のメールヒントを取得します。すべての自動応答の設定と、メールボックスの状態が [完全] になっています。

<!-- {
  "blockType": "request",
  "name": "user_getmailtips"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/getMailTips
Content-Type: application/json

{
    "EmailAddresses": [
        "danas@contoso.onmicrosoft.com", 
        "fannyd@contoso.onmicrosoft.com"
    ],
    "MailTipsOptions": "automaticReplies, mailboxFullStatus"
}
```

##### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailTips",
  isCollection: true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Collection(microsoft.graph.mailTips)",
    "value":[
        {
            "emailAddress":{
                "name":"",
                "address":"danas@contoso.onmicrosoft.com"
            },
            "automaticReplies":{
                "message":"<style type=\"text/css\" style=\"\">\r\n<!--\r\np\r\n\t{margin-top:0;\r\n\tmargin-bottom:0}\r\n-->\r\n</style>\r\n<div dir=\"ltr\">\r\n<div id=\"x_divtagdefaultwrapper\" style=\"font-size:12pt; color:#000000; background-color:#FFFFFF; font-family:Calibri,Arial,Helvetica,sans-serif\">\r\n<p>Hi, I am on vacation right now. I'll get back to you after I return.<br>\r\n</p>\r\n</div>\r\n</div>",
                "messageLanguage":{
                    "locale":"en-US",
                    "displayName":"English (United States)"
                },
                "scheduledStartTime": {
                    "dateTime": "2018-08-07T02:00:00.0000000",
                    "timeZone": "UTC"
                },
                "scheduledEndTime": {
                    "dateTime": "2018-08-09T02:00:00.0000000",
                    "timeZone": "UTC"
                }
            },
            "mailboxFull":false
        },
        {
            "emailAddress":{
                "name":"",
                "address":"fannyd@contoso.onmicrosoft.com"
            },
            "automaticReplies":{
                "message":""
            },
            "mailboxFull":false
        }
    ]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: getMailTips",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
