---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: パスを使用した SharePoint サイトの取得
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: afded48114342e8bf5eb76d25f1361f67686af54
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27936187"
---
# <a name="get-a-site-resource-by-path"></a><span data-ttu-id="db1cd-102">パスを使用したサイト リソースの取得</span><span class="sxs-lookup"><span data-stu-id="db1cd-102">Get a site resource by path</span></span>

> <span data-ttu-id="db1cd-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="db1cd-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="db1cd-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="db1cd-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="db1cd-p102">[サイト][] リソースのプロパティとリレーションシップを取得します。**サイト** リソースは、SharePoint のチーム サイトを表します。</span><span class="sxs-lookup"><span data-stu-id="db1cd-p102">Retrieve properties and relationships for a [site][] resource. A **site** resource represents a team site in SharePoint.</span></span>

[サイト]: ../resources/site.md
[site]: ../resources/site.md

<span data-ttu-id="db1cd-108">[ID を使用したサイト](site-get.md)の取得のほかに、サーバーの相対 URL パスに基づいてサイトを取得できます。</span><span class="sxs-lookup"><span data-stu-id="db1cd-108">In addition to retrieving a [site by ID](site-get.md) you can retrieve a site based on server-relative URL path.</span></span>

* <span data-ttu-id="db1cd-109">サイト コレクションのホスト名 (contoso.sharepoint.com)</span><span class="sxs-lookup"><span data-stu-id="db1cd-109">Site collection hostname (contoso.sharepoint.com)</span></span>
* <span data-ttu-id="db1cd-110">サーバーのホスト名を基準にしたサイトのパス。</span><span class="sxs-lookup"><span data-stu-id="db1cd-110">Site path, relative to server hostname.</span></span>

<span data-ttu-id="db1cd-111">予約済みのサイト識別子 `root` もあります。これは次に示すように、常にターゲットのルート サイトを参照します。</span><span class="sxs-lookup"><span data-stu-id="db1cd-111">There is also a reserved site identifier, `root`, which always references the root site for a given target, as follows:</span></span>

* <span data-ttu-id="db1cd-112">`/sites/root`:テナントのルート サイト。</span><span class="sxs-lookup"><span data-stu-id="db1cd-112">`/sites/root`: The tenant root site.</span></span>
* <span data-ttu-id="db1cd-113">`/groups/{group-id}/sites/root`:グループのチーム サイト。</span><span class="sxs-lookup"><span data-stu-id="db1cd-113">`/groups/{group-id}/sites/root`: The group's team site.</span></span>

## <a name="permissions"></a><span data-ttu-id="db1cd-114">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="db1cd-114">Permissions</span></span>

<span data-ttu-id="db1cd-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="db1cd-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db1cd-117">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="db1cd-117">Permission type</span></span>      | <span data-ttu-id="db1cd-118">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="db1cd-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="db1cd-119">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="db1cd-119">Delegated (work or school account)</span></span> | <span data-ttu-id="db1cd-120">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db1cd-120">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="db1cd-121">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="db1cd-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db1cd-122">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="db1cd-122">Not supported.</span></span>    |
|<span data-ttu-id="db1cd-123">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="db1cd-123">Application</span></span> | <span data-ttu-id="db1cd-124">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db1cd-124">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="db1cd-125">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="db1cd-125">HTTP Request</span></span>

<span data-ttu-id="db1cd-126">相対パスを使用してルートの SharePoint サイトにアクセスするには、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="db1cd-126">To access the root SharePoint site with a relative path:</span></span>

<!-- { "blockType": "request", "name": "get-site-by-hostname-and-path", "scopes": "service.sharepoint sites.read.all" } -->

```http
GET /sites/{hostname}:/{relative-path}
```

## <a name="response"></a><span data-ttu-id="db1cd-127">応答</span><span class="sxs-lookup"><span data-stu-id="db1cd-127">Response</span></span>

<span data-ttu-id="db1cd-128">このメソッドは、一意の識別子によって参照されるサイトの[サイト][] リソースを返します。</span><span class="sxs-lookup"><span data-stu-id="db1cd-128">This method returns a [site][] resource for the site referenced by the unique identifier.</span></span>

<!-- { "blockType": "response", "truncated": true, "@odata.type": "microsoft.graph.site" } -->

```http
HTTP/1.1 200 OK

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
  "tocPath": "Sites/Get by path"
} -->
