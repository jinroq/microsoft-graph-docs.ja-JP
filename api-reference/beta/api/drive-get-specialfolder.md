---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: 特殊フォルダーを取得する
ms.openlocfilehash: 8b8b1186682421a5ab564272fd473cb72819202d
ms.sourcegitcommit: 37591c2299c80e7675cd2b5f781e1eeeba628a60
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/08/2019
ms.locfileid: "27748501"
---
# <a name="get-a-special-folder-by-name"></a>名前で特殊フォルダーを取得する

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

特殊なコレクションを使用して、名前で特殊フォルダーにアクセスします。

特殊フォルダーは、フォルダーを (ローカライズが必要となる) パスで探したり、ID を持つフォルダーを参照したりせずに、OneDrive の既知のフォルダーにアクセスするための、単純なエイリアスを提供します。特殊フォルダーの名前が変更されたりドライブ内の別の場所に移動されたりした場合でも、この構文はそのフォルダーを返し続けます。

特殊なフォルダーは、まだ存在していない場合、アプリケーションが最初に書き込みを試行したときに自動的に作成されます。ユーザーが削除した場合は、もう一度書き込まれたときに再作成されます。

> **注:** 読み取り専用のアクセス許可が付与されているときに、存在していない特殊フォルダーを要求すると、`403 Forbidden` エラーが返されます。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|            アクセス許可の種類             |                                           アクセス許可 (特権の小さいものから大きいものへ)                                            |
| :------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------- |
| 委任 (職場または学校のアカウント)     | Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All                            |
| 委任 (個人用 Microsoft アカウント) | Files.ReadWrite.AppFolder、Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All |
| アプリケーション                            | Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All                                                         |

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "request", "name": "get-special-folder", "scopes": "files.read" } -->

```http
GET /me/drive/special/{name}
```

### <a name="special-folder-names"></a>特殊フォルダー名

以下の特殊フォルダー名は、OneDrive および OneDrive for Business で使用できます。

| 名前        | フォルダー ID    | 説明                                                              |
|:------------|:-------------|:-------------------------------------------------------------------------|
| Documents   | `documents`  | ドキュメント フォルダー。                                                    |
| Photos      | `photos`     | フォト フォルダー。                                                       |
| Camera Roll | `cameraroll` | カメラ ロールのバックアップ フォルダー。                                           |
| App Root    | `approot`    | そのアプリケーションの個人用フォルダー。通常は `/Apps/{Application Name}` 内 |
| Music       | `music`      | ミュージック フォルダー。                                                        |


### <a name="optional-query-parameters"></a>オプションのクエリ パラメーター

このメソッドは、応答をカスタマイズするための `$expand` と `$select` の [OData クエリ パラメーター](/graph/query-parameters)をサポートします。

## <a name="response"></a>応答

このメソッドは `200 OK` 応答コードと、応答本文で [driveItem](../resources/driveitem.md) オブジェクトを返します。

プロパティや driveItem 上のリレーションシップへの付加的な呼び出しを伴う、特殊フォルダーのインラインのアドレス指定のメソッドを使用できます。

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "0123456789abc",
  "name": "Documents",
  "eTag": "012345819293.1",
  "specialFolder": {
    "name": "documents"
  }
}
```

## <a name="get-children-of-a-special-folder"></a>特殊フォルダーの子を取得します。

特殊フォルダーの子を要求する場合は、`children` コレクションを要求するか、子コレクションを展開する [expand](/graph/query-parameters) オプションを使用します。

### <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "request", "name": "get-special-children", "scopes": "files.read" } -->

```http
GET /me/drive/special/{name}/children
```

### <a name="response"></a>応答

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "isCollection": true, "truncated": true} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {"name": "myfile.jpg", "size": 2048 },
    {"name": "Documents", "folder": { "childCount": 4} },
    {"name": "Photos", "folder": { "childCount": 203} },
    {"name": "my sheet(1).xlsx", "size": 197 }
  ]
}
```

## <a name="remarks"></a>備考

> **注:** `specialFolder` ファセットを伴う DriveItem は、アイテムが特殊フォルダーであり、`special` コレクション経由でアクセスできることを示しています。

アプリに読み取り専用アクセス許可が付与されている場合、特殊フォルダーまたは特殊フォルダーの子を取得する要求は、その特殊フォルダーが存在していないと、`404 Not Found` エラーまたは `403 Forbidden` エラーで失敗します。

<!-- {
  "type": "#page.annotation",
  "description": "Access known folders in OneDrive through the special folder collection",
  "keywords": "known folders",
  "section": "documentation",
  "tocPath": "OneDrive/Drive/Special folders"
} -->
