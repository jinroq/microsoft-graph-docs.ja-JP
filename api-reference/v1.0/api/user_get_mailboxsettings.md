# <a name="get-user-mailbox-settings"></a>ユーザーのメールボックスの設定を取得する

ユーザーの [mailboxSettings](../resources/mailboxsettings.md) を取得します。これには、自動応答 (ユーザーが電子メールを受信したときに自動的にユーザーに通知)、ロケール (言語と国/地域)、およびタイム ゾーンの設定が含まれます。

すべてのメールボックス設定を表示することも、特定の設定を取得することもできます。

タイム ゾーンは、ユーザーが自分のメールボックスに設定できる優先設定のうちの 1 つです。 有効なタイム ゾーンの形式には、Windows タイム ゾーン形式および [Internet Assigned Numbers Authority (IANA) タイム ゾーン](http://www.iana.org/time-zones) (Olson タイム ゾーンとも呼ばれる) 形式があります。 既定値は Windows 形式です。 

ユーザーの優先タイム ゾーンを取得するとき、そのタイム ゾーンは設定された形式で返されます。 タイム ゾーンを特定の形式 (Windows または IANA) にする場合は、最初に[メールボックス設定としてその形式の優先タイム ゾーンを更新](user_update_mailboxsettings.md)します。 その後は、その形式でタイム ゾーンを取得できるようになります。 または、アプリ内で形式変換を個別に管理することもできます。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | MailboxSettings.Read、MailboxSettings.ReadWrite    |
|委任 (個人用 Microsoft アカウント) | MailboxSettings.Read、MailboxSettings.ReadWrite    |
|アプリケーション | MailboxSettings.Read、MailboxSettings.ReadWrite |

## <a name="http-request"></a>HTTP 要求
自動応答設定を含むメールボックスのすべての設定を取得するには:
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailboxSettings
GET /users/{id|userPrincipalName}/mailboxSettings
```

特定の設定 (たとえば、自動応答の設定、ロケール、またはタイム ゾーンのみ) を取得するには:
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailboxSettings/automaticRepliesSetting
GET /users/{id|userPrincipalName}/mailboxSettings/automaticRepliesSetting

GET /me/mailboxSettings/language
GET /users/{id|userPrincipalName}/mailboxSettings/language

GET /me/mailboxSettings/timeZone
GET /users/{id|userPrincipalName}/mailboxSettings/timeZone
```
## <a name="optional-query-parameters"></a>オプションのクエリ パラメーター
このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/ja-JP/graph/docs/overview/query_parameters)をサポートします。
## <a name="request-headers"></a>要求ヘッダー
| 名前       | 型 | 説明|
|:-----------|:------|:----------|
| Authorization  | string  | ベアラー {トークン}。必須。 |

## <a name="request-body"></a>要求本文
このメソッドには、要求本文を指定しません。

## <a name="response"></a>応答

成功した場合、このメソッドは `200 OK` 応答コードと、次に示す要求されたオブジェクトのいずれかを応答本文で返します。

- [mailboxSettings](../resources/mailboxsettings.md) オブジェクト
- [automaticRepliesSetting](../resources/automaticRepliesSetting.md) オブジェクト
- [localeInfo](../resources/localeinfo.md) オブジェクト
- string (**timeZone** の場合)

## <a name="example"></a>例
##### <a name="request-1"></a>要求 1
最初の例では、サインインしているユーザーのメールボックスのメールボックス設定をすべて取得します。取得する設定には、自動応答の設定、タイム ゾーン、言語設定が含まれます。
<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_1"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailboxSettings
```
##### <a name="response-1"></a>応答 1
応答には、メールボックス設定のすべてが含まれます。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailboxSettings"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/mailboxSettings",
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
    }
}
```

##### <a name="request-2"></a>要求 2
2 番目の例では、具体的にサインインしているユーザーのメールボックスの自動応答設定を取得します。
<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_2"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailboxSettings/automaticRepliesSetting
```
##### <a name="response-2"></a>応答 2
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
    "@odata.context": "https://graph.microsoft.com/api/v1.0/$metadata#Me/mailboxSettings/automaticRepliesSetting",
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get mailbox settings",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->