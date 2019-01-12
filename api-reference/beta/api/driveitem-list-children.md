---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: フォルダーの内容を一覧表示する
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 982bb2374d02ee48408d8c500041fad7813b8588
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951216"
---
# <a name="list-children-of-a-driveitem"></a>driveItem の子を一覧表示する

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

DriveItem の**子**リレーションシップで [DriveItems](../resources/driveitem.md) のコレクションを返します。

NULL でない **folder** または **package** ファセットがある DriveItems は、1 つ以上の子 DriveItems を持つことができます。


## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All    |
|委任 (個人用 Microsoft アカウント) | Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All    |
|アプリケーション | Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/children
GET /groups/{group-id}/drive/items/{item-id}/children
GET /me/drive/items/{item-id}/children
GET /sites/{site-id}/drive/items/{item-id}/children
GET /users/{user-id}/drive/items/{item-id}/children
```

## <a name="optional-query-parameters"></a>オプションのクエリ パラメーター

このメソッドは、応答をカスタマイズするための `$expand`、`$select`、`$skipToken`、`$top`、`$orderby` の [OData クエリ パラメーター](/graph/query-parameters)をサポートします。

### <a name="optional-request-headers"></a>オプションの要求ヘッダー

| ヘッダー名     | 値 | 説明                                                                                                                                              |
|:----------------|:------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| _if-none-match_ | etag  | この要求ヘッダーが含まれている場合、指定された eTag (または cTag) がファイルの現在のタグに一致すると、`HTTP 304 Not Modified` 応答が返されます。 |

## <a name="examples"></a>例

### <a name="list-children-in-the-root-of-the-current-users-drive"></a>現在のユーザーのドライブのルートの子を一覧表示する

ドライブのルートのファイルを取得するには、ドライブ上の `root` リレーションシップを使用し、子のリレーションシップにアクセスします。

<!-- { "blockType": "request", "name": "list-children-root", "scopes": "files.read" } -->

```http
GET /me/drive/root/children
```


### <a name="list-children-of-a-driveitem-with-a-known-id"></a>既知の ID を持つ DriveItem の子を一覧表示する

ドライブのルートのファイルを取得するには、ドライブ上の `root` リレーションシップを使用し、子のリレーションシップにアクセスします。

<!-- { "blockType": "request", "name": "list-children", "scopes": "files.read" } -->

```http
GET /drives/{drive-id}/items/{item-id}/children
```

### <a name="list-children-of-a-driveitem-with-a-known-path"></a>既知のパスを持つ DriveItem の子を一覧表示する

<!-- { "blockType": "request", "name": "list-children-from-path", "scopes": "files.read" } -->

```http
GET /drives/{drive-id}/root:/{path-relative-to-root}:/children
```

## <a name="response"></a>応答

成功すると、このメソッドはターゲット アイテムの子コレクション内にあるアイテムの一覧を返します。
子のコレクションは、[driveItem][item-resource] リソースで構成されます。

<!-- { "blockType": "response", 
       "@odata.type": "Collection(microsoft.graph.driveItem)", 
       "truncated": true,
       "name": [ "list-children-root", "list-children", "list-children-from-path" ] } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {"name": "myfile.jpg", "size": 2048, "file": {} },
    {"name": "Documents", "folder": { "childCount": 4} },
    {"name": "Photos", "folder": { "childCount": 203} },
    {"name": "my sheet(1).xlsx", "size": 197 }
  ],
  "@odata.nextLink": "https://..."
}
```

**注:** コレクションが既定のページ サイズ (200 アイテム) を超えた場合は、応答で **@odata.nextLink** プロパティが返され、より多くのアイテムが使用できることが示されます。また、アイテムの次のページの要求 URL も提供されます。

ページ サイズは[オプションのクエリ文字列パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)で制御できます。

### <a name="error-responses"></a>エラー応答

エラーがどのように返されるかについては、「[エラー応答][error-response]」を参照してください。

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "List the children of an item.",
  "keywords": "list,children,collection",
  "section": "documentation",
  "tocPath": "Items/List children"
} -->
