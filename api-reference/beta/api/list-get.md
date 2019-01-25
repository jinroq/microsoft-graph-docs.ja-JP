---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: SharePoint リストを取得する
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: f796d7b02750034be6d2205a4a25f51c2911f5f2
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521657"
---
# <a name="get-metadata-for-a-list"></a>リストのメタデータを取得する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[list][] のメタデータを返します。

[list]: ../resources/list.md

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Sites.Read.All、Sites.ReadWrite.All    |
|委任 (個人用 Microsoft アカウント) | サポートされていません。    |
|アプリケーション | Sites.Read.All、Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP 要求

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}?expand=columns,items(expand=fields)
```

## <a name="request-body"></a>要求本文

このメソッドには、要求本文を指定しません。

## <a name="example"></a>例

#### <a name="request"></a>要求

<!-- { "blockType": "request", "name": "get-list" } -->

```http
GET /sites/{site-id}/lists/{list-id}
```

#### <a name="response"></a>応答

<!-- { "blockType": "response", "@type": "microsoft.graph.list", "truncated": true, "scopes": "sites.read.all service.sharepoint" } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "1234-112-112-4",
  "name": "MicroFeed",
  "createdDateTime": "2016-08-30T08:32:00Z",
  "lastModifiedDateTime": "2016-08-30T08:32:00Z",
  "list": {
    "hidden": false,
    "template": "genericList"
    }
}
```

`select` ステートメントと `expand` ステートメントを使用すれば、リストのメタデータ、列定義、リスト アイテムを単一の要求で取得できます。

#### <a name="request"></a>要求

<!-- { "blockType": "request", "name": "get-list-multi-expand" } -->

```http
GET /sites/{site-id}/lists/{list-id}?select=name,lastModifiedDateTime&expand=columns(select=name,description),items(expand=fields(select=Name,Color,Quantity))
```

#### <a name="response"></a>応答

<!-- { "blockType": "response", "@type": "microsoft.graph.list", "truncated": true, "scopes": "sites.read.all service.sharepoint" } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "name": "Inventory",
  "lastModifiedDateTime": "2016-08-30T08:32:00Z",
  "columns": [
    {
      "name": "Name",
      "description": "Customer-facing name of the SKU"
    },
    {
      "name": "Color",
      "description": "Color of the item in stock"
    },
    {
      "name": "Quantity",
      "description": "Number of items in stock"
    }
  ],
  "items": [
    {
      "id": "2",
      "fields": {
        "Name": "Gadget",
        "Color": "Red",
        "Quantity": 503
       }
    },
    {
      "id": "4",
      "fields": {
        "Name": "Widget",
        "Color": "Blue",
        "Quantity": 2357
       }
    },
    {
      "id": "7",
      "fields": {
        "Name": "Gizmo",
        "Color": "Green",
        "Quantity": 92
       }
    }
  ]
}
```

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Lists/Get metadata",
  "suppressions": [
    "Error: /api-reference/beta/api/list-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
