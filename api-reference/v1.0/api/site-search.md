---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: キーワードで SharePoint サイトを検索する
ms.openlocfilehash: 8022a49cd545f99df74157f80a133e3e5174a964
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024234"
---
# <a name="search-for-sites"></a><span data-ttu-id="596f5-102">サイトを検索する</span><span class="sxs-lookup"><span data-stu-id="596f5-102">Search for sites</span></span>

<span data-ttu-id="596f5-103">SharePoint テナント全体で、指定したキーワードと一致する[サイト][]を検索します。</span><span class="sxs-lookup"><span data-stu-id="596f5-103">Search across a SharePoint tenant for [sites][] that match provided keywords.</span></span>

[sites]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="596f5-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="596f5-105">Permissions</span></span>

<span data-ttu-id="596f5-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="596f5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="596f5-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="596f5-108">Permission type</span></span>                        | <span data-ttu-id="596f5-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="596f5-109">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="596f5-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="596f5-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="596f5-111">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="596f5-111">Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="596f5-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="596f5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="596f5-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="596f5-113">Not supported.</span></span>
|<span data-ttu-id="596f5-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="596f5-114">Application</span></span>                            | <span data-ttu-id="596f5-115">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="596f5-115">Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="596f5-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="596f5-116">HTTP request</span></span>

<!-- { "blockType": "request", "name": "search-sites", "scopes": "sites.readwrite.all", "tags": "service.sharepoint" } -->

```http
GET /sites?search={query}
```

## <a name="response"></a><span data-ttu-id="596f5-117">応答</span><span class="sxs-lookup"><span data-stu-id="596f5-117">Response</span></span>

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

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites/Search"
} -->