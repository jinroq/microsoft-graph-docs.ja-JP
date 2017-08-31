# <a name="search-for-a-driveitem-within-a-drive"></a>ドライブ内の DriveItem を検索する

クエリと一致するアイテムを対象にアイテムの階層を検索します。フォルダー階層内、ドライブ全体、または現在のユーザーと共有されるファイル内で検索できます。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All    |
|委任 (個人用 Microsoft アカウント) | Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All    |
|アプリケーション | Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```
GET /me/drive/root/search(q='{search-text}')
GET /me/drive/items/{item-id}/search(q='{search-text}')
GET /me/drive/root:/{item-path}:/search(q='{search-text}')
GET /drives/{drive-id}/root/search(q='{search-text}')
GET /groups/{group-id}/drive/root/search(q='{search-text}')
```

## <a name="optional-query-parameters"></a>オプションのクエリ パラメーター
このメソッドは、応答をカスタマイズするための `$expand``$select`、`$skipToken`、`$top`、および `$orderby` [OData クエリ パラメーター](../../../concepts/query_parameters.md)をサポートします。

## <a name="request-body"></a>要求本文
このメソッドには、要求本文を指定しません。

#### <a name="function-parameters"></a>関数パラメーター

| 名前 | 値  | 説明                                                                                                                          |
|:-----|:-------|:-------------------------------------------------------------------------------------------------------------------------------------|
| `q`  | string | アイテムの検索に使用するクエリ テキスト。値は、ファイル名、メタデータ、およびファイルのコンテンツを含む複数のフィールドに渡って照合できます。 |

## <a name="example"></a>例

##### <a name="request"></a>要求

ここでは、現在のユーザーの OneDrive を検索する要求の例を示します。
<!-- {
  "blockType": "request",
  "name": "item_search"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/root/search(q='{search-query}')
```

##### <a name="response"></a>応答
このメソッドは、検索条件に一致する [DriveItems](../resources/driveitem.md) のコレクション含んでいるオブジェクトを返します。アイテムが見つからない場合は、空のコレクションが返されます。

一致が多すぎる場合は、応答はページ化され、**@odata.nextLink** プロパティには、後続の結果ページへの URL が含まれます。`$top` クエリ パラメーターを使用すると、ページ内のアイテム数を指定できます。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.driveItem",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
      {
        "id": "0123456789abc!123",
        "name": "Contoso Project",
        "folder": {},
        "searchResult": { "onClickTelemetryUrl": "https://bing.com/0123456789abc!123" }
      },
      {
        "id": "0123456789abc!456",
        "name": "Contoso Project 2016",
        "folder": {},
        "searchResult": { "onClickTelemetryUrl": "https://bing.com/0123456789abc!456" }
      }
    ],
    "@odata.nextLink": "https://graph.microsoft.com/v1.0/me/drive/root/search(query='contoso project')&skipToken=1asdlnjnkj1nalkm!asd"
}
```

## <a name="searching-for-items-a-user-can-access"></a>ユーザーがアクセスできるアイテムの検索

ドライブ内のアイテムの検索に加えて、アプリでは現在のユーザーと共有されるアイテムを含めるように、検索範囲を広げることができます。検索範囲を広げるには、[Drive](../resources/drive.md) リソースの **search** メソッドを使用します。

##### <a name="request"></a>要求

<!-- {
  "blockType": "request",
  "name": "item_search_all"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/search(q='{search-query}')
```

##### <a name="response"></a>応答
**ドライブ** リソースからの検索時の応答には、ドライブの外部のアイテム (現在のユーザーと共有されているアイテム) が含まれていることがあります。こうしたアイテムには、それらが対象のドライブの外部に保存されていることを示す、[**remoteItem**](../resources/remoteitem.md) ファセットが含まれます。 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.driveItem",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
      {
        "id": "0123456789abc!123",
        "name": "Contoso Project",
        "folder": {},
        "searchResult": { "onClickTelemetryUrl": "https://bing.com/0123456789abc!123" },
        "remoteItem": { "id": "!23141901", "driveId": "s!1020101jlkjl12lx" }
      },
      {
        "id": "0123456789abc!456",
        "name": "Contoso Project 2016",
        "folder": {},
        "searchResult": { "onClickTelemetryUrl": "https://bing.com/0123456789abc!456" }
      }
    ],
    "@odata.nextLink": "https://graph.microsoft.com/v1.0/me/drive/root/search(query='contoso project')&skipToken=1asdlnjnkj1nalkm!asd"
}
```




<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "item: search",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Items/Search items"
}-->
