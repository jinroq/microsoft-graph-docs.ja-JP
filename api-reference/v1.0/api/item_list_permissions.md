# <a name="list-permissions-on-a-driveitem"></a>DriveItem のアクセス許可を一覧表示する

[DriveItem](../resources/driveitem.md) の有効なアクセス許可を一覧表示します。

DriveItem の **permissions** リレーションシップは、[DriveItem の取得](item_get.md)または DriveItem のコレクションの取得の一環として展開することはできません。permissions プロパティに直接アクセスする必要があります。

## <a name="access-to-permissions"></a>アクセス許可にアクセスする

アクセス許可のコレクションには、機密情報が含まれている可能性があり、呼び出し元によっては使用できないこともあります。

* アイテムのオーナーの場合は、すべてのアクセス許可が返されます。これには、共同所有者が含まれます。
* 所有者以外の呼び出し元の場合、その呼び出し元に適用されるアクセス許可のみが返されます。
* 秘密 (`shareId` や `webUrl` など) を含むアクセス許可のプロパティは、そのアクセス許可を作成できる呼び出し元にのみ返されます。

## <a name="prerequisites"></a>前提条件
この API を実行するには、以下のいずれかの**スコープ**が必要です。

  * Files.Read
  * Files.ReadWrite

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{item-id}/permissions
GET /me/drive/root:/{path}:/permissions
GET /drives/{drive-id}/items/{item-id}/permissions
GET /groups/{group-id}/drive/items/{item-id}/permissions
```

## <a name="request-headers"></a>要求ヘッダー

| 名前          | 型   | 説明                                                                                                                                     |
|:--------------|:-------|:------------------------------------------------------------------------------------------------------------------------------------------------|
| if-none-match | string | この要求ヘッダーが含まれている場合、指定された etag がアイテムの現在の etag に一致すると、`HTTP 304 Not Modified` 応答が返されます。 |


## <a name="optional-query-parameters"></a>オプションのクエリ パラメーター
このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。

## <a name="request-body"></a>要求本文
このメソッドには、要求本文を指定しません。

## <a name="response"></a>応答
成功した場合、このメソッドは応答本文で `200 OK` 応答コードと、[Permission](../resources/permission.md) リソースのコレクションを返します。

アイテムの有効なアクセス許可は、次の 2 つのソースが元になります。

* アイテム自体に直接適用されるアクセス許可
* アイテムの先祖から継承されたアクセス許可

呼び出し元は、**inheritedFrom** プロパティを確認して、アクセス許可が継承されているかどうかによって区別できます。このプロパティは、アクセス許可が継承された先祖を参照する [**itemReference**](../resources/itemreference.md) リソースです。

## <a name="example"></a>例
##### <a name="request"></a>要求
以下は、要求の例です。
<!-- {
  "blockType": "request",
  "name": "get_permissions"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{item-id}/permissions
```


##### <a name="response"></a>応答
以下は、応答の例です。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permission",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "1",
      "roles": ["write"],
      "link": {
        "webUrl": "https://onedrive.live.com/redir?resid=5D33DD65C6932946!70859&authkey=!AL7N1QAfSWcjNU8&ithint=folder%2cgif",
        "type": "edit"
      }
    },
    {
      "id": "2",
      "roles": ["write"],
      "grantedTo": {
        "user": {
          "id": "5D33DD65C6932946",
          "displayName": "John Doe"
        }
      },
      "inheritedFrom": {
        "driveId": "1234567890ABD",
        "id": "1234567890ABC!123",
        "path": "/drive/root:/Documents" }
    },
    {
      "id": "3",
      "roles": ["write"],
      "link": {
        "webUrl": "https://onedrive.live.com/redir?resid=5D33DD65C6932946!70859&authkey=!AL7N1QAfSWcjNU8&ithint=folder%2cgif",
        "type": "edit",
        "application": {
          "id": "12345",
          "displayName": "TimeTravelPlus"
        }
      }
    }
  ]
}
```

単一のアクセス許可リソースの取得の詳細については、「[アクセス許可を取得する](permission_get.md)」を参照してください。


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List permissions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Item/List permissions"
}-->
