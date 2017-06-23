# <a name="create-thread"></a>スレッドを作成する

指定した会話に新しいスレッドを作成します。 

指定したとおりにスレッドと投稿を作成します。[スレッドに返信](conversationthread_reply.md) を使用して、そのスレッドへの投稿を続けます。また、投稿 ID を取得している場合は、そのスレッドのその投稿にも[返信](post_reply.md)できます。

注:[最初にスレッドを作成して、新しい会話を開始](group_post_threads.md)することもできます。

## <a name="prerequisites"></a>前提条件
この API を実行するために必要な**スコープ**は、次のとおりです。*Group.ReadWrite.All*
## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/conversations/{id}/threads
```
## <a name="request-headers"></a>要求ヘッダー
| 名前       | 型 | 説明|
|:---------------|:--------|:----------|
| Authorization  | string  | ベアラー {トークン}。必須。 |

## <a name="request-body"></a>要求本文
要求の本文に、[ConversationThread](../resources/conversationthread.md) オブジェクトの JSON 表記を指定します。


## <a name="response"></a>応答
成功した場合、このメソッドは `201, Created` 応答コードと、応答本文で [conversationThread](../resources/conversationthread.md) オブジェクトを返します。

## <a name="example"></a>例
##### <a name="request"></a>要求
以下は、要求の例です。
<!-- {
  "blockType": "request",
  "name": "create_conversationthread_from_conversation"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/conversations/{id}/threads
Content-type: application/json

{
  "topic": "topic-value",
  "posts": [{
      "body": {
        "contentType": "html",
        "content": "this is body content"
      }
  }]
}
```
要求の本文に、[conversationThread](../resources/conversationthread.md) オブジェクトの JSON 表記を指定します。
##### <a name="response"></a>応答

成功した場合、このメソッドは `201, Created` 応答コードと、応答本文で新しいスレッドの `id` を返します。以下は、応答の例です。 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 346

{
  "id": "thread-id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create thread",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
