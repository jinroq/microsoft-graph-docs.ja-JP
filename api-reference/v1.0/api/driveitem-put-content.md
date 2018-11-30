---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: サイズの小さいファイルをアップロードする
ms.openlocfilehash: ca6b374561699ccf70c55878dc67cb17d9ed744b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020692"
---
# <a name="upload-or-replace-the-contents-of-a-driveitem"></a>DriveItem の内容をアップロードまたは置換する

簡単なアップロード API を使用すると、新しいファイルの内容を提供したり、単一の API 呼び出しで既存のファイルの内容を更新したりすることができます。このメソッドは、サイズが 4MB までのファイルのみをサポートしています。

大きなファイルをアップロードする場合は、「[アップロード セッションを使ってサイズの大きなファイルをアップロードする](driveitem-createuploadsession.md)」を参照してください。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All    |
|委任 (個人用 Microsoft アカウント) | Files.ReadWrite、Files.ReadWrite.All    |
|アプリケーション | Files.ReadWrite.All、Sites.ReadWrite.All |

## <a name="http-request-to-replace-an-existing-item"></a>HTTP 要求 (既存アイテムを置換する)

<!-- { "blockType": "ignored" } -->

```http
PUT /drives/{drive-id}/items/{item-id}/content
PUT /groups/{group-id}/drive/items/{item-id}/content
PUT /me/drive/items/{item-id}/content
PUT /sites/{site-id}/drive/items/{item-id}/content
PUT /users/{user-id}/drive/items/{item-id}/content
```

## <a name="http-request-to-upload-a-new-file"></a>HTTP 要求 (新しいファイルをアップロードする)

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

成功した場合、このメソッドは新しく作成された、または更新されたファイルの応答本文で [driveItem](../resources/driveitem.md) オブジェクトを返します。

## <a name="example-upload-a-new-file"></a>例 (新しいファイルのアップロード)

この例では、"The contents of the file goes here."(ファイルの内容がここに入ります。) という文字列を、 サインインしたユーザーのドライブにある FolderA 下の FileB.txt という名前のファイルにアップロードします。

<!-- { "blockType": "request", "name": "upload-via-put", "scopes": "files.readwrite" } -->

```http
PUT /me/drive/root:/FolderA/FileB.txt:/content
Content-Type: text/plain

The contents of the file goes here.
```

### <a name="response"></a>応答

成功した場合、このメソッドは、応答本文で新しく作成したファイルの [driveItem][item-resource] リソースを返します。

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

<!-- { "blockType": "request", "name": "upload-via-put-id", "scopes": "files.readwrite" } -->

```http
PUT /me/drive/items/{item-id}/content
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

## <a name="error-responses"></a>エラー応答

エラーがどのように返されるかについては、「[エラー応答][error-response]」を参照してください。

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a new file with content or update a file's content.",
  "keywords": "insert,upsert,update,upload",
  "section": "documentation"
} -->