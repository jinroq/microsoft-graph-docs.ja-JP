---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: パスで SharePoint サイトを取得する
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 574b6537fd218b2337f63f5966b267aa60f0f458
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32545262"
---
# <a name="get-a-site-resource-by-path"></a><span data-ttu-id="c71df-102">パスを使用したサイト リソースの取得</span><span class="sxs-lookup"><span data-stu-id="c71df-102">Get a site resource by path</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c71df-p101">[サイト][] リソースのプロパティとリレーションシップを取得します。**サイト** リソースは、SharePoint のチーム サイトを表します。</span><span class="sxs-lookup"><span data-stu-id="c71df-p101">Retrieve properties and relationships for a [site][] resource. A **site** resource represents a team site in SharePoint.</span></span>

[サイト]: ../resources/site.md
[site]: ../resources/site.md

<span data-ttu-id="c71df-106">[ID を使用したサイト](site-get.md)の取得のほかに、サーバーの相対 URL パスに基づいてサイトを取得できます。</span><span class="sxs-lookup"><span data-stu-id="c71df-106">In addition to retrieving a [site by ID](site-get.md) you can retrieve a site based on server-relative URL path.</span></span>

* <span data-ttu-id="c71df-107">サイト コレクションのホスト名 (contoso.sharepoint.com)</span><span class="sxs-lookup"><span data-stu-id="c71df-107">Site collection hostname (contoso.sharepoint.com)</span></span>
* <span data-ttu-id="c71df-108">サーバーのホスト名を基準にしたサイトのパス。</span><span class="sxs-lookup"><span data-stu-id="c71df-108">Site path, relative to server hostname.</span></span>

<span data-ttu-id="c71df-109">予約済みのサイト識別子 `root` もあります。これは次に示すように、常にターゲットのルート サイトを参照します。</span><span class="sxs-lookup"><span data-stu-id="c71df-109">There is also a reserved site identifier, `root`, which always references the root site for a given target, as follows:</span></span>

* <span data-ttu-id="c71df-110">`/sites/root`:テナントのルート サイト。</span><span class="sxs-lookup"><span data-stu-id="c71df-110">`/sites/root`: The tenant root site.</span></span>
* <span data-ttu-id="c71df-111">`/groups/{group-id}/sites/root`:グループのチーム サイト。</span><span class="sxs-lookup"><span data-stu-id="c71df-111">`/groups/{group-id}/sites/root`: The group's team site.</span></span>

## <a name="permissions"></a><span data-ttu-id="c71df-112">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c71df-112">Permissions</span></span>

<span data-ttu-id="c71df-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c71df-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c71df-115">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c71df-115">Permission type</span></span>      | <span data-ttu-id="c71df-116">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c71df-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c71df-117">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c71df-117">Delegated (work or school account)</span></span> | <span data-ttu-id="c71df-118">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c71df-118">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="c71df-119">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c71df-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c71df-120">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c71df-120">Not supported.</span></span>    |
|<span data-ttu-id="c71df-121">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c71df-121">Application</span></span> | <span data-ttu-id="c71df-122">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c71df-122">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c71df-123">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c71df-123">HTTP Request</span></span>

<span data-ttu-id="c71df-124">相対パスを使用してルートの SharePoint サイトにアクセスするには、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="c71df-124">To access the root SharePoint site with a relative path:</span></span>

<!-- { "blockType": "request", "name": "get-site-by-hostname-and-path", "scopes": "service.sharepoint sites.read.all" } -->

```http
GET /sites/{hostname}:/{relative-path}
```

## <a name="response"></a><span data-ttu-id="c71df-125">応答</span><span class="sxs-lookup"><span data-stu-id="c71df-125">Response</span></span>

<span data-ttu-id="c71df-126">このメソッドは、一意の識別子によって参照されるサイトの[サイト][] リソースを返します。</span><span class="sxs-lookup"><span data-stu-id="c71df-126">This method returns a [site][] resource for the site referenced by the unique identifier.</span></span>

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

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites/Get by path",
  "suppressions": [
    "Error: /api-reference/beta/api/site-getbypath.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
