# <a name="create-acceptedsender"></a>AcceptedSender の作成

AcceptedSender リストに新しいユーザーやグループを追加します。

`@odata.id` 内のユーザーやグループを要求の本文で指定します。承諾済み送信者リスト内のユーザーは、グループに会話を投稿できません。承認送信者と拒否送信者のリストに同一のユーザーやグループを指定すると、エラーになるので注意してください。
## <a name="prerequisites"></a>前提条件
この API を実行するには、以下のいずれかの**スコープ**が必要です。*Group.ReadWrite.All*
## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/acceptedSenders/$ref
```
## <a name="request-headers"></a>要求ヘッダー
| ヘッダー       | 値 |
|:---------------|:--------|
| Authorization  | Bearer <token>. Required.  |

## <a name="request-body"></a>要求本文
要求の本文で、ユーザーまたはグループのオブジェクトの id を指定します。


## <a name="response"></a>応答
このメソッドは `204, No Content` 応答コードを返し、応答の本文は返しません。

## <a name="example"></a>例
##### <a name="request"></a>要求
以下は、要求の例です。
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/acceptedSenders/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id":"https://graph.microsoft.com/v1.0/users/alexd@contoso.com"
}
```
##### <a name="response"></a>応答
以下は、応答の例です。
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create acceptedSender",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
