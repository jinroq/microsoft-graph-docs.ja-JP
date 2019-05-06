---
author: daspek
ms.author: dspektor
ms.date: 10/06/2017
title: 分析を取得する
localization_priority: Normal
ms.openlocfilehash: b0112041d6b8a8fead91ff76501d9e9b5f1c3102
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33598362"
---
# <a name="get-analytics"></a><span data-ttu-id="c185e-102">分析を取得する</span><span class="sxs-lookup"><span data-stu-id="c185e-102">Get analytics</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c185e-103">このリソースの下で行われたビューに関する[Itemanalytics][]を取得します。</span><span class="sxs-lookup"><span data-stu-id="c185e-103">Get [itemAnalytics][] about the views that took place under this resource.</span></span>
<span data-ttu-id="c185e-104">**Itemanalytics**リソースは、およびのアクティビティの`allTime`統計を取得する便利な`lastSevenDays`方法です。</span><span class="sxs-lookup"><span data-stu-id="c185e-104">The **itemAnalytics** resource is a convenient way to get activity stats for `allTime` and the `lastSevenDays`.</span></span>
<span data-ttu-id="c185e-105">ユーザー設定の時間範囲または間隔の場合は、 [getActivitiesByInterval][] API を使用します。</span><span class="sxs-lookup"><span data-stu-id="c185e-105">For a custom time range or interval, use the [getActivitiesByInterval][] API.</span></span>

><span data-ttu-id="c185e-106">**注:\*\*\*\*Itemanalytics**リソースは、すべての[国内展開](/graph/deployments)でまだ使用できません。</span><span class="sxs-lookup"><span data-stu-id="c185e-106">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

[itemAnalytics]: ../resources/itemanalytics.md
[getActivitiesByInterval]: ../api/itemactivity-getbyinterval.md

## <a name="permissions"></a><span data-ttu-id="c185e-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c185e-109">Permissions</span></span>

<span data-ttu-id="c185e-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c185e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c185e-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c185e-112">Permission type</span></span>                        | <span data-ttu-id="c185e-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c185e-113">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="c185e-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c185e-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="c185e-115">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c185e-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="c185e-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c185e-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c185e-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c185e-117">Not supported.</span></span>
|<span data-ttu-id="c185e-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c185e-118">Application</span></span>                            | <span data-ttu-id="c185e-119">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c185e-119">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="c185e-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c185e-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/analytics
GET /sites/{site-id}/analytics
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/analytics
```

## <a name="example"></a><span data-ttu-id="c185e-121">例</span><span class="sxs-lookup"><span data-stu-id="c185e-121">Example</span></span>

#### <a name="request"></a><span data-ttu-id="c185e-122">要求</span><span class="sxs-lookup"><span data-stu-id="c185e-122">Request</span></span>

<!-- { "blockType": "request", "name": "get-analytics" } -->

```http
GET /drives/{drive-id}/items/{item-id}/analytics
```

#### <a name="response"></a><span data-ttu-id="c185e-123">応答</span><span class="sxs-lookup"><span data-stu-id="c185e-123">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.itemAnalytics", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
    "allTime": {
        "access": {
            "actionCount": 123,
            "actorCount": 89
        }
    },
    "lastSevenDays": {
        "access": {
            "actionCount": 52,
            "actorCount": 41
        }
    }
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="c185e-124">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="c185e-124">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c185e-125">Visual</span><span class="sxs-lookup"><span data-stu-id="c185e-125">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-analytics-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c185e-126">Java</span><span class="sxs-lookup"><span data-stu-id="c185e-126">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-analytics-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "BaseItem/Get analytics",
  "suppressions": [
    "Error: /api-reference/beta/api/itemanalytics-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/itemanalytics-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
