---
author: JeremyKelley
description: 提供されたキーワードに一致するサイトの SharePoint テナント全体を検索します。
ms.date: 09/10/2017
title: キーワードで SharePoint サイトを検索する
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: dbc66bc734d4ef0a47e30ce1e967918e964489a0
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/04/2019
ms.locfileid: "36724534"
---
# <a name="search-for-sites"></a>サイトを検索する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

提供されたキーワードに一致する[サイト][]の SharePoint テナント全体を検索します。

[サイト]: ../resources/site.md

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類                        | アクセス許可 (特権の小さいものから大きいものへ)
|:--------------------------------------|:-------------------------------------
|委任 (職場または学校のアカウント)     | Sites.Read.All、Sites.ReadWrite.All
|委任 (個人用 Microsoft アカウント) | サポートされていません。
|アプリケーション                            | Sites.Read.All、Sites.ReadWrite.All

## <a name="http-request"></a>HTTP 要求


# <a name="httptabhttp"></a>[プロトコル](#tab/http)
<!-- { "blockType": "request", "name": "search-sites", "scopes": "service.sharepoint sites.readwrite.all" } -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/sites?search={query}
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/search-sites-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/search-sites-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[目的-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/search-sites-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a>応答

<!-- { "blockType": "response", "@type": "Collection(microsoft.graph.site)", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "contoso.sharepoint.com,da60e844-ba1d-49bc-b4d4-d5e36bae9019,712a596e-90a1-49e3-9b48-bfa80bee8740",
      "name": "Team A Site",
      "description": "",
      "createdDateTime": "2016-10-18T03:05:59Z",
      "lastModifiedDateTime": "2016-10-18T10:40:59Z",
      "webUrl": "https://contoso.sharepoint.com/sites/siteA"
    },
    {
      "id": "contoso.sharepoint.com,da60e844-ba1d-49bc-b4d4-d5e36bae9019,0271110f-634f-4300-a841-3a8a2e851851",
      "name": "Team B Site",
      "description": "",
      "createdDateTime": "2016-10-18T03:05:59Z",
      "lastModifiedDateTime": "2016-10-18T10:40:59Z",
      "webUrl": "https://contoso.sharepoint.com/sites/siteB"
    }
  ]
}
```
>**注:** 並べ替えに使用できる唯一のプロパティは、"**日付**1" です。 検索フィルターは、検索結果を取得するときに複数のプロパティを使用する自由なテキスト検索です。

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites/Search",
  "suppressions": [
  ]
}
-->
