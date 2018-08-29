---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: キーワードで SharePoint サイトを検索する
ms.openlocfilehash: 0f9c562da7509b213e78da85d52a091d9cec421c
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/21/2018
ms.locfileid: "23265359"
---
# <a name="search-for-sites"></a><span data-ttu-id="d7058-102">サイトを検索する</span><span class="sxs-lookup"><span data-stu-id="d7058-102">Search for sites</span></span>

<span data-ttu-id="d7058-103">SharePoint テナント全体で、指定したキーワードと一致する[サイト][]を検索します。</span><span class="sxs-lookup"><span data-stu-id="d7058-103">Search across a SharePoint tenant for [sites][] that match provided keywords.</span></span>

[sites]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="d7058-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d7058-105">Permissions</span></span>

<span data-ttu-id="d7058-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d7058-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d7058-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d7058-108">Permission type</span></span>                        | <span data-ttu-id="d7058-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d7058-109">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="d7058-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d7058-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="d7058-111">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7058-111">Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="d7058-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d7058-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d7058-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d7058-113">Not supported.</span></span>
|<span data-ttu-id="d7058-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d7058-114">Application</span></span>                            | <span data-ttu-id="d7058-115">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7058-115">Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="d7058-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d7058-116">HTTP request</span></span>

<!-- { "blockType": "request", "name": "search-sites", "scopes": "sites.readwrite.all", "tags": "service.sharepoint" } -->

```http
GET /sites?search={query}
```

## <a name="response"></a><span data-ttu-id="d7058-117">応答</span><span class="sxs-lookup"><span data-stu-id="d7058-117">Response</span></span>

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
