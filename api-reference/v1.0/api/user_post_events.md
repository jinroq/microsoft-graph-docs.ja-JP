# <a name="create-event"></a>イベントを作成する

ユーザーの既定の予定表から[イベント](../resources/event.md)を取得します。 

**start** と **end** プロパティの型が [DateTimeTimeZone](../resources/datetimetimezone.md) であるため、これらの値の一部としてイベントの開始時刻と終了時刻のそれぞれにタイム ゾーンを指定できます、 

イベントが作成されると、サーバーはすべての出席者に招待状を送信します。


## <a name="prerequisites"></a>前提条件
この API を実行するには、以下のいずれかの**スコープ**が必要です。*Calendars.ReadWrite*
## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
POST /me/events
POST /users/{id | userPrincipalName}/events

POST /me/calendar/events
POST /users/{id | userPrincipalName}/calendar/events

POST /me/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendars/{id}/events
```
## <a name="request-headers"></a>要求ヘッダー
| ヘッダー       | 値 |
|:-----------|:------|
| Authorization  | Bearer <token>. Required.  |
| Content-Type  | application/json. Required.  |

## <a name="request-body"></a>要求本文
要求本文で、[イベント](../resources/event.md) オブジェクトの JSON 表記を指定します。

**イベント** リソースは[拡張機能](../../../concepts/extensibility_overview.md)をサポートしているため、`POST` 操作を使用して、リソースの作成時にカスタム プロパティを独自のデータとともにイベントに追加することができます。

## <a name="response"></a>応答
成功した場合、このメソッドは `201, Created` 応答コードと、応答本文で[イベント](../resources/event.md) オブジェクトを返します。

## <a name="example"></a>例
##### <a name="request"></a>要求
以下は、要求の例です。
<!-- {
  "blockType": "request",
  "name": "create_event_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events
Content-type: application/json
Content-length: 285

{
  "originalStartTimeZone": "originalStartTimeZone-value",
  "originalEndTimeZone": "originalEndTimeZone-value",
  "responseStatus": {
    "response": "",
    "time": "datetime-value"
  },
  "iCalUId": "iCalUId-value",
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true
}
```
要求本文で、[イベント](../resources/event.md) オブジェクトの JSON 表記を指定します。
##### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 285

{
  "originalStartTimeZone": "originalStartTimeZone-value",
  "originalEndTimeZone": "originalEndTimeZone-value",
  "responseStatus": {
    "response": "",
    "time": "datetime-value"
  },
  "iCalUId": "iCalUId-value",
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true
}
```
## <a name="see-also"></a>関連項目

- [拡張機能を使用してカスタム データをリソースに追加する](../../../concepts/extensibility_overview.md)
- [オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)](../../../concepts/extensibility_open_users.md)
<!--
- [Add custom data to groups using schema extensions (preview)](../../../concepts/extensibility_schema_groups.md)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
