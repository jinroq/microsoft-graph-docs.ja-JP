# <a name="add-attachment"></a>添付ファイルを追加する

[添付ファイル](../resources/attachment.md)をイベントに追加する場合に、この API を使用します。現在、各 REST 要求の合計サイズは 4 MB に制限されているため、追加できる添付ファイルのサイズは 4 MB 未満に制限されます。
## <a name="prerequisites"></a>前提条件
この API を実行するには、以下のいずれかの**スコープ**が必要です。*Calendars.ReadWrite*
## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
ユーザーまたはグループの既定の[カレンダー](../resources/calendar.md)内の[イベント](../resources/event.md)の添付ファイル。
```http
POST /me/events/{id}/attachments
POST /users/{id | userPrincipalName}/events/{id}/attachments
POST /groups/{id}/events/{id}/attachments

POST /me/calendar/events/{id}/attachments
POST /users/{id | userPrincipalName}/calendar/events/{id}/attachments
POST /groups/{id}/calendar/events/{id}/attachments
```
ユーザーの既定 [calendarGroup](../resources/calendargroup.md) に属する[カレンダー](../resources/calendar.md)内[イベント](../resources/event.md)の添付ファイル。
```http
POST /me/calendars/{id}/events/{id}/attachments
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/attachments

POST /me/calendargroup/calendars/{id}/events/{id}/attachments
POST /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/attachments
```
ユーザーの [calendarGroup](../resources/calendargroup.md) に属する[カレンダー](../resources/calendar.md)内[イベント](../resources/event.md)の添付ファイル。
```http
POST /me/calendargroups/{id}/calendars/{id}/events/{id}/attachments
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/attachments
```
## <a name="request-headers"></a>要求ヘッダー
| 名前       | 型 | 説明|
|:---------------|:--------|:----------|
| Authorization  | string  | Bearer <token>. Required. |
| Content-Type | string  | エンティティ本文内のデータの性質です。必須。 |

## <a name="request-body"></a>要求本文
要求本文で、[Attachment](../resources/attachment.md) オブジェクトの JSON 表記を指定します。


## <a name="response"></a>応答
成功した場合、このメソッドは `201, Created` 応答コードと、応答本文で [Attachment](../resources/attachment.md) オブジェクトを返します。

## <a name="example-file-attachment"></a>例 (添付ファイル)

##### <a name="request"></a>要求
以下は、要求の例です。
<!-- {
  "blockType": "request",
  "name": "create_file_attachment_from_event"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/attachments
Content-type: application/json
Content-length: 142

{
  "@odata.type": "#microsoft.graph.fileAttachment",
  "name": "name-value",
  "contentBytes": "contentBytes-value"
}
```

要求本文で、[Attachment](../resources/attachment.md) オブジェクトの JSON 表記を指定します。

##### <a name="response"></a>応答
以下は、応答の例です。
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP 200 OK
```

## <a name="example-item-attachment"></a>例 (項目の添付ファイル)

##### <a name="request"></a>要求

以下は、要求の例です。

<!-- {
  "blockType": "request",
  "name": "create_item_attachment_from_event"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events/{id}/attachments
Content-type: application/json
Content-length: 100

{
  "@odata.type": "#microsoft.graph.itemAttachment",
  "name": "name-value",
  "item": {}
}
```

##### <a name="response"></a>応答
以下は、応答の例です。
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
