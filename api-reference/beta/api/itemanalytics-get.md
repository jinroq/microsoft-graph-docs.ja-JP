---
author: daspek
ms.author: dspektor
ms.date: 10/06/2017
title: 分析を取得する
localization_priority: Normal
ms.openlocfilehash: 0bd237ea86e66b228ca571cca8a0f93a757866bf
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35449218"
---
# <a name="get-analytics"></a><span data-ttu-id="8f122-102">分析を取得する</span><span class="sxs-lookup"><span data-stu-id="8f122-102">Get analytics</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8f122-103">このリソースの下で行われたビューに関する[Itemanalytics][]を取得します。</span><span class="sxs-lookup"><span data-stu-id="8f122-103">Get [itemAnalytics][] about the views that took place under this resource.</span></span>
<span data-ttu-id="8f122-104">**Itemanalytics**リソースは、およびのアクティビティの`allTime`統計を取得する便利な`lastSevenDays`方法です。</span><span class="sxs-lookup"><span data-stu-id="8f122-104">The **itemAnalytics** resource is a convenient way to get activity stats for `allTime` and the `lastSevenDays`.</span></span>
<span data-ttu-id="8f122-105">ユーザー設定の時間範囲または間隔の場合は、 [getActivitiesByInterval][] API を使用します。</span><span class="sxs-lookup"><span data-stu-id="8f122-105">For a custom time range or interval, use the [getActivitiesByInterval][] API.</span></span>

><span data-ttu-id="8f122-106">**注:\*\*\*\*Itemanalytics**リソースは、すべての[国内展開](/graph/deployments)でまだ使用できません。</span><span class="sxs-lookup"><span data-stu-id="8f122-106">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

[itemAnalytics]: ../resources/itemanalytics.md
[getActivitiesByInterval]: ../api/itemactivity-getbyinterval.md

## <a name="permissions"></a><span data-ttu-id="8f122-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8f122-109">Permissions</span></span>

<span data-ttu-id="8f122-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8f122-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8f122-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8f122-112">Permission type</span></span>                        | <span data-ttu-id="8f122-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8f122-113">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="8f122-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8f122-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="8f122-115">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f122-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="8f122-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8f122-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8f122-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8f122-117">Not supported.</span></span>
|<span data-ttu-id="8f122-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8f122-118">Application</span></span>                            | <span data-ttu-id="8f122-119">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f122-119">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="8f122-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8f122-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/analytics
GET /sites/{site-id}/analytics
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/analytics
```

## <a name="example"></a><span data-ttu-id="8f122-121">例</span><span class="sxs-lookup"><span data-stu-id="8f122-121">Example</span></span>

#### <a name="request"></a><span data-ttu-id="8f122-122">要求</span><span class="sxs-lookup"><span data-stu-id="8f122-122">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="8f122-123">プロトコル</span><span class="sxs-lookup"><span data-stu-id="8f122-123">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-analytics" } -->

```http
GET /drives/{drive-id}/items/{item-id}/analytics
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8f122-124">C#</span><span class="sxs-lookup"><span data-stu-id="8f122-124">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-analytics-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8f122-125">Javascript</span><span class="sxs-lookup"><span data-stu-id="8f122-125">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-analytics-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8f122-126">目的-C</span><span class="sxs-lookup"><span data-stu-id="8f122-126">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-analytics-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8f122-127">応答</span><span class="sxs-lookup"><span data-stu-id="8f122-127">Response</span></span>

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

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "BaseItem/Get analytics",
  "suppressions": [
  ]
}
-->
