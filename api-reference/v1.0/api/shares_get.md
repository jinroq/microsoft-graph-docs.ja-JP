# <a name="accessing-shared-driveitems"></a>共有 DriveItems へのアクセス

**shareId** または共有の URL を使用して、共有 [DriveItem](../resources/driveitem.md) または共有アイテムのコレクションにアクセスします。

この API で共有の URL を使用するには、[URL を共有のトークンに変換する](#transform-a-sharing-url)必要があります。

## <a name="prerequisites"></a>前提条件

この API を実行するには、以下のいずれかの**スコープ**が必要です。

* Files.ReadWrite
* Files.ReadWrite.All
* Sites.ReadWrite.All

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->
```http
GET /shares/{sharingIdOrUrl}
```

## <a name="request-body"></a>要求本文
このメソッドには、要求本文を指定しません。

## <a name="response"></a>応答

成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [sharedDriveItem](../resources/shareddriveitem.md) リソースを返します。

## <a name="example"></a>例

##### <a name="request"></a>要求

以下は、共有アイテムを取得する要求の例です。

<!-- {
  "blockType": "request",
  "name": "get_shares_by_url"
}-->
```http
GET https://graph.microsoft.com/v1.0/shares/{shareIdOrUrl}
```
##### <a name="response"></a>応答

以下は、応答の例です。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sharedDriveItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "B64397C8-07AE-43E4-920E-32BFB4331A5B",
  "name": "contoso project.docx",
  "owner": {
    "user": {
      "id": "98E88F1C-F8DC-47CC-A406-C090248B30E5",
      "displayName": "Ryan Gregg"
    }
  }
}
```

## <a name="access-the-shared-item-directly"></a>共有アイテムに直接アクセスする

[**SharedDriveItem**](../resources/shareddriveitem.md) には、いくつかの有用な情報が含まれていますが、ほとんどのアプリは、共有の [DriveItem](../resources/driveitem.md)に直接アクセスする必要があります。**SharedDriveItem** リソースには、共有アイテムのスコープ内でコンテンツにアクセスできる、**root** と **items** のリレーションシップが含まれています。

## <a name="example-single-file"></a>例 (単一ファイル)

##### <a name="request"></a>要求

**root** リレーションシップを要求することで、共有された **DriveItem** が返されます。

```http
GET https://graph.microsoft.com/v1.0/shares/{shareIdOrUrl}/root
```

##### <a name="response"></a>応答

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "9FFFDB3C-5B87-4062-9606-1B008CA88E44",
  "name": "contoso project.docx",
  "eTag": "2246BD2D-7811-4660-BD0F-1CF36133677B,1",
  "file": {},
  "size": 109112
}
```

## <a name="example-shared-folder"></a>例 (共有フォルダー)

##### <a name="request"></a>要求

**root** リレーションシップを要求して、**children** コレクションを展開することで、共有されている **DriveItem** が共有フォルダー内のファイルとともに返されます。

```http
GET https://graph.microsoft.com/v1.0/shares/{shareIdOrUrl}/root?$expand=children
```

##### <a name="response"></a>応答

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "9FFFDB3C-5B87-4062-9606-1B008CA88E44",
  "name": "Contoso Project",
  "eTag": "2246BD2D-7811-4660-BD0F-1CF36133677B,1",
  "folder": {}
  "size": 10911212,
  "children": [
    {
      "id": "AFBBDD79-868E-452D-AD4D-24697D4A4044",
      "name": "Propsoal.docx",
      "file": {},
      "size": 19001
    },
    {
      "id": "A91FE90A-2F2C-4EE6-B412-C4FFBA3F71A6",
      "name": "Update to Proposal.docx",
      "file": {},
      "size": 91001
    }
  ]
}
```

## <a name="transform-a-sharing-url"></a>共有の URL を変換する

**shares** API を使用して共有の URL にアクセスするには、URL を共有のトークンに変換する必要があります。

URL を共有のトークンに変化するには:

1. 共有の URL を Base64 エンコードします。
2. 次に示すように、base64 でエンコードしたデータを[パディングされていない base64url 形式](https://en.wikipedia.org/wiki/Base64)に変換します。
  1. 文字列から、末尾の `=` 文字をトリミングします。
  2. 安全でない URL 文字を同等の文字に置き換えます (`/` を `_` に、`+` を `-` に置換します)。
3. 文字列の先頭に `u!` を追加します。

たとえば、次に示す C# メソッドにより、入力文字列を共有のトークンに変換します。

```csharp
string UrlToSharingToken(string inputUrl) {
  var base64Value = System.Convert.ToBase64String(System.Text.Encoding.UTF8.GetBytes(inputUrl));
  return "u!" + base64Value.TrimEnd('=').Replace('/','_').Replace('+','-');
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update permission",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Update permission"
}-->
