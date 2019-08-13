---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SharePoint サイトを取得する
localization_priority: Priority
ms.prod: sharepoint
description: サイト リソースのプロパティと関係を取得します。
doc_type: apiPageType
ms.openlocfilehash: 051c49468adfdc60508b93932e0b56b2b363c988
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36320027"
---
# <a name="get-a-site-resource"></a><span data-ttu-id="58bf2-103">サイト リソースを取得する</span><span class="sxs-lookup"><span data-stu-id="58bf2-103">Get a site resource</span></span>

<span data-ttu-id="58bf2-p101">[サイト][] リソースのプロパティとリレーションシップを取得します。**サイト** リソースは、SharePoint のチーム サイトを表します。</span><span class="sxs-lookup"><span data-stu-id="58bf2-p101">Retrieve properties and relationships for a [site][] resource. A **site** resource represents a team site in SharePoint.</span></span>

[サイト]: ../resources/site.md
[site]: ../resources/site.md

<span data-ttu-id="58bf2-107">**サイト**は、次の値の複合 ID である一意の識別子によってアドレス指定されます。</span><span class="sxs-lookup"><span data-stu-id="58bf2-107">A **site** is addressed by a unique identifier which is a composite ID of the following values:</span></span>

* <span data-ttu-id="58bf2-108">サイト コレクションのホスト名 (contoso.sharepoint.com)</span><span class="sxs-lookup"><span data-stu-id="58bf2-108">Site collection hostname (contoso.sharepoint.com)</span></span>
* <span data-ttu-id="58bf2-109">サイト コレクションの一意 ID (GUID)</span><span class="sxs-lookup"><span data-stu-id="58bf2-109">Site collection unique ID (GUID)</span></span>
* <span data-ttu-id="58bf2-110">サイトの一意 ID (GUID)</span><span class="sxs-lookup"><span data-stu-id="58bf2-110">Site unique ID (GUID)</span></span>

<span data-ttu-id="58bf2-111">予約済みのサイト識別子 `root` もあります。これは次に示すように、常にターゲットのルート サイトを参照します。</span><span class="sxs-lookup"><span data-stu-id="58bf2-111">There is also a reserved site identifier, `root`, which always references the root site for a given target, as follows:</span></span>

* <span data-ttu-id="58bf2-112">`/sites/root`:テナントのルート サイト。</span><span class="sxs-lookup"><span data-stu-id="58bf2-112">`/sites/root`: The tenant root site.</span></span>
* <span data-ttu-id="58bf2-113">`/groups/{group-id}/sites/root`:グループのチーム サイト。</span><span class="sxs-lookup"><span data-stu-id="58bf2-113">`/groups/{group-id}/sites/root`: The group's team site.</span></span>

## <a name="permissions"></a><span data-ttu-id="58bf2-114">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="58bf2-114">Permissions</span></span>

<span data-ttu-id="58bf2-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="58bf2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="58bf2-117">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="58bf2-117">Permission type</span></span>      | <span data-ttu-id="58bf2-118">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="58bf2-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="58bf2-119">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="58bf2-119">Delegated (work or school account)</span></span> | <span data-ttu-id="58bf2-120">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58bf2-120">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="58bf2-121">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="58bf2-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="58bf2-122">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="58bf2-122">Not supported.</span></span>    |
|<span data-ttu-id="58bf2-123">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="58bf2-123">Application</span></span> | <span data-ttu-id="58bf2-124">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58bf2-124">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="get-the-tenants-root-site"></a><span data-ttu-id="58bf2-125">テナントのルート サイトを取得する</span><span class="sxs-lookup"><span data-stu-id="58bf2-125">Get the tenant's root site</span></span>

<span data-ttu-id="58bf2-126">テナント内のルートの SharePoint サイトにアクセスするには次のようにします。</span><span class="sxs-lookup"><span data-stu-id="58bf2-126">To access the root SharePoint site within a tenant:</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /sites/root
GET /sites/contoso.sharepoint.com
```

## <a name="access-a-site-by-server-relative-url"></a><span data-ttu-id="58bf2-127">サーバーの相対 URL でサイトにアクセスする</span><span class="sxs-lookup"><span data-stu-id="58bf2-127">Access a site by server-relative URL</span></span>

<span data-ttu-id="58bf2-128">**サイト** リソースのサーバーの相対 URL がある場合、次のように要求を構築することができます。</span><span class="sxs-lookup"><span data-stu-id="58bf2-128">If you have the server-relative URL for a **site** resource, you can construct a request as follows:</span></span>

```http
GET /sites/{hostname}:/{server-relative-path}
```

## <a name="access-a-group-team-site"></a><span data-ttu-id="58bf2-129">グループのチーム サイトにアクセスする</span><span class="sxs-lookup"><span data-stu-id="58bf2-129">Access a group team site</span></span>

<span data-ttu-id="58bf2-130">グループのチーム サイトにアクセスするには次のようにします。</span><span class="sxs-lookup"><span data-stu-id="58bf2-130">To access the team site for a group:</span></span>

```http
GET /groups/{group-id}/sites/root
```

## <a name="example"></a><span data-ttu-id="58bf2-131">例</span><span class="sxs-lookup"><span data-stu-id="58bf2-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="58bf2-132">要求</span><span class="sxs-lookup"><span data-stu-id="58bf2-132">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="58bf2-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="58bf2-133">--Http</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-site", "scopes": "sites.read.all" } -->

```http
GET /sites/{site-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="58bf2-134">C#</span><span class="sxs-lookup"><span data-stu-id="58bf2-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-site-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="58bf2-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="58bf2-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-site-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="58bf2-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="58bf2-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-site-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="58bf2-137">Java</span><span class="sxs-lookup"><span data-stu-id="58bf2-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-site-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="58bf2-138">応答</span><span class="sxs-lookup"><span data-stu-id="58bf2-138">Response</span></span>

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
  "tocPath": "Sites/Get by ID",
  "suppressions": [
  ]
} -->
