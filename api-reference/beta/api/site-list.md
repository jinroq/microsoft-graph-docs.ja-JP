---
title: サイトを列挙します。
description: 指定されたフィルター条件に一致し、オプションのクエリを実行している組織で利用できる [サイト] の一覧を表示します。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: f225d9990637f8251ae40e3f66b0f993bbf74f32
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520341"
---
# <a name="enumerate-sites"></a><span data-ttu-id="b381a-103">サイトを列挙します。</span><span class="sxs-lookup"><span data-stu-id="b381a-103">Enumerate sites</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b381a-104">指定されたフィルター条件に一致し、オプションのクエリを実行する組織で使用可能な[サイト][]を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="b381a-104">List the available [sites][] in an organization that match provided filter criteria and query options.</span></span>

<span data-ttu-id="b381a-105">次のクエリ オプションのみが現在サポートされています。</span><span class="sxs-lookup"><span data-stu-id="b381a-105">Only the following query options are currently supported:</span></span>

| <span data-ttu-id="b381a-106">フィルター ステートメント</span><span class="sxs-lookup"><span data-stu-id="b381a-106">Filter statement</span></span>             | <span data-ttu-id="b381a-107">SELECT ステートメント</span><span class="sxs-lookup"><span data-stu-id="b381a-107">Select statement</span></span>        | <span data-ttu-id="b381a-108">説明</span><span class="sxs-lookup"><span data-stu-id="b381a-108">Description</span></span>
|:-----------------------------|:------------------------|:--------------------
|`siteCollection/root ne null` | `siteCollection,webUrl` | <span data-ttu-id="b381a-109">組織内のすべてのルート レベルのサイト コレクションの一覧を表示します。</span><span class="sxs-lookup"><span data-stu-id="b381a-109">Lists all root-level site collections in the organization.</span></span> <span data-ttu-id="b381a-110">各地域のホーム サイトを発見するのに便利です。</span><span class="sxs-lookup"><span data-stu-id="b381a-110">Useful for discovering the home site for each geography.</span></span>

<span data-ttu-id="b381a-111">さらに、特定のキーワードに一致するサイトを検索するのに 'と、サイト' のコレクションに対して**[検索][]** クエリを使用することがあります。</span><span class="sxs-lookup"><span data-stu-id="b381a-111">In addition, you may use a **[search][]** query against the '/sites' collection to find sites matching given keywords.</span></span>

[Search]: site-search.md
[search]: site-search.md
[sites]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="b381a-114">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b381a-114">Permissions</span></span>

<span data-ttu-id="b381a-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b381a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b381a-117">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b381a-117">Permission type</span></span>                        | <span data-ttu-id="b381a-118">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b381a-118">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="b381a-119">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b381a-119">Delegated (work or school account)</span></span>     | <span data-ttu-id="b381a-120">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b381a-120">Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="b381a-121">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b381a-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b381a-122">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b381a-122">Not supported.</span></span>
|<span data-ttu-id="b381a-123">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b381a-123">Application</span></span>                            | <span data-ttu-id="b381a-124">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b381a-124">Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="b381a-125">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b381a-125">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET https://graph.microsoft.com/beta/sites?filter=siteCollection/root ne null
```

## <a name="example"></a><span data-ttu-id="b381a-126">例</span><span class="sxs-lookup"><span data-stu-id="b381a-126">Example</span></span>

#### <a name="request"></a><span data-ttu-id="b381a-127">要求</span><span class="sxs-lookup"><span data-stu-id="b381a-127">Request</span></span>

<!-- { "blockType": "request", "name": "list-sites" } -->

```http
GET https://graph.microsoft.com/beta/sites?select=siteCollection,webUrl&filter=siteCollection/root%20ne%20null
```

#### <a name="response"></a><span data-ttu-id="b381a-128">応答</span><span class="sxs-lookup"><span data-stu-id="b381a-128">Response</span></span>

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

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Site/List sites",
  "suppressions": [
    "Error: /api-reference/beta/api/site-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
