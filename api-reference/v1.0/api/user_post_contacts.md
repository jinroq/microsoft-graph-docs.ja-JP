# <a name="create-contact"></a>連絡先を作成する

連絡先をルート連絡先フォルダーまたは別の連絡先フォルダーの連絡先エンドポイントに追加します。
## <a name="prerequisites"></a>前提条件
この API を実行するには、以下のいずれかの**スコープ**が必要です。*Contacts.ReadWrite*
## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
POST /me/contacts
POST /users/{id | userPrincipalName}/contacts
POST /me/contactFolders/{contactFolderId}/contacts
POST /users/{id | userPrincipalName}/contactFolders/{contactFolderId}/contacts
```
## <a name="request-headers"></a>要求ヘッダー
| ヘッダー       | 値 |
|:---------------|:--------|
| Authorization  | Bearer <token>. Required.  |
| Content-Type  | application/json  |

## <a name="request-body"></a>要求本文
要求本文で、[連絡先](../resources/contact.md)オブジェクトの JSON 表記を指定します。


## <a name="response"></a>応答
成功した場合、このメソッドは `201, Created` 応答コードと、応答本文で[連絡先](../resources/contact.md)オブジェクトを返します。

## <a name="example"></a>例
##### <a name="request"></a>要求
以下は、要求の例です。
<!-- {
  "blockType": "request",
  "name": "create_contact_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/contacts
Content-type: application/json

{
  "givenName": "Pavel",
  "surname": "Bansky",
  "emailAddresses": [
    {
      "address": "pavelb@fabrikam.onmicrosoft.com",
      "name": "Pavel Bansky"
    }
  ],
  "businessPhones": [
    "+1 732 555 0102"
  ]
}
```
要求本文で、[連絡先](../resources/contact.md)オブジェクトの JSON 表記を指定します。

##### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "createdDateTime": "2015-11-09T02:14:32Z",
  "lastModifiedDateTime": "2015-11-09T02:14:32Z",
   "displayName": "Pavel Bansky"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
