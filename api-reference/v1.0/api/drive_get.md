# <a name="get-drive"></a>ドライブを取得する

[Drive](../resources/drive.md) リソースのプロパティと関係を取得します。ドライブは、ファイル システムの最上位のコンテナーです。Graph API を使用すると、ユーザーの OneDrive または OneDrive for Business や SharePoint ドキュメント ライブラリのドライブ リソースにアクセスできます。

## <a name="prerequisites"></a>前提条件

この API を実行するには、以下のいずれかの**スコープ**が必要です。

* Files.Read
* Files.ReadWrite
* Files.Read.All
* Files.ReadWrite.All
* Sites.Read.All
* Sites.ReadWrite.All

## <a name="get-a-users-onedrive"></a>ユーザーの OneDrive を取得する

ユーザーの OneDrive または OneDrive for Business にアクセスするには、[User](../resources/user.md) リソースについての**ドライブ**関係をアプリが要求する必要があります。

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->

```http
GET /me/drive
GET /users/{idOrUserPrincipalName}/drive
```

## <a name="get-the-document-library-associated-with-a-group"></a>グループに関連付けられたドキュメント ライブラリを取得する

[グループの](../resources/group.md)既定のドキュメント ライブラリにアクセスするには、そのグループについての**ドライブ**関係をアプリが要求する必要があります。

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->

```http
GET /groups/{idOrUserPrincipalName}/drive
```


## <a name="optional-query-parameters"></a>オプションのクエリ パラメーター

このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。

## <a name="request-body"></a>要求本文

このメソッドには、要求本文を指定しません。

## <a name="response"></a>応答

成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Drive](../resources/drive.md) リソースを返します。

## <a name="example"></a>例

##### <a name="request"></a>要求

サインインしているユーザーの OneDrive または OneDrive for Business を取得する要求の例を次に示します。

<!-- {
  "blockType": "request",
  "name": "get_drive"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive
```

##### <a name="response"></a>応答

以下は、応答の例です。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.drive"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "b!t18F8ybsHUq1z3LTz8xvZqP8zaSWjkFNhsME-Fepo75dTf9vQKfeRblBZjoSQrd7",
    "driveType": "business",    
    "owner": {
        "user": {
            "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
            "displayName": "Ryan Gregg"
        }
    },
    "quota": {
        "deleted": 256938,
        "remaining": 1099447353539,
        "state": "normal",
        "total": 1099511627776
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get metadata for a OneDrive, OneDrive for Business, or Office 365 group drive",
  "keywords": "drive,onedrive,default drive,group drive",
  "section": "documentation",
  "tocPath": "OneDrive/Drive/Get Drive"
}-->
