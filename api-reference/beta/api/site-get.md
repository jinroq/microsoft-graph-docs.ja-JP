---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SharePoint サイトを取得する
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 25d52ee0ee2007819ac422638bab95b3b4c83ec8
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35869678"
---
# <a name="get-a-site-resource"></a><span data-ttu-id="0bcd8-102">サイト リソースを取得する</span><span class="sxs-lookup"><span data-stu-id="0bcd8-102">Get a site resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0bcd8-p101">[サイト][] リソースのプロパティとリレーションシップを取得します。**サイト** リソースは、SharePoint のチーム サイトを表します。</span><span class="sxs-lookup"><span data-stu-id="0bcd8-p101">Retrieve properties and relationships for a [site][] resource. A **site** resource represents a team site in SharePoint.</span></span>

[サイト]: ../resources/site.md
[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="0bcd8-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0bcd8-106">Permissions</span></span>

<span data-ttu-id="0bcd8-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0bcd8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0bcd8-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0bcd8-109">Permission type</span></span>      | <span data-ttu-id="0bcd8-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0bcd8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0bcd8-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0bcd8-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0bcd8-112">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0bcd8-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="0bcd8-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0bcd8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0bcd8-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0bcd8-114">Not supported.</span></span>    |
|<span data-ttu-id="0bcd8-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0bcd8-115">Application</span></span> | <span data-ttu-id="0bcd8-116">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0bcd8-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="get-the-tenants-root-site"></a><span data-ttu-id="0bcd8-117">テナントのルート サイトを取得する</span><span class="sxs-lookup"><span data-stu-id="0bcd8-117">Get the tenant's root site</span></span>

<span data-ttu-id="0bcd8-118">テナント内のルートの SharePoint サイトにアクセスするには次のようにします。</span><span class="sxs-lookup"><span data-stu-id="0bcd8-118">To access the root SharePoint site within a tenant:</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /sites/root
GET /sites/contoso.sharepoint.com
```

## <a name="access-a-site-by-server-relative-url"></a><span data-ttu-id="0bcd8-119">サーバーの相対 URL でサイトにアクセスする</span><span class="sxs-lookup"><span data-stu-id="0bcd8-119">Access a site by server-relative URL</span></span>

<span data-ttu-id="0bcd8-120">**サイト** リソースのサーバーの相対 URL がある場合、次のように要求を構築することができます。</span><span class="sxs-lookup"><span data-stu-id="0bcd8-120">If you have the server-relative URL for a **site** resource, you can construct a request as follows:</span></span>

```http
GET /sites/{hostname}:/{server-relative-path}
```

## <a name="access-a-group-team-site"></a><span data-ttu-id="0bcd8-121">グループのチーム サイトにアクセスする</span><span class="sxs-lookup"><span data-stu-id="0bcd8-121">Access a group team site</span></span>

<span data-ttu-id="0bcd8-122">グループのチーム サイトにアクセスするには次のようにします。</span><span class="sxs-lookup"><span data-stu-id="0bcd8-122">To access the team site for a group:</span></span>

```http
GET /groups/{group-id}/sites/root
```

## <a name="example"></a><span data-ttu-id="0bcd8-123">例</span><span class="sxs-lookup"><span data-stu-id="0bcd8-123">Example</span></span>

### <a name="request"></a><span data-ttu-id="0bcd8-124">要求</span><span class="sxs-lookup"><span data-stu-id="0bcd8-124">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="0bcd8-125">プロトコル</span><span class="sxs-lookup"><span data-stu-id="0bcd8-125">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-site" } -->

```http
GET /sites/{site-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0bcd8-126">C#</span><span class="sxs-lookup"><span data-stu-id="0bcd8-126">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-site-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0bcd8-127">Javascript</span><span class="sxs-lookup"><span data-stu-id="0bcd8-127">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-site-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0bcd8-128">目的-C</span><span class="sxs-lookup"><span data-stu-id="0bcd8-128">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-site-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="0bcd8-129">Java</span><span class="sxs-lookup"><span data-stu-id="0bcd8-129">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-site-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0bcd8-130">応答</span><span class="sxs-lookup"><span data-stu-id="0bcd8-130">Response</span></span>

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

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites/Get by ID",
  "suppressions": [
  ]
}
-->
