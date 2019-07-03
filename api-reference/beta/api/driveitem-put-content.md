---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: サイズの小さいファイルをアップロードする
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 492ad11a6bd74b45fea77aee46c6e0050a1927a3
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35436271"
---
# <a name="upload-or-replace-the-contents-of-a-driveitem"></a>DriveItem の内容をアップロードまたは置換する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

簡単なアップロード API を使用すると、新しいファイルの内容を提供したり、単一の API 呼び出しで既存のファイルの内容を更新したりすることができます。このメソッドは、サイズが 4MB までのファイルのみをサポートしています。

大きなファイルをアップロードする場合は、「[アップロード セッションを使ってサイズの大きなファイルをアップロードする](driveitem-createuploadsession.md)」を参照してください。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All    |
|委任 (個人用 Microsoft アカウント) | Files.ReadWrite、Files.ReadWrite.All    |
|アプリケーション | Files.ReadWrite.All、Sites.ReadWrite.All |

## <a name="http-request-to-replace-an-existing-item"></a>HTTP 要求 (既存アイテムを置換する場合)

<!-- { "blockType": "ignored" } -->

```http
PUT /drives/{drive-id}/items/{item-id}/content
PUT /groups/{group-id}/drive/items/{item-id}/content
PUT /me/drive/items/{item-id}/content
PUT /sites/{site-id}/drive/items/{item-id}/content
PUT /users/{user-id}/drive/items/{item-id}/content
```

## <a name="http-request-to-upload-a-new-file"></a>HTTP 要求 (新しいファイルをアップロードする場合)

<!-- { "blockType": "ignored" } -->

```http
PUT /drives/{drive-id}/items/{parent-id}:/{filename}:/content
PUT /groups/{group-id}/drive/items/{parent-id}:/{filename}:/content
PUT /me/drive/items/{parent-id}:/{filename}:/content
PUT /sites/{site-id}/drive/items/{parent-id}:/{filename}:/content
PUT /users/{user-id}/drive/items/{parent-id}:/{filename}:/content
```

## <a name="request-body"></a>要求本文

要求の本文の内容は、アップロードするファイルのバイナリ ストリームである必要があります。

## <a name="response"></a>応答

成功した場合、このメソッドは、新しく作成されたファイルまたは更新されたファイルの応答本文で [driveItem](../resources/driveitem.md) オブジェクトを返します。

## <a name="example-upload-a-new-file"></a>例 (新しいファイルのアップロード)

この例では、"The contents of the file goes here."(ファイルの内容がここに入ります。) という文字列を、 サインインしたユーザーのドライブの FolderA の下の FileB.txt という名前のファイルにアップロードします。

<!-- { "blockType": "request", "name": "upload-via-put", "scopes": "files.readwrite" } -->

```http
PUT /me/drive/root:/FolderA/FileB.txt:/content
Content-Type: text/plain

The contents of the file goes here.
```

### <a name="response"></a>応答

成功した場合、このメソッドは、新しく作成されたファイルの応答本文で [driveItem][item-resource] リソースを返します。

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "0123456789abc",
  "name": "FileB.txt",
  "size": 35,
  "file": { }
}
```

## <a name="example-updating-an-existing-file"></a>例 (既存ファイルの更新)

この例では、既知の ID を持つファイルの内容を置き換えます。


# <a name="httptabhttp"></a>[プロトコル](#tab/http)
<!-- { "blockType": "request", "name": "upload-via-put-id", "scopes": "files.readwrite" } -->

```http
PUT /me/drive/items/{item-id}/content
Content-Type: text/plain

The contents of the file goes here.
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/upload-via-put-id-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/upload-via-put-id-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>応答

成功した場合、このメソッドは、新しく作成されたファイルの応答本文で [driveItem][item-resource] リソースを返します。

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "0123456789abc",
  "name": "FileB.txt",
  "size": 35,
  "file": { }
}
```

## <a name="error-responses"></a>エラー応答

エラーがどのように返されるかについては、「[エラー応答][error-response]」を参照してください。

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md

<!--
{
  "type": "#page.annotation",
  "description": "Create a new file with content or update a file's content.",
  "keywords": "insert,upsert,update,upload",
  "section": "documentation",
  "suppressions": [
  ]
}
-->
