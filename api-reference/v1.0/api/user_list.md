# <a name="list-users"></a>ユーザーを一覧表示する

ユーザー オブジェクトの一覧を取得します。

## <a name="prerequisites"></a>前提条件

この API を実行するには、以下のいずれかの**スコープ**が必要です。*User.ReadBasic.All、User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All*

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
GET /users
```

## <a name="optional-query-parameters"></a>オプションのクエリ パラメーター

このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。

既定では、限定的なプロパティのセットのみが返されます (_businessPhones、displayName、givenName、id、jobTitle、mail、mobilePhone、officeLocation、preferredLanguage、surname、userPrincipalName_)。 

別のプロパティ セットを返すには、ODATA `$select` クエリ パラメーターを使用して、目的の[ユーザー](../resources/user.md) プロパティのセットを指定する必要があります。たとえば、_displayName_、_givenName_、_id_ および _postalCode_ を返すには、クエリに `$select=displayName,givenName,postalCode` を追加します。

> 注意: 特定のプロパティは、ユーザー コレクションでは返すことができません。[単一のユーザーを取得する](./user_get.md)場合にのみ、_aboutMe、birthday、hireDate、interests、mySite、pastProjects, preferredName、responsibilities、schools、skills、mailboxSettings_ の各プロパティがサポートされます。

## <a name="request-headers"></a>要求ヘッダー

| ヘッダー        | 値                      |
|:--------------|:---------------------------|
| Authorization | Bearer {トークン} (必須)  |
| Content-Type  | application/json           | 

## <a name="request-body"></a>要求本文

このメソッドには、要求本文を指定しません。

## <a name="response"></a>応答

成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [user](../resources/user.md) オブジェクトのコレクションを返します。

## <a name="example"></a>例

##### <a name="request"></a>要求

以下は、要求の例です。
<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```http
GET https://graph.microsoft.com/v1.0/users
```

##### <a name="response"></a>応答

以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 608

{
  "value": [
    {
      "businessPhones": [
        "businessPhones-value"
      ],
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "jobTitle": "jobTitle-value",
      "mail": "mail-value",
      "mobilePhone": "mobilePhone-value",
      "officeLocation": "officeLocation-value",
      "preferredLanguage": "preferredLanguage-value",
      "surname": "surname-value",
      "userPrincipalName": "userPrincipalName-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List users",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
