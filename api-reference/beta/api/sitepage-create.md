---
author: rahmit
ms.author: rahmit
ms.date: 05/07/2018
title: SharePoint サイトに新しいページを作成します。
ms.openlocfilehash: 142b34a56f4971d8228ba6761bc7a3a9e2f48caf
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072900"
---
# <a name="create-a-page-in-the-site-pages-list-of-a-site"></a><span data-ttu-id="d02bb-102">サイトのサイトのページ一覧でページを作成します。</span><span class="sxs-lookup"><span data-stu-id="d02bb-102">Create a page in the site pages list of a site</span></span>

> <span data-ttu-id="d02bb-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d02bb-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d02bb-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d02bb-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d02bb-105">[サイト][]のサイトのページ[] ボックスの一覧][]で、新しい[sitePage][]を作成します。</span><span class="sxs-lookup"><span data-stu-id="d02bb-105">Create a new [sitePage][] in the site pages [list][] in a [site][].</span></span>

## <a name="permissions"></a><span data-ttu-id="d02bb-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d02bb-106">Permissions</span></span>

<span data-ttu-id="d02bb-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d02bb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d02bb-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d02bb-109">Permission type</span></span>      | <span data-ttu-id="d02bb-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d02bb-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d02bb-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d02bb-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d02bb-112">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d02bb-112">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="d02bb-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d02bb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d02bb-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d02bb-114">Not supported.</span></span>    |
|<span data-ttu-id="d02bb-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d02bb-115">Application</span></span> | <span data-ttu-id="d02bb-116">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d02bb-116">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d02bb-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d02bb-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /sites/{site-id}/pages
```

## <a name="request-body"></a><span data-ttu-id="d02bb-118">要求本文</span><span class="sxs-lookup"><span data-stu-id="d02bb-118">Request body</span></span>

<span data-ttu-id="d02bb-119">要求の本体を作成する[sitePage][]リソースの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="d02bb-119">In the request body, supply a JSON representation of the [sitePage][] resource to create.</span></span>

## <a name="example"></a><span data-ttu-id="d02bb-120">使用例</span><span class="sxs-lookup"><span data-stu-id="d02bb-120">Example</span></span>

<span data-ttu-id="d02bb-121">次の例では、新しいページを作成する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="d02bb-121">The following example shows how to create a new page.</span></span>

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

## <a name="response"></a><span data-ttu-id="d02bb-122">応答</span><span class="sxs-lookup"><span data-stu-id="d02bb-122">Response</span></span>

<span data-ttu-id="d02bb-123">成功した場合、このメソッドは、作成されたページの応答の本体で、 [sitePage][]を返します。</span><span class="sxs-lookup"><span data-stu-id="d02bb-123">If successful, this method returns a [sitePage][] in the response body for the created page.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.sitePage", "truncated": true } -->

```json
HTTP/1.1 201 Created
Content-type: application/json

{
    "id": 2,
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

<span data-ttu-id="d02bb-124">**注:** 応答オブジェクトは、わかりやすくするために切り詰められています。</span><span class="sxs-lookup"><span data-stu-id="d02bb-124">**Note:** The response object is truncated for clarity.</span></span> <span data-ttu-id="d02bb-125">実際の呼び出しでは、既定のプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="d02bb-125">Default properties will be returned from the actual call.</span></span>

[list]: ../resources/list.md
[listItem]: ../resources/listitem.md
[site]: ../resources/site.md
[sitePage]: ../resources/sitepage.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a sitePage in the SitePages list in a site.",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Pages/Create"
} -->
