---
author: JeremyKelley
description: ListItem の特定のバージョンのメタデータを取得します。
ms.date: 09/10/2017
title: 旧バージョンのリスト アイテムを取得する - SharePoint API
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 752287ac5e004688e1dd1747f3689c5f460dc946
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35984096"
---
# <a name="get-a-listitemversion-resource-preview"></a>ListItemVersion リソースを取得する (プレビュー)

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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

<!--
{
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history",
  "suppressions": []
}
-->
