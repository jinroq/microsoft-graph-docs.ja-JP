---
title: ユーザーのメールボックスの設定を取得する
description: 'ユーザーの mailboxSettings を取得します。 これには、自動応答 (自動的にユーザーに通知) の設定が含まれます。 '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 296a5225ca924374a3c38242207f7f329b2e8401
ms.sourcegitcommit: 3e7769ad097e9c34233fa5fea83afa23c34e14a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/10/2019
ms.locfileid: "36822810"
---
# <a name="get-user-mailbox-settings"></a>ユーザーのメールボックスの設定を取得する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

ユーザーの [mailboxSettings](../resources/mailboxsettings.md) を取得します。 すべてのメールボックスの設定を表示するか、特定の設定を取得することができます。

ユーザーは、Outlook クライアントを使用して、メールボックスの次の設定を行うことができます。

- [自動応答](../resources/automaticrepliessetting.md)(電子メールの受信時にユーザーに自動的に通知します)
- 日付の形式
- [ロケール](../resources/localeinfo.md)(言語および国/地域)
- 時刻の形式
- タイム ゾーン
- [稼働時間](../resources/workinghours.md)

ユーザーは、web 上の Outlook を使用して、優先する日付と時刻の形式を設定できます。 ユーザーは、サポートされている[短い日付](https://docs.microsoft.com/en-us/dotnet/standard/base-types/standard-date-and-time-format-strings#ShortDate)形式または[短い時刻](https://docs.microsoft.com/en-us/dotnet/standard/base-types/standard-date-and-time-format-strings#ShortTime)形式のいずれかを選択できます。 この`GET`操作は、ユーザーが選択した形式を返します。

ユーザーは、自分のメールボックスサーバーに対して管理者が設定した[サポートさ](outlookuser-supportedtimezones.md)れているタイムゾーンから選択することによって、任意の Outlook クライアントのタイムゾーンを設定できます。 管理者は、Windows タイムゾーン形式または[インターネット割り当て番号証明機関 (IANA) タイム](https://www.iana.org/time-zones)ゾーン (olson タイムゾーンとも呼ばれる) 形式でタイムゾーンを設定できます。 既定値は Windows 形式です。 

この`GET`操作は、管理者が設定した形式でユーザーの優先タイムゾーンを返します。 タイム ゾーンを特定の形式 (Windows または IANA) にする場合は、最初に[メールボックス設定としてその形式の優先タイム ゾーンを更新](user-update-mailboxsettings.md)します。 その後は、その形式でタイム ゾーンを取得できるようになります。 または、アプリ内で形式変換を個別に管理することもできます。 

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | MailboxSettings.Read、MailboxSettings.ReadWrite    |
|委任 (個人用 Microsoft アカウント) | MailboxSettings.Read、MailboxSettings.ReadWrite    |
|アプリケーション | MailboxSettings.Read、MailboxSettings.ReadWrite |

## <a name="http-request"></a>HTTP 要求
ユーザーのすべてのメールボックス設定を取得するには、次のようにします。
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailboxSettings
GET /users/{id|userPrincipalName}/mailboxSettings
```

特定の設定を取得するには、自動応答の設定、ロケール、タイムゾーン、または稼働時間のみを取得します。
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailboxSettings/automaticRepliesSetting
GET /users/{id|userPrincipalName}/mailboxSettings/automaticRepliesSetting

GET /me/mailboxSettings/dateFormat
GET /users/{id|userPrincipalName}/mailboxSettings/dateFormat

GET /me/mailboxSettings/language
GET /users/{id|userPrincipalName}/mailboxSettings/language

GET /me/mailboxSettings/timeFormat
GET /users/{id|userPrincipalName}/mailboxSettings/timeFormat

GET /me/mailboxSettings/timeZone
GET /users/{id|userPrincipalName}/mailboxSettings/timeZone

GET /me/mailboxSettings/workingHours
GET /users/{id|userPrincipalName}/mailboxSettings/workingHours
```
## <a name="optional-query-parameters"></a>オプションのクエリ パラメーター
このメソッドは、応答をカスタマイズするための[OData クエリパラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)の一部をサポートしています。
## <a name="request-headers"></a>要求ヘッダー
| 名前       | 型 | 説明|
|:-----------|:------|:----------|
| Authorization  | string  | ベアラー {トークン}。必須。 |

## <a name="request-body"></a>要求本文
このメソッドには、要求本文を指定しません。

## <a name="response"></a>応答

成功した場合、このメソッドは `200 OK` 応答コードと、次に示す要求されたオブジェクトのいずれかを応答本文で返します。

- [mailboxSettings](../resources/mailboxsettings.md) オブジェクト
- [automaticRepliesSetting](../resources/automaticrepliessetting.md) オブジェクト
- string ( **dateFormat**の場合)
- [localeInfo](../resources/localeinfo.md) オブジェクト
- string ( **Timeformat**)
- string (**timeZone** の場合)
- [workingHours](../resources/workinghours.md)

## <a name="examples"></a>例

### <a name="example-1"></a>例 1
#### <a name="request"></a>要求 
最初の例では、サインインしているユーザーのメールボックスのすべてのメールボックス設定を取得します。これには自動応答、日付形式、ロケール (言語と国/地域)、時間の形式、タイムゾーン、および稼働時間の設定が含まれます。

# <a name="httptabhttp"></a>[プロトコル](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/mailboxSettings
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mailboxsettings-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mailboxsettings-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[目的-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mailboxsettings-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>応答
応答には、サインインしているユーザーのすべてのメールボックス設定が含まれます。 注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。 実際の呼び出しではすべてのプロパティが返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailboxSettings"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/mailboxSettings",
    "automaticRepliesSetting": {
        "status": "Scheduled",
        "externalAudience": "All",
        "scheduledStartDateTime": {
            "dateTime": "2016-03-14T07:00:00.0000000",
            "timeZone": "UTC"
        },
        "scheduledEndDateTime": {
            "dateTime": "2016-03-28T07:00:00.0000000",
            "timeZone": "UTC"
        },
        "internalReplyMessage": "<html>\n<body>\n<p>I'm at our company's worldwide reunion and will respond to your message as soon as I return.<br>\n</p></body>\n</html>\n",
        "externalReplyMessage": "<html>\n<body>\n<p>I'm at the Contoso worldwide reunion and will respond to your message as soon as I return.<br>\n</p></body>\n</html>\n"
    },
    "timeZone":"UTC",
    "language":{
      "locale":"en-US",
      "displayName":"English (United States)"
    },
    "workingHours":{
        "daysOfWeek":[
            "monday",
            "tuesday",
            "wednesday",
            "thursday",
            "friday"
        ],
        "startTime":"08:00:00.0000000",
        "endTime":"17:00:00.0000000",
        "timeZone":{
            "name":"Pacific Standard Time"
        }
    },
    "dateFormat": "MM/dd/yyyy",
    "timeFormat": "hh:mm tt"
}
```

### <a name="example-2"></a>例 2
#### <a name="request"></a>要求
2 番目の例では、具体的にサインインしているユーザーのメールボックスの自動応答設定を取得します。

# <a name="httptabhttp"></a>[プロトコル](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/mailboxSettings/automaticRepliesSetting
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mailboxsettings-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mailboxsettings-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[目的-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mailboxsettings-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>応答
この応答には自動とうとう設定のみが含まれます。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.automaticRepliesSetting"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/mailboxSettings/automaticRepliesSetting",
    "status": "alwaysEnabled",
    "externalAudience": "None",
    "scheduledStartDateTime": {
        "dateTime": "2016-03-19T02:00:00.0000000",
        "timeZone": "UTC"
    },
    "scheduledEndDateTime": {
        "dateTime": "2016-03-20T02:00:00.0000000",
        "timeZone": "UTC"
    },
    "internalReplyMessage": "<html>\n<body>\n<p>I'm at our company's worldwide reunion and will respond to your message as soon as I return.<br>\n</p></body>\n</html>\n",
    "externalReplyMessage": "<html>\n<body>\n<p>I'm at the Contoso worldwide reunion and will respond to your message as soon as I return.<br>\n</p></body>\n</html>\n"
}
```

### <a name="example-3"></a>例 3
#### <a name="request"></a>要求
3 番目の例では、サインインしているユーザーのメールボックスの自動応答の設定を具体的に指定して取得します。
<!-- {
  "blockType": "ignored",
  "name": "get_mailboxsettings_3"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailboxSettings/workingHours
```
#### <a name="response"></a>応答
この応答には、自動応答の設定のみが含まれます。 ユーザーの就業時間には、[カスタム タイム ゾーン](../resources/customtimezone.md)が適用されていることに注意してください。 注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。 実際の呼び出しではすべてのプロパティが返されます。
<!-- {
  "blockType": "ignored",
  "name": "get_mailboxsettings_3",
  "truncated": true,
  "@odata.type": "microsoft.graph.workingHours"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('94447c6e-ea4c-494c-a9ed-d905e366c5cb')/mailboxSettings/workingHours",
    "daysOfWeek":[
        "monday",
        "tuesday",
        "wednesday",
        "thursday",
        "friday",
        "saturday"
    ],
    "startTime":"09:00:00.0000000",
    "endTime":"18:30:00.0000000",
    "timeZone":{
        "@odata.type":"#microsoft.graph.customTimeZone",
        "bias":-200,
        "name":"Customized Time Zone",
        "standardOffset":{
            "time":"02:00:00.0000000",
            "dayOccurrence":4,
            "dayOfWeek":"sunday",
            "month":5,
            "year":0
        },
        "daylightOffset":{
            "daylightBias":-100,
            "time":"02:00:00.0000000",
            "dayOccurrence":2,
            "dayOfWeek":"sunday",
            "month":10,
            "year":0
        }
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get mailbox settings",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
