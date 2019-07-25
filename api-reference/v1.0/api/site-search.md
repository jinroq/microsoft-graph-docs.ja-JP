---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: サイトを検索する
description: 提供されたキーワードに一致するサイトの SharePoint テナント全体を検索します。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 9815eb67128e5b13611d142f2c595efb169b80e7
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35892219"
---
# <a name="search-for-sites"></a><span data-ttu-id="9fb81-103">サイトを検索する</span><span class="sxs-lookup"><span data-stu-id="9fb81-103">Search for sites</span></span>

<span data-ttu-id="9fb81-104">提供されたキーワードに一致する[サイト][]の SharePoint テナント全体を検索します。</span><span class="sxs-lookup"><span data-stu-id="9fb81-104">Search across a SharePoint tenant for [sites][] that match keywords provided.</span></span>

[サイト]: ../resources/site.md
[sites]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="9fb81-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9fb81-106">Permissions</span></span>

<span data-ttu-id="9fb81-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9fb81-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9fb81-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9fb81-109">Permission type</span></span>                        | <span data-ttu-id="9fb81-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9fb81-110">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="9fb81-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9fb81-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9fb81-112">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9fb81-112">Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="9fb81-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9fb81-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9fb81-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9fb81-114">Not supported.</span></span>
|<span data-ttu-id="9fb81-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9fb81-115">Application</span></span>                            | <span data-ttu-id="9fb81-116">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9fb81-116">Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="9fb81-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9fb81-117">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="9fb81-118">プロトコル</span><span class="sxs-lookup"><span data-stu-id="9fb81-118">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "search-sites", "scopes": "sites.readwrite.all", "tags": "service.sharepoint" } -->

```http
GET /sites?search={query}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9fb81-119">C#</span><span class="sxs-lookup"><span data-stu-id="9fb81-119">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/search-sites-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9fb81-120">Javascript</span><span class="sxs-lookup"><span data-stu-id="9fb81-120">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/search-sites-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9fb81-121">目的-C</span><span class="sxs-lookup"><span data-stu-id="9fb81-121">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/search-sites-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="9fb81-122">Java</span><span class="sxs-lookup"><span data-stu-id="9fb81-122">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/search-sites-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="9fb81-123">応答</span><span class="sxs-lookup"><span data-stu-id="9fb81-123">Response</span></span>

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
><span data-ttu-id="9fb81-124">**注:** 並べ替えに使用できる唯一のプロパティは、"**日付**1" です。</span><span class="sxs-lookup"><span data-stu-id="9fb81-124">**Note:** The only property that works for sorting is **createdDateTime**.</span></span> <span data-ttu-id="9fb81-125">検索フィルターは、検索結果を取得するときに複数のプロパティを使用する自由なテキスト検索です。</span><span class="sxs-lookup"><span data-stu-id="9fb81-125">The search filter is a free text search that uses multiple properties when retrieving the search results.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites/Search",
  "suppressions": [
  ]
} -->
