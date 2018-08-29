---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharePoint サイトを取得する
ms.openlocfilehash: f3153845a0ce117c5442b5e66d1e96a388ac6720
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/21/2018
ms.locfileid: "23264064"
---
# <a name="get-a-site-resource"></a><span data-ttu-id="58379-102">サイト リソースを取得する</span><span class="sxs-lookup"><span data-stu-id="58379-102">Get a site resource</span></span>

<span data-ttu-id="58379-p101">[サイト][] リソースのプロパティとリレーションシップを取得します。**サイト** リソースは、SharePoint のチーム サイトを表します。</span><span class="sxs-lookup"><span data-stu-id="58379-p101">Retrieve properties and relationships for a [site][] resource. A **site** resource represents a team site in SharePoint.</span></span>

[サイト]: ../resources/site.md
[site]: ../resources/site.md

<span data-ttu-id="58379-106">**サイト**は、以下の値の複合 ID である、一意識別子にアドレス指定されます。</span><span class="sxs-lookup"><span data-stu-id="58379-106">A **site** is addressed be a unique identifier which is a composite ID of the following values:</span></span>

* <span data-ttu-id="58379-107">サイト コレクションのホスト名 (contoso.sharepoint.com)</span><span class="sxs-lookup"><span data-stu-id="58379-107">Site collection hostname (contoso.sharepoint.com)</span></span>
* <span data-ttu-id="58379-108">サイト コレクションの一意 ID (GUID)</span><span class="sxs-lookup"><span data-stu-id="58379-108">Site collection unique ID (GUID)</span></span>
* <span data-ttu-id="58379-109">サイトの一意 ID (GUID)</span><span class="sxs-lookup"><span data-stu-id="58379-109">Site unique ID (GUID)</span></span>

<span data-ttu-id="58379-110">予約済みのサイト識別子 `root` もあります。これは次に示すように、常にターゲットのルート サイトを参照します。</span><span class="sxs-lookup"><span data-stu-id="58379-110">There is also a reserved site identifier, `root`, which always references the root site for a given target, as follows:</span></span>

* <span data-ttu-id="58379-111">`/sites/root`:テナントのルート サイト。</span><span class="sxs-lookup"><span data-stu-id="58379-111">`/sites/root`: The tenant root site.</span></span>
* <span data-ttu-id="58379-112">`/groups/{group-id}/sites/root`:グループのチーム サイト。</span><span class="sxs-lookup"><span data-stu-id="58379-112">`/groups/{group-id}/sites/root`: The group's team site.</span></span>

## <a name="permissions"></a><span data-ttu-id="58379-113">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="58379-113">Permissions</span></span>

<span data-ttu-id="58379-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="58379-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="58379-116">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="58379-116">Permission type</span></span>      | <span data-ttu-id="58379-117">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="58379-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="58379-118">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="58379-118">Delegated (work or school account)</span></span> | <span data-ttu-id="58379-119">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58379-119">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="58379-120">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="58379-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="58379-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="58379-121">Not supported.</span></span>    |
|<span data-ttu-id="58379-122">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="58379-122">Application</span></span> | <span data-ttu-id="58379-123">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58379-123">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="get-the-tenants-root-site"></a><span data-ttu-id="58379-124">テナントのルート サイトを取得する</span><span class="sxs-lookup"><span data-stu-id="58379-124">Get the tenant's root site</span></span>

<span data-ttu-id="58379-125">テナント内のルートの SharePoint サイトにアクセスするには次のようにします。</span><span class="sxs-lookup"><span data-stu-id="58379-125">To access the root SharePoint site within a tenant:</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /sites/root
GET /sites/contoso.sharepoint.com
```

## <a name="access-a-site-by-server-relative-url"></a><span data-ttu-id="58379-126">サーバーの相対 URL でサイトにアクセスする</span><span class="sxs-lookup"><span data-stu-id="58379-126">Access a site by server-relative URL</span></span>

<span data-ttu-id="58379-127">**サイト** リソースのサーバーの相対 URL がある場合、次のように要求を構築することができます。</span><span class="sxs-lookup"><span data-stu-id="58379-127">If you have the server-relative URL for a **site** resource, you can construct a request as follows:</span></span>

```http
GET /sites/{hostname}:/{server-relative-path}
```

## <a name="access-a-group-team-site"></a><span data-ttu-id="58379-128">グループのチーム サイトにアクセスする</span><span class="sxs-lookup"><span data-stu-id="58379-128">Access a group team site</span></span>

<span data-ttu-id="58379-129">グループのチーム サイトにアクセスするには次のようにします。</span><span class="sxs-lookup"><span data-stu-id="58379-129">To access the team site for a group:</span></span>

```http
GET /groups/{group-id}/sites/root
```

## <a name="example"></a><span data-ttu-id="58379-130">例</span><span class="sxs-lookup"><span data-stu-id="58379-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="58379-131">要求</span><span class="sxs-lookup"><span data-stu-id="58379-131">Request</span></span>

<!-- { "blockType": "request", "name": "get-site", "scopes": "sites.read.all" } -->

```http
GET /sites/{site-id}
```

### <a name="response"></a><span data-ttu-id="58379-132">応答</span><span class="sxs-lookup"><span data-stu-id="58379-132">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.site", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

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
  "tocPath": "Sites/Get by ID"
} -->
