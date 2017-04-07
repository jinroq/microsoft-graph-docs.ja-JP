# <a name="list-items-shared-with-the-signed-in-user"></a>サインインしているユーザーと共有しているアイテムを一覧表示する

[ドライブ](../resources/drive.md) の所有者と共有されている、[DriveItem](../resources/driveitem.md) リソースのコレクションを取得します。

## <a name="prerequisites"></a>前提条件
この API を実行するには、以下のいずれかの**スコープ**が必要です。

  * Files.Read.All
  * Files.ReadWrite.All

**注:** Files.Read または Files.ReadWrite の範囲での /sharedWithMe 要求は成功しますが、いくつかのプロパティが失われている可能性があります。さらに、**すべて**の範囲のうちの一つがなければ、この API から返された共有項目はアクセスできません。

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->
```
GET /me/drive/sharedWithMe
```

## <a name="request-body"></a>要求本文
このメソッドには、要求本文を指定しません。

## <a name="example"></a>例

<!-- { "blockType": "request", "name": "drive-sharedwithme", "scopes": "files.read" } -->
```http
GET https://graph.microsoft.com/v1.0/me/drive/sharedWithMe
```

## <a name="response"></a>応答

これは、ドライブの所有者を共有している DriveItem リソースを含む、[DriveItem](../resources/driveitem.md) リソースのコレクションを返します。この例では、ドライブはユーザーの既定のドライブです。そのため、これはサインインしているユーザーと共有しているアイテムを返します。


<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "isCollection": true, "truncated": true } -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "1312abc",
      "remoteItem": {
        "id": "1991210caf!192",
        "name": "March Proposal.docx",
        "file": { },
        "size": 19121,
        "parentReference": {
          "driveId": "1991210caf",
          "id": "1991210caf!104"
        }
      }
    },
    {
      "id": "1312def",
      "remoteItem": {
        "id": "1991210caf!1991",
        "name": "Team Roster.xlsx",
        "file": { },
        "size": 37619,
        "parentReference": {
          "driveId": "1991210caf",
          "id": "1991210caf!104"
        }
      }
    }
  ]
}
```

## <a name="remarks"></a>注釈

**sharedWithMe** アクションから返された DriveItems には、それらが異なるドライブからのアイテムであることを示す [**remoteItem**](../resources/remoteitem.md) ファセットが必ず含まれます。共有された DriveItem リソースにアクセスするには、**remoteItem** で提供された情報を使用して、以下に示す書式で要求を作成する必要があります。

<!-- {"blockType": "ignored"} -->
```http
GET https://graph.microsoft.com/v1.0/drives/{remoteItem.parentReference.driveId}/items/{remoteItem.id}
```

<!-- {
  "type": "#page.annotation",
  "description": "Retrieve a list of files shared with the signed-in user.",
  "keywords": "sharedWithMe onedrive shared files",
  "section": "documentation",
  "tocPath": "OneDrive/Drive/Shared with me"
} -->
