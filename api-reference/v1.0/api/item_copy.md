# <a name="copy-a-driveitem"></a>DriveItem をコピーする

新しい親の下の、または新しい名前を指定した [driveItem](../resources/driveitem.md) (すべての子を含む) のコピーを作成します。

## <a name="prerequisites"></a>前提条件
この API を実行するには、以下のいずれかの**スコープ**が必要です。

  * Files.ReadWrite

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->
```
POST /me/drive/items/{item-id}/copy
POST /me/drive/root:/{path}:/copy
POST /groups/{group-id}/drive/items/{item-id}/copy
```

## <a name="request-body"></a>要求本文
要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。


| 名前            | 値                                          | 説明                                                                                                 |
|:----------------|:-----------------------------------------------|:------------------------------------------------------------------------------------------------------------|
| parentReference | [ItemReference](../resources/itemreference.md) | 省略可能。コピーが作成される親アイテムへの参照。                                         |
| name            | string                                         | 省略可能。コピーの新しい名前。これを指定しない場合は、元の名前と同じ名前が使用されます。    |

**注:**_parentReference_ には `id` か `path` のいずれかを含める必要がありますが、両方を含める必要はありません。両方が含まれる場合は、それらが同じアイテムを参照する必要があります。そうでないと、エラーが発生します。

## <a name="example"></a>例

<!-- { "blockType": "request", "name": "copy-item", "scopes": "files.readwrite" } -->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{item-id}/copy
Content-Type: application/json

{
  "parentReference": {
    "path": "/drive/root:/Documents"
  },
  "name": "contoso plan.docx"
}
```

## <a name="response"></a>応答

要求の受け入れ時に、コピーの進行状況を監視する方法についての詳細を返します。

<!-- { "blockType": "response" } -->
```http
HTTP/1.1 202 Accepted
```

## <a name="remarks"></a>注釈

多くの場合、コピー操作は非同期で実行されます。API からの応答は、コピー操作が受け入れられたか、コピー先のファイル名が既に使用中のためという理由で拒否されたことのみを示します。

**注:**API は、コピーが成功したかどうかを知るためのメソッドは提供しません。

<!-- {
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Copy"
} -->
