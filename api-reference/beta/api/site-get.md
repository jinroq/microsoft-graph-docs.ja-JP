---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharePoint サイトを取得する
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 7ef1a6a3a0bdbcf84cb0e0696e280842a63f4812
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27942368"
---
# <a name="get-a-site-resource"></a><span data-ttu-id="762c9-102">サイト リソースを取得する</span><span class="sxs-lookup"><span data-stu-id="762c9-102">Get a site resource</span></span>

> <span data-ttu-id="762c9-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="762c9-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="762c9-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="762c9-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="762c9-p102">[サイト][] リソースのプロパティとリレーションシップを取得します。**サイト** リソースは、SharePoint のチーム サイトを表します。</span><span class="sxs-lookup"><span data-stu-id="762c9-p102">Retrieve properties and relationships for a [site][] resource. A **site** resource represents a team site in SharePoint.</span></span>

[サイト]: ../resources/site.md
[site]: ../resources/site.md

<span data-ttu-id="762c9-108">**サイト**は、以下の値の複合 ID である、一意識別子にアドレス指定されます。</span><span class="sxs-lookup"><span data-stu-id="762c9-108">A **site** is addressed be a unique identifier which is a composite ID of the following values:</span></span>

* <span data-ttu-id="762c9-109">サイト コレクションのホスト名 (contoso.sharepoint.com)</span><span class="sxs-lookup"><span data-stu-id="762c9-109">Site collection hostname (contoso.sharepoint.com)</span></span>
* <span data-ttu-id="762c9-110">サイト コレクションの一意 ID (GUID)</span><span class="sxs-lookup"><span data-stu-id="762c9-110">Site collection unique ID (GUID)</span></span>
* <span data-ttu-id="762c9-111">サイトの一意 ID (GUID)</span><span class="sxs-lookup"><span data-stu-id="762c9-111">Site unique ID (GUID)</span></span>

<span data-ttu-id="762c9-112">予約済みのサイト識別子 `root` もあります。これは次に示すように、常にターゲットのルート サイトを参照します。</span><span class="sxs-lookup"><span data-stu-id="762c9-112">There is also a reserved site identifier, `root`, which always references the root site for a given target, as follows:</span></span>

* <span data-ttu-id="762c9-113">`/sites/root`:テナントのルート サイト。</span><span class="sxs-lookup"><span data-stu-id="762c9-113">`/sites/root`: The tenant root site.</span></span>
* <span data-ttu-id="762c9-114">`/groups/{group-id}/sites/root`:グループのチーム サイト。</span><span class="sxs-lookup"><span data-stu-id="762c9-114">`/groups/{group-id}/sites/root`: The group's team site.</span></span>

## <a name="permissions"></a><span data-ttu-id="762c9-115">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="762c9-115">Permissions</span></span>

<span data-ttu-id="762c9-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="762c9-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="762c9-118">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="762c9-118">Permission type</span></span>      | <span data-ttu-id="762c9-119">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="762c9-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="762c9-120">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="762c9-120">Delegated (work or school account)</span></span> | <span data-ttu-id="762c9-121">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="762c9-121">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="762c9-122">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="762c9-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="762c9-123">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="762c9-123">Not supported.</span></span>    |
|<span data-ttu-id="762c9-124">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="762c9-124">Application</span></span> | <span data-ttu-id="762c9-125">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="762c9-125">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="get-the-tenants-root-site"></a><span data-ttu-id="762c9-126">テナントのルート サイトを取得する</span><span class="sxs-lookup"><span data-stu-id="762c9-126">Get the tenant's root site</span></span>

<span data-ttu-id="762c9-127">テナント内のルートの SharePoint サイトにアクセスするには次のようにします。</span><span class="sxs-lookup"><span data-stu-id="762c9-127">To access the root SharePoint site within a tenant:</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /sites/root
GET /sites/contoso.sharepoint.com
```

## <a name="access-a-site-by-server-relative-url"></a><span data-ttu-id="762c9-128">サーバーの相対 URL でサイトにアクセスする</span><span class="sxs-lookup"><span data-stu-id="762c9-128">Access a site by server-relative URL</span></span>

<span data-ttu-id="762c9-129">**サイト** リソースのサーバーの相対 URL がある場合、次のように要求を構築することができます。</span><span class="sxs-lookup"><span data-stu-id="762c9-129">If you have the server-relative URL for a **site** resource, you can construct a request as follows:</span></span>

```http
GET /sites/{hostname}:/{server-relative-path}
```

## <a name="access-a-group-team-site"></a><span data-ttu-id="762c9-130">グループのチーム サイトにアクセスする</span><span class="sxs-lookup"><span data-stu-id="762c9-130">Access a group team site</span></span>

<span data-ttu-id="762c9-131">グループのチーム サイトにアクセスするには次のようにします。</span><span class="sxs-lookup"><span data-stu-id="762c9-131">To access the team site for a group:</span></span>

```http
GET /groups/{group-id}/sites/root
```

## <a name="example"></a><span data-ttu-id="762c9-132">例</span><span class="sxs-lookup"><span data-stu-id="762c9-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="762c9-133">要求</span><span class="sxs-lookup"><span data-stu-id="762c9-133">Request</span></span>

<!-- { "blockType": "request", "name": "get-site" } -->

```http
GET /sites/{site-id}
```

### <a name="response"></a><span data-ttu-id="762c9-134">応答</span><span class="sxs-lookup"><span data-stu-id="762c9-134">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.site", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "contoso.sharepoint.com,2C712604-1370-44E7-A1F5-426573FDA80A,2D2244C3-251A-49EA-93A8-39E1C3A060FE",
  "owner": {
    "user": {
      "displayName": "Daron Spektor",
      "id": "5280E7FE-DC7A-4486-9490-E790D81DFEB3"
    }
  },
  "displayName": "OneDrive Team Site",
  "name": "1drvteam",
  "createdDateTime": "2017-05-09T20:56:00Z",
  "lastModifiedDateTime": "2017-05-09T20:56:01Z",
  "webUrl": "https://contoso.sharepoint.com/teams/1drvteam"
}
```

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites/Get by ID"
} -->
