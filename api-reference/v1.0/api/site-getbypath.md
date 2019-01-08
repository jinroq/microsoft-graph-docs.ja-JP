---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: パスを使用した SharePoint サイトの取得
ms.openlocfilehash: 5cac58e32df30435eb927a466ead6f0b5d9c9468
ms.sourcegitcommit: 37591c2299c80e7675cd2b5f781e1eeeba628a60
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/08/2019
ms.locfileid: "27748522"
---
# <a name="get-a-site-resource-by-path"></a><span data-ttu-id="52663-102">パスを使用したサイト リソースの取得</span><span class="sxs-lookup"><span data-stu-id="52663-102">Get a site resource by path</span></span>

<span data-ttu-id="52663-p101">[サイト][] リソースのプロパティとリレーションシップを取得します。**サイト** リソースは、SharePoint のチーム サイトを表します。</span><span class="sxs-lookup"><span data-stu-id="52663-p101">Retrieve properties and relationships for a [site][] resource. A **site** resource represents a team site in SharePoint.</span></span>

[サイト]: ../resources/site.md
[site]: ../resources/site.md

<span data-ttu-id="52663-106">[ID を使用したサイト](site-get.md)の取得のほかに、サーバーの相対 URL パスに基づいてサイトを取得できます。</span><span class="sxs-lookup"><span data-stu-id="52663-106">In addition to retrieving a [site by ID](site-get.md) you can retrieve a site based on server-relative URL path.</span></span>

* <span data-ttu-id="52663-107">サイト コレクションのホスト名 (contoso.sharepoint.com)</span><span class="sxs-lookup"><span data-stu-id="52663-107">Site collection hostname (contoso.sharepoint.com)</span></span>
* <span data-ttu-id="52663-108">サーバーのホスト名を基準にしたサイトのパス。</span><span class="sxs-lookup"><span data-stu-id="52663-108">Site path, relative to server hostname.</span></span>

<span data-ttu-id="52663-109">予約済みのサイト識別子 `root` もあります。これは次に示すように、常にターゲットのルート サイトを参照します。</span><span class="sxs-lookup"><span data-stu-id="52663-109">There is also a reserved site identifier, `root`, which always references the root site for a given target, as follows:</span></span>

* <span data-ttu-id="52663-110">`/sites/root`:テナントのルート サイト。</span><span class="sxs-lookup"><span data-stu-id="52663-110">`/sites/root`: The tenant root site.</span></span>
* <span data-ttu-id="52663-111">`/groups/{group-id}/sites/root`:グループのチーム サイト。</span><span class="sxs-lookup"><span data-stu-id="52663-111">`/groups/{group-id}/sites/root`: The group's team site.</span></span>

## <a name="permissions"></a><span data-ttu-id="52663-112">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="52663-112">Permissions</span></span>

<span data-ttu-id="52663-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="52663-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52663-115">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="52663-115">Permission type</span></span>      | <span data-ttu-id="52663-116">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="52663-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="52663-117">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="52663-117">Delegated (work or school account)</span></span> | <span data-ttu-id="52663-118">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52663-118">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="52663-119">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="52663-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="52663-120">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="52663-120">Not supported.</span></span>    |
|<span data-ttu-id="52663-121">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="52663-121">Application</span></span> | <span data-ttu-id="52663-122">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52663-122">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="52663-123">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="52663-123">HTTP Request</span></span>

<span data-ttu-id="52663-124">相対パスを使用してルートの SharePoint サイトにアクセスするには、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="52663-124">To access the root SharePoint site with a relative path:</span></span>

<!-- { "blockType": "request", "name": "get-site-by-hostname-and-path", "scopes": "sites.read.all", "tags": "service.sharepoint" } -->

```http
GET /sites/{hostname}:/{relative-path}
```

## <a name="response"></a><span data-ttu-id="52663-125">応答</span><span class="sxs-lookup"><span data-stu-id="52663-125">Response</span></span>

<span data-ttu-id="52663-126">このメソッドは、一意の識別子によって参照されるサイトの[サイト][] リソースを返します。</span><span class="sxs-lookup"><span data-stu-id="52663-126">This method returns a [site][] resource for the site referenced by the unique identifier.</span></span>

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
