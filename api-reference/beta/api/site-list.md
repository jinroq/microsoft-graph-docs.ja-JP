---
title: サイトの列挙
description: 指定したフィルター条件とクエリオプションに一致する組織内で利用可能な [sites] [] を一覧表示します。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: f61aab6a7a333e83438f5cc6d03c6ac79e277df2
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33638642"
---
# <a name="enumerate-sites"></a>サイトの列挙

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

指定したフィルター条件とクエリオプションに一致する組織内の使用可能な[サイト][]を一覧表示します。

次のクエリオプションのみが現在サポートされています。

| Filter ステートメント             | Select ステートメント        | 説明
|:-----------------------------|:------------------------|:--------------------
|`siteCollection/root ne null` | `siteCollection,webUrl` | 組織内のすべてのルートレベルのサイトコレクションを一覧表示します。 各地域のホームサイトを検出するのに役立ちます。

また、'/サイト ' コレクションに対して**[検索][]** クエリを使用して、特定のキーワードに一致するサイトを検索することもできます。

[探す]: site-search.md
[サイト]: ../resources/site.md

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類                        | アクセス許可 (特権の小さいものから大きいものへ)
|:--------------------------------------|:-------------------------------------
|委任 (職場または学校のアカウント)     | Sites.Read.All、Sites.ReadWrite.All
|委任 (個人用 Microsoft アカウント) | サポートされていません。
|アプリケーション                            | Sites.Read.All、Sites.ReadWrite.All

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->

```http
GET https://graph.microsoft.com/beta/sites?filter=siteCollection/root ne null
```

## <a name="example"></a>例

#### <a name="request"></a>要求

<!-- { "blockType": "request", "name": "list-sites" } -->

```http
GET https://graph.microsoft.com/beta/sites?select=siteCollection,webUrl&filter=siteCollection/root%20ne%20null
```

#### <a name="response"></a>応答

<!-- { "blockType": "response", "@type": "microsoft.graph.site", "isCollection": true, "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "contoso.sharepoint.com,da60e844-ba1d-49bc-b4d4-d5e36bae9019,712a596e-90a1-49e3-9b48-bfa80bee8740",
      "name": "Contoso USA",
      "root": { },
      "siteCollection": {
        "hostname": "contoso.sharepoint.com",
        "dataLocationCode": "NAM",
        "root": { }
      },
      "webUrl": "https://contoso.sharepoint.com"
    },
    {
      "id": "contoso-jpn.sharepoint.com,da60e844-ba1d-49bc-b4d4-d5e36bae9019,0271110f-634f-4300-a841-3a8a2e851851",
      "name": "Contoso Japan",
      "root": { },
      "siteCollection": {
        "hostname": "contoso-jp.sharepoint.com",
        "dataLocationCode": "JPN",
        "root": { }
      },
      "webUrl": "https://contoso-jp.sharepoint.com"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a>SDK サンプルコード
# <a name="ctabcs"></a>[Visual](#tab/cs)
[!INCLUDE [sample-code](../includes/list-sites-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Java](#tab/javascript)
[!INCLUDE [sample-code](../includes/list-sites-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Site/List sites",
  "suppressions": [
    "Error: /api-reference/beta/api/site-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/site-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
