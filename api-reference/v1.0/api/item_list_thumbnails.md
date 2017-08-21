# <a name="list-thumbnails-for-a-driveitem"></a>DriveItem のサムネイルを一覧表示する

[DriveItem](../resources/driveitem.md) リソースの [ThumbnailSet](../resources/thumbnailset.md) リソースのコレクションを取得します。

DriveItem はゼロ以上の [ThumbnailSet](../resources/thumbnailset.md) リソースで表すことができます。各 **thumbnailSet** は 1 つ以上の[**サムネイル**](../resources/thumbnail.md) オブジェクトを持つことができ、そのオブジェクトはアイテムを表すイメージです。たとえば、**thumbnailSet** には `small`、`medium`、`large` など、一般的な**サムネイル** オブジェクトが含まれます。

OneDrive 上でサムネイルを操作する方法はたくさんあります。次に、最も一般的なものを示します。

* アイテムの利用可能なサムネイルを列挙する
* アイテムの 1 つのサムネイルを取得する
* サムネイルのコンテンツを取得する
* 1 つの要求で複数のアイテムのサムネイルを取得する
* カスタムのサムネイル サイズを取得する
* アイテムのカスタム サムネイルをアップロードする
* カスタムのアップロード済みサムネイルが存在するかどうかを確認する


## <a name="prerequisites"></a>前提条件
この API を実行するには、以下のいずれかの**スコープ**が必要です。

* Files.Read
* Files.ReadWrite
* Files.Read.All
* Files.ReadWrite.All
* Sites.Read.All
* Sites.ReadWrite.All


## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/root:/{item-path}:/thumbnails
GET /me/drive/items/{item-id}/thumbnails
GET /groups/{group-id}/drive/items/{item-id}/thumbnails
```

## <a name="optional-query-parameters"></a>オプションのクエリ パラメーター
このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。

## <a name="request-body"></a>要求本文
このメソッドには、要求本文を指定しません。

## <a name="response"></a>応答

成功した場合、このメソッドは応答本文で `200 OK` 応答コードと [ThumbnailSet](../resources/thumbnailset.md) オブジェクトのコレクションを返します。

## <a name="example"></a>例

##### <a name="request"></a>要求

以下は、要求の例です。

<!-- {
  "blockType": "request",
  "name": "get_thumbnails"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{item-id}/thumbnails
```


##### <a name="response"></a>応答
以下は、応答の例です。

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.thumbnailSet",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "0",
      "small": { "height": 64, "width": 96, "url": "https://sn3302files..."},
      "medium": { "height": 117, "width": 176, "url": "https://sn3302files..."},
      "large": { "height": 533, "width": 800, "url": "https://sn3302files..."}
    }
  ]
}
```

## <a name="retrieve-a-single-thumbnail"></a>1 つのサムネイルを取得する

1 つのサムネイルとサイズのメタデータを、要求で直接識別することにより取得します。

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "request", "name": "get-one-thumbnail" } -->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}
```

## <a name="path-parameters"></a>パス パラメーター

| 名前         | 型   | 説明                                                                         |
|:-------------|:-------|:------------------------------------------------------------------------------------|
| **item-id**  | string | 参照されるアイテムの一意識別子。                                      |
| **thumb-id** | number | サムネイルのインデックス (通常 0-4)。                                            |
| **size**     | string | 要求されたサムネイルのサイズ。これは、リストされた標準的なサイズのいずれかでなければなりません。 |


<!-- { "blockType": "response", "@odata.type": "microsoft.graph.thumbnail" } -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "width": 100,
  "height": 100,
  "url": "http://onedrive.com/asd123a/asdjlkasjdkasdjlk.jpg"
}
```

## <a name="retrieve-thumbnail-content"></a>サムネイルのコンテンツを取得する

サムネイルの **content** プロパティを要求することにより、サムネイルのコンテンツを直接、取得できます。

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "request", "name":"get-thumbnail-content" } -->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}/content
```

## <a name="response"></a>応答

サービスは、サムネイルの URL へのリダイレクトで応答します。

<!-- { "blockType": "response" } -->
```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

サムネイルのコンテンツ URL は事前認証されており、承認ヘッダーをダウンロードする必要はありません。これらの URL の存続時間は短く、数時間しか有効ではないため、アプリでキャッシュされません。


## <a name="size-values"></a>サイズの値

次の表で、使用可能なサムネイルのサイズを定義します。サムネイルの任意のサイズを要求できますが、定義済みの値が存在する可能性が高く、値は即時に返されます。

| 名前           | 解像度  | 縦横比 | 説明                                                          |
|:---------------|:------------|:-------------|:---------------------------------------------------------------------|
| `small`        | 96 longest  | Original     | 圧縮率の高い小さなサムネイルは、正方形にトリミングされます。 |
| `medium`       | 176 longest | Original     | OneDrive の Web ビューの標準的なアイテムのサイズにトリミングされます。         |
| `large`        | 800 longest | Original     | サムネイルの長辺が 800 ピクセルになるよう、サイズ変更されます。               |

## <a name="remarks"></a>注釈

**注:** OneDrive for Business および SharePoint の場合:

* 次の呼び出しを使用したサムネイル コレクションの展開は機能しません: `GET /drive/root:/{item-path}?expand=children(expand=thumbnails)`
  `GET /drive/items/{item-id}/children?expand=thumbnails`


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get metadata and content for thumbnails of multiple sizes for OneDrive items.",
  "keywords": "thumbnail,content,download,sizes",
  "section": "documentation",
  "tocPath": "OneDrive/Item/List thumbnails"
} -->
