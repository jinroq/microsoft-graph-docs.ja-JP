# <a name="message-createforward"></a>メッセージ: createForward

転送メッセージの下書きを作成します。その後、下書きを[更新](../api/message_update.md)または[送信](../api/message_send.md)できます。

## <a name="prerequisites"></a>前提条件
この API を実行するには、以下のいずれかの**スコープ**が必要です。*Mail.ReadWrite*
## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/createForward
POST /users/{id | userPrincipalName}/messages/{id}/createForward
POST /me/mailFolders/{id}/messages/{id}/createForward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createForward
```
## <a name="request-headers"></a>要求ヘッダー
| 名前       | 型 | 説明|
|:---------------|:--------|:----------|
| Authorization  | string  | Bearer <token>. Required. |
| Content-Type | string  | エンティティ本文内のデータの性質です。必須。 |

## <a name="request-body"></a>要求本文

## <a name="response"></a>応答
成功した場合、このメソッドは `201, Created` 応答コードと、応答本文で [Message](../resources/message.md) オブジェクトを返します。

## <a name="example"></a>例
以下は、この API を呼び出す方法の例です。
##### <a name="request"></a>要求
以下は、要求の例です。
<!-- {
  "blockType": "request",
  "name": "message_createforward"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/createForward
Content-type: application/json
Content-length: 248

{
  "comment": "Comment-value",
  "toRecipients": [
    {
      "emailAddress": {
        "address": "address-value"
      }
    },
    {
      "emailAddress": {
        "address": "address-value"
      }
    }
  ]
}
```

##### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 248

{
  "receivedDateTime": "datetime-value",
  "sentDateTime": "datetime-value",
  "hasAttachments": true,
  "subject": "subject-value",
  "body": {
    "contentType": "",
    "content": "content-value"
  },
  "bodyPreview": "bodyPreview-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: createForward",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
