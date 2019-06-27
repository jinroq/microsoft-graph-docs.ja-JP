---
title: ListItemVersion リソースを取得する
description: ListItem の特定のバージョンのメタデータを取得します。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 36164373d0df1ddfd69df4d9e5800d52b2363108
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35271961"
---
# <a name="get-a-listitemversion-resource"></a>ListItemVersion リソースを取得する

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

<!-- { "blockType": "request", "name": "get-single-version-listItem", "scopes": "files.read sites.read.all", "tags": "service.graph service.sharepoint" } -->

```http
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}?expand=fields
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
#### <a name="sdk-sample-code"></a>SDK サンプル コード
# <a name="ctabcs"></a>[C#](#tab/cs)
[!INCLUDE [sample-code](../includes/get-single-version-listItem-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-single-version-listItem-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[目的-C](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get-single-version-listItem-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- {
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history",
  "suppressions": [
    "Error: /api-reference/v1.0/api/listitemversion-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/listitemversion-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/listitemversion-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->
