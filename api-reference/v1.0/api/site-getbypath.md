---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: パスで SharePoint サイトを取得する
localization_priority: Normal
ms.prod: sharepoint
description: サイトリソースのプロパティとリレーションシップを取得します。
doc_type: apiPageType
ms.openlocfilehash: 5e6195ddb90578d31d4cf68f081aafebbd004e24
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36021474"
---
# <a name="get-a-site-resource-by-path"></a><span data-ttu-id="a2bd3-103">パスを使用したサイト リソースの取得</span><span class="sxs-lookup"><span data-stu-id="a2bd3-103">Get a site resource by path</span></span>

<span data-ttu-id="a2bd3-p101">[サイト][] リソースのプロパティとリレーションシップを取得します。**サイト** リソースは、SharePoint のチーム サイトを表します。</span><span class="sxs-lookup"><span data-stu-id="a2bd3-p101">Retrieve properties and relationships for a [site][] resource. A **site** resource represents a team site in SharePoint.</span></span>

[サイト]: ../resources/site.md
[site]: ../resources/site.md

<span data-ttu-id="a2bd3-107">[ID を使用したサイト](site-get.md)の取得のほかに、サーバーの相対 URL パスに基づいてサイトを取得できます。</span><span class="sxs-lookup"><span data-stu-id="a2bd3-107">In addition to retrieving a [site by ID](site-get.md) you can retrieve a site based on server-relative URL path.</span></span>

* <span data-ttu-id="a2bd3-108">サイト コレクションのホスト名 (contoso.sharepoint.com)</span><span class="sxs-lookup"><span data-stu-id="a2bd3-108">Site collection hostname (contoso.sharepoint.com)</span></span>
* <span data-ttu-id="a2bd3-109">サーバーのホスト名を基準にしたサイトのパス。</span><span class="sxs-lookup"><span data-stu-id="a2bd3-109">Site path, relative to server hostname.</span></span>

<span data-ttu-id="a2bd3-110">予約済みのサイト識別子 `root` もあります。これは次に示すように、常にターゲットのルート サイトを参照します。</span><span class="sxs-lookup"><span data-stu-id="a2bd3-110">There is also a reserved site identifier, `root`, which always references the root site for a given target, as follows:</span></span>

* <span data-ttu-id="a2bd3-111">`/sites/root`:テナントのルート サイト。</span><span class="sxs-lookup"><span data-stu-id="a2bd3-111">`/sites/root`: The tenant root site.</span></span>
* <span data-ttu-id="a2bd3-112">`/groups/{group-id}/sites/root`:グループのチーム サイト。</span><span class="sxs-lookup"><span data-stu-id="a2bd3-112">`/groups/{group-id}/sites/root`: The group's team site.</span></span>

## <a name="permissions"></a><span data-ttu-id="a2bd3-113">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a2bd3-113">Permissions</span></span>

<span data-ttu-id="a2bd3-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a2bd3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2bd3-116">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a2bd3-116">Permission type</span></span>      | <span data-ttu-id="a2bd3-117">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a2bd3-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a2bd3-118">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a2bd3-118">Delegated (work or school account)</span></span> | <span data-ttu-id="a2bd3-119">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2bd3-119">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="a2bd3-120">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a2bd3-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a2bd3-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a2bd3-121">Not supported.</span></span>    |
|<span data-ttu-id="a2bd3-122">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a2bd3-122">Application</span></span> | <span data-ttu-id="a2bd3-123">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2bd3-123">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a2bd3-124">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a2bd3-124">HTTP Request</span></span>

<span data-ttu-id="a2bd3-125">相対パスを使用してルートの SharePoint サイトにアクセスするには、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="a2bd3-125">To access the root SharePoint site with a relative path:</span></span>

<!-- { "blockType": "request", "name": "get-site-by-hostname-and-path", "scopes": "sites.read.all", "tags": "service.sharepoint" } -->

```http
GET /sites/{hostname}:/{relative-path}
```

## <a name="response"></a><span data-ttu-id="a2bd3-126">応答</span><span class="sxs-lookup"><span data-stu-id="a2bd3-126">Response</span></span>

<span data-ttu-id="a2bd3-127">このメソッドは、一意の識別子によって参照されるサイトの[サイト][] リソースを返します。</span><span class="sxs-lookup"><span data-stu-id="a2bd3-127">This method returns a [site][] resource for the site referenced by the unique identifier.</span></span>

<!-- { "blockType": "response", "truncated": true, "@odata.type": "microsoft.graph.site" } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "contoso.sharepoint.com,2C712604-1370-44E7-A1F5-426573FDA80A,2D2244C3-251A-49EA-93A8-39E1C3A060FE",
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
  "suppressions": [
    "Warning: Couldn't serialize request for path /sites/{var}/children/{var} into EDMX: System.InvalidOperationException: Uri path requires navigating into unknown object hierarchy: missing property 'children' on 'site'. Possible issues:
         1) Doc bug where 'children' isn't defined on the resource.      2) Doc bug where 'children' is an example key and should instead be replaced with a placeholder like {item-id} or declared in the sampleKeys annotation.       3) Doc bug where 'site' is supposed to be an entity type, but is being treated as a complex because it (and its ancestors) are missing the keyProperty annotation
     at ApiDocs.Publishing.CSDL.CsdlWriter.ParseRequestTargetType(String requestPath, MethodCollection requestMethodCollection, EntityFramework edmx, IssueLogger issues) in D:/src/mds2/ApiDocs.Publishing/CSDL/CsdlWriter.cs:line 982
     at ApiDocs.Publishing.CSDL.CsdlWriter.ProcessRestRequestPaths(EntityFramework edmx, String[] baseUrlsToRemove, IssueLogger issues) in D:/src/mds2/ApiDocs.Publishing/CSDL/CsdlWriter.cs:line 653"
  ],
  "tocPath": "Sites/Get by path"
} -->
