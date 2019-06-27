---
author: rahmit
ms.author: rahmit
ms.date: 03/15/2018
title: サイト内のページを取得する
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 47a9360d54263cf60213002518df8f39e24f7656
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35271555"
---
# <a name="get-a-page-in-the-site-pages-list-of-a-site"></a><span data-ttu-id="168f1-102">サイトのサイトページリストのページを取得する</span><span class="sxs-lookup"><span data-stu-id="168f1-102">Get a page in the site pages list of a site</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="168f1-103">[サイト][]のサイトページ[リスト][]内の[sitepage][]のメタデータを返します。</span><span class="sxs-lookup"><span data-stu-id="168f1-103">Returns the metadata for a [sitePage][] in the site pages [list][] in a [site][].</span></span>

[sitePage]: ../resources/sitepage.md
[list]: ../resources/list.md
[サイト]: ../resources/site.md
[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="168f1-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="168f1-107">Permissions</span></span>

<span data-ttu-id="168f1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="168f1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="168f1-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="168f1-110">Permission type</span></span>      | <span data-ttu-id="168f1-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="168f1-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="168f1-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="168f1-112">Delegated (work or school account)</span></span> | <span data-ttu-id="168f1-113">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="168f1-113">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="168f1-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="168f1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="168f1-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="168f1-115">Not supported.</span></span>    |
|<span data-ttu-id="168f1-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="168f1-116">Application</span></span> | <span data-ttu-id="168f1-117">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="168f1-117">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="168f1-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="168f1-118">HTTP request</span></span>

```http
GET /sites/{site-id}/pages/{page-id}
```

## <a name="example"></a><span data-ttu-id="168f1-119">例</span><span class="sxs-lookup"><span data-stu-id="168f1-119">Example</span></span>

##### <a name="request"></a><span data-ttu-id="168f1-120">要求</span><span class="sxs-lookup"><span data-stu-id="168f1-120">Request</span></span>

<!-- { "blockType": "request", "name": "get-page", "scopes": "sites.read.all", "tags": "service.sharepoint" } -->

```http
GET /sites/{site-id}/pages/{page-id}
```

##### <a name="response"></a><span data-ttu-id="168f1-121">応答</span><span class="sxs-lookup"><span data-stu-id="168f1-121">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.sitePage", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "2",
    "eTag": "75bc70e2-6587-45be-8493-c99a956b2e05,7",
    "createdDateTime": "2016-12-06T20:04:40Z",
    "lastModifiedDateTime": "2016-12-06T20:05:09Z",
    "webUrl": "https://www.contoso.com/sites/Engineering/SitePages/Events.aspx",
    "createdBy": {
        "user": {
            "email": "rahmit@microsoft.com",
            "id": "1b37d2e1-5000-4648-b431-7dfa509b5660",
            "displayName": "Rahul Mittal (ODSP)"
        }
    },
    "lastModifiedBy": {
        "user": {
            "email": "rahmit@microsoft.com",
            "id": "1b37d2e1-5000-4648-b431-7dfa509b5660",
            "displayName": "Rahul Mittal (ODSP)"
        }
    },
    "parentReference": {
        "id": "eb3bfd48-56f8-4c1e-8312-e58588b22e7c"
    },
    "contentType": {
        "id": "0x0101009D1CB255DA76424F860D91F20E6C411800C9E7033636784C4B88A284B1823C45FD",
        "name": "Site Page"
    },
    "description": "",
    "title": "Upcoming Events",
    "publishingState": {
        "level": "published",
        "versionId": "1.0"
    },
    "webParts": [
        {
            "type": "rte",
            "data": {
                "innerHTML": "<p>Here are the team's upcoming events:</p>"
            }
        },
        {
            "type": "d1d91016-032f-456d-98a4-721247c305e8",
            "data": {
                "title": "Events",
                "description": "Display upcoming events",
                "serverProcessedContent": {
                    "htmlStrings": {},
                    "searchablePlainTexts": {
                        "title": ""
                    },
                    "imageSources": {},
                    "links": {
                        "baseUrl": "https://www.contoso.com/sites/Engineering"
                    },
                    "componentDependencies": {
                        "layoutComponentId": "8ac0c53c-e8d0-4e3e-87d0-7449eb0d4027"
                    }
                },
                "dataVersion": "1.0",
                "properties": {
                    "selectedListId": "032e08ab-89b0-4d8f-bc10-73094233615c",
                    "selectedCategory": "",
                    "dateRangeOption": 0,
                    "startDate": "",
                    "endDate": "",
                    "isOnSeeAllPage": false,
                    "layoutId": "FilmStrip",
                    "dataProviderId": "Event",
                    "webId": "0764c419-1ecc-4126-ba32-0c25ae0fffe8",
                    "siteId": "6b4ffc7a-cfc2-4a76-903a-1cc3686dee23"
                }
            }
        }
    ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="168f1-122">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="168f1-122">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="168f1-123">C#</span><span class="sxs-lookup"><span data-stu-id="168f1-123">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-page-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="168f1-124">Javascript</span><span class="sxs-lookup"><span data-stu-id="168f1-124">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-page-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="168f1-125">目的-C</span><span class="sxs-lookup"><span data-stu-id="168f1-125">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get-page-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!--
{
  "type": "#page.annotation",
  "description": "Get a page in a site",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Pages/Enumerate",
  "suppressions": [
    "Error: /api-reference/beta/api/sitepage-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/sitepage-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/sitepage-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
