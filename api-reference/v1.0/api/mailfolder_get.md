# <a name="get-mailfolder"></a>mailFolder を取得する

メッセージ フォルダー オブジェクトのプロパティとリレーションシップを取得します。


### <a name="get-another-users-message-folder"></a>別のユーザーのメッセージ フォルダーを取得する

アプリケーションのアクセス許可がある場合や、1 人のユーザーから適切に委任された[アクセス許可](#permissions)がある場合には、別のユーザーのメッセージ フォルダーを取得することができます。 このセクションでは、委任されたアクセス許可に関連するシナリオについて説明します。

たとえば、アプリがユーザー John から委任されたアクセス許可を取得したとします。 別のユーザー Garth は、John とメッセージ フォルダーを共有しています。 その場合、以下に示す例のクエリで、Garth のユーザー ID (またはユーザー プリンシパル名) を指定することにより、その共有フォルダーを取得できます。

<!-- { "blockType": "ignored" } -->
```http
GET /users/{Garth-id | Garth-userPrincipalName}/mailFolders/{id}
```

この機能は、後述の [HTTP 要求](#http-request)セクションに記載されている、個々のユーザーに対するすべての GET メッセージ フォルダー操作に適用されます。 これは、Garth が John にメールボックス全体を委任した場合にも適用されます。

Garth が John とメッセージ フォルダーを共有していない、もしくはメールボックスを John に委任していない場合、それらの GET 操作に Garth のユーザー ID またはユーザー プリンシパル名を指定すると、エラーが返されます。 このような場合、ユーザー ID またはユーザー プリンシパル名の指定は、サインインしているユーザー自身のメッセージ フォルダーを取得するためにのみ使用でき、そのクエリは /me ショートカットを使用することと同義となります。

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}
```

この機能は、以下の GET 操作でのみ使用できます。

- 共有の連絡先フォルダー、予定表、メッセージ フォルダー 
- 連絡先、イベント、共有フォルダー内のメッセージ
- 委任されたメールボックス内の上述のリソース

この機能は、連絡先、イベント、メッセージ、それらのフォルダーに対する他の操作では使用できません。


## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Mail.Read、Mail.ReadWrite    |
|委任 (個人用 Microsoft アカウント) | Mail.Read、Mail.ReadWrite    |
|アプリケーション | Mail.Read、Mail.ReadWrite |

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}
```
## <a name="optional-query-parameters"></a>オプションのクエリ パラメーター
このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。
## <a name="request-headers"></a>要求ヘッダー
| 名前       | 型 | 説明|
|:-----------|:------|:----------|
| Authorization  | string  | ベアラー {トークン}。必須。 |

## <a name="request-body"></a>要求本文
このメソッドには、要求本文を指定しません。

## <a name="response"></a>応答

成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [mailFolder](../resources/mailfolder.md) オブジェクトを返します。
## <a name="example"></a>例
##### <a name="request"></a>要求
以下は、要求の例です。
<!-- {
  "blockType": "request",
  "name": "get_mailfolder"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/{id}
```
##### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 179

{
  "displayName": "displayName-value",
  "parentFolderId": "parentFolderId-value",
  "childFolderCount": 99,
  "unreadItemCount": 99,
  "totalItemCount": 99,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get mailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
