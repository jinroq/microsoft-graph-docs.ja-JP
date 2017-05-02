# <a name="get-attachment"></a>添付ファイルを取得する

[イベント](../resources/event.md)、[メッセージ](../resources/message.md)、または[投稿](../resources/post.md)に添付されている添付ファイルのプロパティとリレーションシップを読み取ります。 

添付ファイルには、次の種類のいずれかを指定できます。

* ファイル ([fileAttachment](../resources/fileattachment.md) リソース)
* 項目 ([itemAttachment](../resources/itemattachment.md) リソースで表される連絡先、イベント、またはメッセージ)
* ファイルへのリンク ([referenceAttachment](../resources/referenceAttachment.md) リソース)

これらの添付ファイル リソースのすべての種類は、[attachment](../resources/attachment.md) リソースから派生します。 

## <a name="prerequisites"></a>前提条件
この API を実行するには、以下のいずれかの**スコープ**が必要です。

* メッセージの添付ファイルにアクセスする場合:*Mail.Read*
* イベントの添付ファイルにアクセスする場合:*Calendars.Read*
* グループ イベントおよび投稿の添付ファイルにアクセスする場合:*Group.Read.All*

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
ユーザーまたはグループの既定の[カレンダー](../resources/calendar.md)内の[イベント](../resources/event.md)の添付ファイル。
```http
GET /me/events/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/events/{id}/attachments/{id}
GET /groups/{id}/events/{id}/attachments/{id}

GET /me/calendar/{id}/events/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/calendar/events/{id}/attachments/{id}
GET /groups/{id}/calendar/events/{id}/attachments/{id}
```
ユーザーの既定 [calendarGroup](../resources/calendargroup.md) に属する[カレンダー](../resources/calendar.md)内[イベント](../resources/event.md)の添付ファイル。
```http
GET /me/calendars/{id}/events/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/calendars/{id}/events/{id}/attachments/{id}

GET /me/calendargroup/calendars/{id}/events/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/attachments/{id}
```
ユーザーの [calendarGroup](../resources/calendargroup.md) に属する[カレンダー](../resources/calendar.md)内[イベント](../resources/event.md)の添付ファイル。
```http
GET /me/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}
```
ユーザーのメールボックス内の[メッセージ](../resources/message.md)の添付ファイル。
```http
GET /me/messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/messages/{id}/attachments/{id}
```
ユーザーのメールボックスの最上位レベルの [mailFolder](../resources/mailfolder.md) に含まれている[メッセージ](../resources/message.md)の添付ファイル。
```http
GET /me/mailFolders/{id}/messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments/{id}
```
ユーザーのメールボックスの [mailFolder](../resources/mailfolder.md) の子フォルダーに含まれている[メッセージ](../resources/message.md)の添付ファイル。次の例は、入れ子のレベルの 1 つを示していますが、メッセージは子の子などに入れることができます。
```http
GET /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```
グループの[会話](../resources/conversation.md)に属する[スレッド](../resources/conversationthread.md)内の[投稿](../resources/post.md)の添付ファイル。
```http
GET /groups/{id}/threads/{id}/posts/{id}/attachments/{id}
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments/{id}
```
## <a name="optional-query-parameters"></a>オプションのクエリ パラメーター
このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。
## <a name="request-headers"></a>要求ヘッダー
| 名前       | 型 | 説明|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer <token>. Required. |

## <a name="request-body"></a>要求本文
このメソッドには、要求本文を指定しません。
## <a name="response"></a>応答
成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Attachment](../resources/attachment.md) オブジェクトを返します。

## <a name="example-file-attachment"></a>例 (添付ファイル)

##### <a name="request"></a>要求
以下は、イベントの添付ファイルを取得する要求の例です。
<!-- {
  "blockType": "request",
  "name": "get_file_attachment"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/events/{id}/attachments/{id}
```

##### <a name="response"></a>応答
以下は、応答の例です。注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。実際の呼び出しではすべてのプロパティが返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.fileAttachment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 199

{
  "@odata.type": "#microsoft.graph.fileAttachment",
  "contentType": "contentType-value",
  "contentLocation": "contentLocation-value",
  "contentBytes": "contentBytes-value",
  "contentId": "null",
  "lastModifiedDateTime": "2016-01-01T12:00:00Z",
  "id": "id-value",
  "isInline": false,
  "name": "name-value",
  "size": 99
}
```
## <a name="example-item-attachment"></a>例 (項目の添付ファイル)

##### <a name="request"></a>要求
以下は、イベントの項目の添付ファイルを取得する要求の例です。
<!-- {
  "blockType": "request",
  "name": "get_item_attachment"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/events/{id}/attachments/{id}
```

##### <a name="response"></a>応答
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemAttachment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.type": "#microsoft.graph.itemAttachment",
  "lastModifiedDateTime": "datetime-value",
  "name": "name-value",
  "contentType": "contentType-value",
  "size": 99,
  "isInline": true,
  "id": "id-value"
}
```


## <a name="example-reference-attachment"></a>例 (添付ファイルの参照)
##### <a name="request"></a>要求
以下は、イベントの添付ファイルの参照を取得する要求の例です。
<!-- {
  "blockType": "request",
  "name": "get_reference_attachment"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/events/{id}/attachments/{id}
```
##### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.referenceAttachment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 215

{
  "@odata.type": "#microsoft.graph.referenceAttachment",
  "contentType": "contentType-value",
  "lastModifiedDateTime": "datetime-value",
  "id": "id-value",
  "isInline": false,
  "name": "name-value",
  "size": 99,
}
```



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
