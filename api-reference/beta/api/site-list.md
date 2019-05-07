---
title: サイトの列挙
description: 指定したフィルター条件とクエリオプションに一致する組織内で利用可能な [sites] [] を一覧表示します。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: f61aab6a7a333e83438f5cc6d03c6ac79e277df2
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33638642"
---
# <a name="enumerate-sites"></a><span data-ttu-id="f3da2-103">サイトの列挙</span><span class="sxs-lookup"><span data-stu-id="f3da2-103">Enumerate sites</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f3da2-104">指定したフィルター条件とクエリオプションに一致する組織内の使用可能な[サイト][]を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="f3da2-104">List the available [sites][] in an organization that match provided filter criteria and query options.</span></span>

<span data-ttu-id="f3da2-105">次のクエリオプションのみが現在サポートされています。</span><span class="sxs-lookup"><span data-stu-id="f3da2-105">Only the following query options are currently supported:</span></span>

| <span data-ttu-id="f3da2-106">Filter ステートメント</span><span class="sxs-lookup"><span data-stu-id="f3da2-106">Filter statement</span></span>             | <span data-ttu-id="f3da2-107">Select ステートメント</span><span class="sxs-lookup"><span data-stu-id="f3da2-107">Select statement</span></span>        | <span data-ttu-id="f3da2-108">説明</span><span class="sxs-lookup"><span data-stu-id="f3da2-108">Description</span></span>
|:-----------------------------|:------------------------|:--------------------
|`siteCollection/root ne null` | `siteCollection,webUrl` | <span data-ttu-id="f3da2-109">組織内のすべてのルートレベルのサイトコレクションを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="f3da2-109">Lists all root-level site collections in the organization.</span></span> <span data-ttu-id="f3da2-110">各地域のホームサイトを検出するのに役立ちます。</span><span class="sxs-lookup"><span data-stu-id="f3da2-110">Useful for discovering the home site for each geography.</span></span>

<span data-ttu-id="f3da2-111">また、'/サイト ' コレクションに対して**[検索][]** クエリを使用して、特定のキーワードに一致するサイトを検索することもできます。</span><span class="sxs-lookup"><span data-stu-id="f3da2-111">In addition, you may use a **[search][]** query against the '/sites' collection to find sites matching given keywords.</span></span>

[探す]: site-search.md
[search]: site-search.md
[サイト]: ../resources/site.md
[sites]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="f3da2-114">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f3da2-114">Permissions</span></span>

<span data-ttu-id="f3da2-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f3da2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3da2-117">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f3da2-117">Permission type</span></span>                        | <span data-ttu-id="f3da2-118">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f3da2-118">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="f3da2-119">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f3da2-119">Delegated (work or school account)</span></span>     | <span data-ttu-id="f3da2-120">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3da2-120">Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="f3da2-121">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f3da2-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f3da2-122">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f3da2-122">Not supported.</span></span>
|<span data-ttu-id="f3da2-123">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f3da2-123">Application</span></span>                            | <span data-ttu-id="f3da2-124">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3da2-124">Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="f3da2-125">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f3da2-125">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET https://graph.microsoft.com/beta/sites?filter=siteCollection/root ne null
```

## <a name="example"></a><span data-ttu-id="f3da2-126">例</span><span class="sxs-lookup"><span data-stu-id="f3da2-126">Example</span></span>

#### <a name="request"></a><span data-ttu-id="f3da2-127">要求</span><span class="sxs-lookup"><span data-stu-id="f3da2-127">Request</span></span>

<!-- { "blockType": "request", "name": "list-sites" } -->

```http
GET https://graph.microsoft.com/beta/sites?select=siteCollection,webUrl&filter=siteCollection/root%20ne%20null
```

#### <a name="response"></a><span data-ttu-id="f3da2-128">応答</span><span class="sxs-lookup"><span data-stu-id="f3da2-128">Response</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="f3da2-129">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="f3da2-129">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f3da2-130">Visual</span><span class="sxs-lookup"><span data-stu-id="f3da2-130">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/list-sites-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f3da2-131">Java</span><span class="sxs-lookup"><span data-stu-id="f3da2-131">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/list-sites-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Site/List sites",
  "suppressions": [
    "Error: /api-reference/beta/api/site-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/site-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
