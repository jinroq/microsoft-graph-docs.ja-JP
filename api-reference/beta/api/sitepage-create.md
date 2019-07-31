---
author: rahmit
description: サイトの [サイトページ] リストに新しいサイトページを作成します。
ms.date: 05/07/2018
title: SharePoint サイトで新しいページを作成する
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: bb54af97b1a2527893c5090e52e5bb7aa8381c94
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35977868"
---
# <a name="create-a-page-in-the-site-pages-list-of-a-site"></a><span data-ttu-id="65398-103">サイトのサイトページリストにページを作成する</span><span class="sxs-lookup"><span data-stu-id="65398-103">Create a page in the site pages list of a site</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="65398-104">[サイト][]の [サイトページ[] リスト][]に新しいサイト[ページ][]を作成します。</span><span class="sxs-lookup"><span data-stu-id="65398-104">Create a new [sitePage][] in the site pages [list][] in a [site][].</span></span>

## <a name="permissions"></a><span data-ttu-id="65398-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="65398-105">Permissions</span></span>

<span data-ttu-id="65398-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="65398-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65398-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="65398-108">Permission type</span></span>      | <span data-ttu-id="65398-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="65398-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="65398-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="65398-110">Delegated (work or school account)</span></span> | <span data-ttu-id="65398-111">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65398-111">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="65398-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="65398-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="65398-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="65398-113">Not supported.</span></span>    |
|<span data-ttu-id="65398-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="65398-114">Application</span></span> | <span data-ttu-id="65398-115">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65398-115">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="65398-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="65398-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /sites/{site-id}/pages
```

## <a name="request-body"></a><span data-ttu-id="65398-117">要求本文</span><span class="sxs-lookup"><span data-stu-id="65398-117">Request body</span></span>

<span data-ttu-id="65398-118">要求本文で、作成する[Sitepage][]リソースの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="65398-118">In the request body, supply a JSON representation of the [sitePage][] resource to create.</span></span>

## <a name="example"></a><span data-ttu-id="65398-119">例</span><span class="sxs-lookup"><span data-stu-id="65398-119">Example</span></span>

<span data-ttu-id="65398-120">次の例は、新しいページを作成する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="65398-120">The following example shows how to create a new page.</span></span>

<!-- { "blockType": "request", "name": "create-page", "scopes": "sites.readwrite.all" } -->

```json
POST /sites/{site-id}/page
Content-Type: application/json

{
    "name": "Events.aspx",
    "title": "Team Events",
    "publishingState": {
        "level": "checkedOut",
        "versionId": "0.1"
    },
    "webParts": [
        {
            "type": "rte",
            "innerHTML": "<p>Here are the team's upcoming events:</p>"
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

## <a name="response"></a><span data-ttu-id="65398-121">応答</span><span class="sxs-lookup"><span data-stu-id="65398-121">Response</span></span>

<span data-ttu-id="65398-122">成功した場合、このメソッドは作成されたページの応答本文で[Sitepage][]を返します。</span><span class="sxs-lookup"><span data-stu-id="65398-122">If successful, this method returns a [sitePage][] in the response body for the created page.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.sitePage", "truncated": true } -->

```json
HTTP/1.1 201 Created
Content-type: application/json

{
    "id": "2",
    "eTag": "75bc70e2-6587-45be-8493-c99a956b2e05,7",
    "createdDateTime": "2016-12-06T20:04:40Z",
    "lastModifiedDateTime": "2016-12-06T20:05:09Z",
    "webUrl": "https://www.contoso.com/sites/Engineering/SitePages/Events.aspx",
    "createdBy": {
        "user": {
            "email": "rahmit",
            "id": "1b37d2e1-5000-4648-b431-7dfa509b5660",
            "displayName": "Rahul Mittal"
        }
    },
    "lastModifiedBy": {
        "user": {
            "email": "rahmit",
            "id": "1b37d2e1-5000-4648-b431-7dfa509b5660",
            "displayName": "Rahul Mittal"
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
    "title": "Team Events",
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
                        "baseUrl": "https://www.contoso.com/teams/Engineering"
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

<span data-ttu-id="65398-123">**注:** 応答オブジェクトは、わかりやすくするために切り詰められています。</span><span class="sxs-lookup"><span data-stu-id="65398-123">**Note:** The response object is truncated for clarity.</span></span> <span data-ttu-id="65398-124">実際の呼び出しでは、既定のプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="65398-124">Default properties will be returned from the actual call.</span></span>

[list]: ../resources/list.md
[listItem]: ../resources/listitem.md
[サイト]: ../resources/site.md
[site]: ../resources/site.md
[sitePage]: ../resources/sitepage.md

<!--
{
  "type": "#page.annotation",
  "description": "Create a sitePage in the SitePages list in a site.",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Pages/Create",
  "suppressions": []
}
-->
