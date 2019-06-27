---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: SharePoint リストを作成する
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: d0de56a1fac8ecaa15e0f54ba0dda48d19cf868d
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35264585"
---
# <a name="create-a-new-list"></a>新しいリストを作成する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[site][] で新しい [list][] を作成します。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|            アクセス許可の種類             | アクセス許可 (特権の小さいものから大きいものへ) |
| :------------------------------------- | :------------------------------------------ |
| 委任 (職場または学校のアカウント)     | Sites.Manage.All                            |
| 委任 (個人用 Microsoft アカウント) | サポートされていません。                              |
| アプリケーション                            | Sites.ReadWrite.All                         |

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->

```http
POST https://graph.microsoft.com/beta/sites/{site-id}/lists
```

## <a name="request-body"></a>要求本文

要求本文で、作成する [list][] リソースの JSON 表記を指定します。

## <a name="example"></a>例

新しい汎用リストを作成する例を次に示します。

<!-- { "blockType": "request", "name": "create-list", "scopes": "sites.readwrite.all" } -->

```http
POST /sites/{site-id}/lists
Content-Type: application/json

{
  "displayName": "Books",
  "columns": [
    {
      "name": "Author",
      "text": { }
    },
    {
      "name": "PageCount",
      "number": { }
    }
  ],
  "list": {
    "template": "genericList"
  }
}
```

**注:** カスタム列はオプションです。

ここで指定した列だけでなく、参照された **template** で定義された列も含めて、新しいリストが作成されます。
**list** ファセットまたは **template** が指定されていない場合、リストは既定で _Title_ 列を含む `genericList` テンプレートとなります。

## <a name="response"></a>応答

成功した場合、このメソッドは作成されたリストの応答本文で [list][] を返します。

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.list", "truncated": true } -->

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "22e03ef3-6ef4-424d-a1d3-92a337807c30",
  "createdDateTime": "2017-04-30T01:21:00Z",
  "createdBy": {
    "user": {
      "displayName": "Ryan Gregg",
      "id": "8606e4d5-d582-4f5f-aeba-7d7c18b20cfd"
    }
  },
  "lastModifiedDateTime": "2016-08-30T08:26:00Z",
  "lastModifiedBy": {
    "user": {
      "displayName": "Ryan Gregg",
      "id": "8606e4d5-d582-4f5f-aeba-7d7c18b20cfd"
    }
  }
}
```
#### <a name="sdk-sample-code"></a>SDK サンプル コード
# <a name="ctabcs"></a>[C#](#tab/cs)
[!INCLUDE [sample-code](../includes/create-list-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/create-list-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[目的-C](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create-list-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

**注:** 応答オブジェクトは、わかりやすくするために切り詰められています。
実際の呼び出しでは、既定のプロパティが返されます。

[list]: ../resources/list.md
[サイト]: ../resources/site.md

<!--
{
  "type": "#page.annotation",
  "description": "Create a new SharePoint list.",
  "keywords": "",
  "section": "documentation",
  "tocPath": "List/Create",
  "suppressions": [
    "Error: /api-reference/beta/api/list-create.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/list-create.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/list-create.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
