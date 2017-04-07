# <a name="update-profilephoto"></a>ProfilePhoto を更新する

サインイン **ユーザー**、または指定された**グループ**または**連絡先**の写真を更新します。現在各 REST 要求の合計サイズは 4 MB に制限されているため、追加する写真のサイズは 4 MB 未満に制限されます。

バージョン 1.0 では、この操作に PATCH と PUT のいずれかを使用できます。

> **注** バージョン 1.0 のこの操作では、ユーザーの職場用または学校用メールボックスのみがサポートされ、個人用メールボックスはサポートされていません。


## <a name="prerequisites"></a>前提条件
この API を実行するには、以下のいずれかの**スコープ**が必要です。

- サインイン **ユーザー** - *User.ReadWrite* のプロファイル写真
- **グループ** - *Group.ReadWrite.All* のプロファイル写真
- **連絡先** - *Contacts.ReadWrite* の写真

## <a name="http-request-to-update-the-photo"></a>写真を更新するための HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/photo/$value
PATCH /users/{id | userPrincipalName}/photo/$value
PATCH /groups/{id}/photo/$value
PATCH /me/contacts/{id}/photo/$value
PATCH /users/{id | userPrincipalName}/contacts/{id}/photo/$value
PATCH /me/contactfolders/{contactFolderId}/contacts/{id}/photo/$value
PATCH /users/{id | userPrincipalName}/contactfolders/{contactFolderId}/contacts/{id}/photo/$value

PUT /me/photo/$value
PUT /users/{id | userPrincipalName}/photo/$value
PUT /groups/{id}/photo/$value
PUT /me/contacts/{id}/photo/$value
PUT /users/{id | userPrincipalName}/contacts/{id}/photo/$value
PUT /me/contactfolders/{contactFolderId}/contacts/{id}/photo/$value
PUT /users/{id | userPrincipalName}/contactfolders/{contactFolderId}/contacts/{id}/photo/$value
```
## <a name="request-headers"></a>要求ヘッダー
| ヘッダー       | 値 |
|:---------------|:--------|
| Authorization  | Bearer <token>. Required.  |
| Content-Type  | image/jpeg。必須。  |

## <a name="request-body"></a>要求本文
要求本文に、写真のバイナリ データを含めます。

## <a name="response"></a>応答
成功した場合、このメソッドは `200 OK` 応答コードを返します。
## <a name="example"></a>例
##### <a name="request"></a>要求
以下は、要求の例です。
<!-- {
  "blockType": "request",
  "name": "update_profilephoto"
}-->
```http
PUT https://graph.microsoft.com/v1.0/me/photo/$value
Content-type: image/jpeg

Binary data for the image

```
##### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.profilePhoto"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update profilephoto",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
