---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: 旧バージョンのリスト アイテムを取得する - SharePoint API
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 4068ebd1e8a245f2418954ce04bad1f78530acd0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27983878"
---
# <a name="get-a-listitemversion-resource-preview"></a>ListItemVersion リソースを取得する (プレビュー)

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

[ListItem](../resources/listitem.md) の特定のバージョンのメタデータを取得します。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|            アクセス許可の種類             | アクセス許可 (特権の小さいものから大きいものへ) |
| :------------------------------------- | :------------------------------------------ |
| 委任 (職場または学校のアカウント)     | Sites.Read.All、Sites.ReadWrite.All         |
| 委任 (個人用 Microsoft アカウント) | 該当なし                                         |
| アプリケーション                            | Sites.Read.All、Sites.ReadWrite.All         |


## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored"} -->

```http
GET /sites/{site-id}/items/{item-id}/versions/{version-id}
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}
```


## <a name="response"></a>応答

成功した場合、このメソッドは応答本文で `200 OK` 応答コードと [ListItemVersion](../resources/listitemversion.md) オブジェクトを返します。


## <a name="example"></a>例

この例では、listItem の 1 つのバージョンを取得し、fields コレクションを展開して listItem 内のフィールドの値を要求します。

### <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "request", "name": "get-single-version-listItem", "scopes": "files.read" } -->

```http
GET /sites/{site-id}/items/{item-id}/versions/{version-id}?expand=fields
```

### <a name="response"></a>応答

バージョンのコレクションを返します。

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.listItemVersion", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "id": "1.0",
    "lastModifiedBy": {
    "user": {
        "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
        "displayName": "Ryan Gregg"
    }
    },
    "lastModifiedDateTime": "2017-09-14T12:34:53.912Z",
    "fields": {  }
}
```

<!-- {
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history"
} -->
