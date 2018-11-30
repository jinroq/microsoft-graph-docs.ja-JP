---
title: サイトを列挙します。
description: 指定されたフィルター条件に一致し、オプションのクエリを実行している組織で利用できる [サイト] の一覧を表示します。
ms.openlocfilehash: 4e7d9d12f7b18df84a8b23cc3272084b310edb3a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071161"
---
# <a name="enumerate-sites"></a><span data-ttu-id="a8955-103">サイトを列挙します。</span><span class="sxs-lookup"><span data-stu-id="a8955-103">Enumerate sites</span></span>

> <span data-ttu-id="a8955-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a8955-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a8955-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a8955-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a8955-106">指定されたフィルター条件に一致し、オプションのクエリを実行する組織で使用可能な[サイト][]を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="a8955-106">List the available [sites][] in an organization that match provided filter criteria and query options.</span></span>

<span data-ttu-id="a8955-107">次のクエリ オプションのみが現在サポートされています。</span><span class="sxs-lookup"><span data-stu-id="a8955-107">Only the following query options are currently supported:</span></span>

| <span data-ttu-id="a8955-108">フィルター ステートメント</span><span class="sxs-lookup"><span data-stu-id="a8955-108">Filter statement</span></span>             | <span data-ttu-id="a8955-109">ステートメントを選択します。</span><span class="sxs-lookup"><span data-stu-id="a8955-109">Select statement</span></span>        | <span data-ttu-id="a8955-110">説明</span><span class="sxs-lookup"><span data-stu-id="a8955-110">Description</span></span>
|:-----------------------------|:------------------------|:--------------------
|`siteCollection/root ne null` | `siteCollection,webUrl` | <span data-ttu-id="a8955-111">組織内のすべてのルート レベルのサイト コレクションの一覧を表示します。</span><span class="sxs-lookup"><span data-stu-id="a8955-111">Lists all root-level site collections in the organization.</span></span> <span data-ttu-id="a8955-112">各地域のホーム サイトを発見するのに便利です。</span><span class="sxs-lookup"><span data-stu-id="a8955-112">Useful for discovering the home site for each geography.</span></span>

<span data-ttu-id="a8955-113">さらに、特定のキーワードに一致するサイトを検索するのに 'と、サイト' のコレクションに対して**[検索][]** クエリを使用することがあります。</span><span class="sxs-lookup"><span data-stu-id="a8955-113">In addition, you may use a **[search][]** query against the '/sites' collection to find sites matching given keywords.</span></span>

[検索]: site-search.md
[search]: site-search.md
[sites]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="a8955-116">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a8955-116">Permissions</span></span>

<span data-ttu-id="a8955-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a8955-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8955-119">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a8955-119">Permission type</span></span>                        | <span data-ttu-id="a8955-120">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a8955-120">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="a8955-121">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a8955-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="a8955-122">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8955-122">Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="a8955-123">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a8955-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a8955-124">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a8955-124">Not supported.</span></span>
|<span data-ttu-id="a8955-125">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a8955-125">Application</span></span>                            | <span data-ttu-id="a8955-126">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8955-126">Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="a8955-127">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a8955-127">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET https://graph.microsoft.com/beta/sites?filter=siteCollection/root ne null
```

## <a name="example"></a><span data-ttu-id="a8955-128">例</span><span class="sxs-lookup"><span data-stu-id="a8955-128">Example</span></span>

#### <a name="request"></a><span data-ttu-id="a8955-129">要求</span><span class="sxs-lookup"><span data-stu-id="a8955-129">Request</span></span>

<!-- { "blockType": "request", "name": "list-sites" } -->

```http
GET https://graph.microsoft.com/beta/sites?select=siteCollection,webUrl&filter=siteCollection/root%20ne%20null
```

#### <a name="response"></a><span data-ttu-id="a8955-130">応答</span><span class="sxs-lookup"><span data-stu-id="a8955-130">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.site", "isCollection": true, "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "contoso.sharepoint.com,da60e844-ba1d-49bc-b4d4-d5e36bae9019,712a596e-90a1-49e3-9b48-bfa80bee8740",
      "name": "Contoso USA",
      "root": { },
      "siteCollection": {
        "hostname": "contoso.sharepoint.com",
        "dataLocationCode": "NAM",
        "root": { }
      },
      "webUrl": "https://contoso.sharepoint.com"
    },
    {
      "id": "contoso-jpn.sharepoint.com,da60e844-ba1d-49bc-b4d4-d5e36bae9019,0271110f-634f-4300-a841-3a8a2e851851",
      "name": "Contoso Japan",
      "root": { },
      "siteCollection": {
        "hostname": "contoso-jp.sharepoint.com",
        "dataLocationCode": "JPN",
        "root": { }
      },
      "webUrl": "https://contoso-jp.sharepoint.com"
    }
  ]
}
```

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Site/List sites"
} -->
