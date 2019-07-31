---
author: daspek
description: このリソースの下で行われたビューに関する itemAnalytics を取得します。
ms.date: 10/06/2017
title: 分析を取得する
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 47ee4b3d003c81b077e67cf8dca8e8cec047d37d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35993180"
---
# <a name="get-analytics"></a><span data-ttu-id="a3933-103">分析を取得する</span><span class="sxs-lookup"><span data-stu-id="a3933-103">Get analytics</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a3933-104">このリソースの下で行われたビューに関する[Itemanalytics][]を取得します。</span><span class="sxs-lookup"><span data-stu-id="a3933-104">Get [itemAnalytics][] about the views that took place under this resource.</span></span>
<span data-ttu-id="a3933-105">**Itemanalytics**リソースは、およびのアクティビティの`allTime`統計を取得する便利な`lastSevenDays`方法です。</span><span class="sxs-lookup"><span data-stu-id="a3933-105">The **itemAnalytics** resource is a convenient way to get activity stats for `allTime` and the `lastSevenDays`.</span></span>
<span data-ttu-id="a3933-106">ユーザー設定の時間範囲または間隔の場合は、 [getActivitiesByInterval][] API を使用します。</span><span class="sxs-lookup"><span data-stu-id="a3933-106">For a custom time range or interval, use the [getActivitiesByInterval][] API.</span></span>

><span data-ttu-id="a3933-107">**注:\*\*\*\*Itemanalytics**リソースは、すべての[国内展開](/graph/deployments)でまだ使用できません。</span><span class="sxs-lookup"><span data-stu-id="a3933-107">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

[itemAnalytics]: ../resources/itemanalytics.md
[getActivitiesByInterval]: ../api/itemactivity-getbyinterval.md

## <a name="permissions"></a><span data-ttu-id="a3933-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a3933-110">Permissions</span></span>

<span data-ttu-id="a3933-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a3933-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3933-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a3933-113">Permission type</span></span>                        | <span data-ttu-id="a3933-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a3933-114">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="a3933-115">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a3933-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="a3933-116">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3933-116">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="a3933-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a3933-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a3933-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a3933-118">Not supported.</span></span>
|<span data-ttu-id="a3933-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a3933-119">Application</span></span>                            | <span data-ttu-id="a3933-120">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3933-120">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="a3933-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a3933-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/analytics
GET /sites/{site-id}/analytics
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/analytics
```

## <a name="example"></a><span data-ttu-id="a3933-122">例</span><span class="sxs-lookup"><span data-stu-id="a3933-122">Example</span></span>

#### <a name="request"></a><span data-ttu-id="a3933-123">要求</span><span class="sxs-lookup"><span data-stu-id="a3933-123">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="a3933-124">プロトコル</span><span class="sxs-lookup"><span data-stu-id="a3933-124">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-analytics" } -->

```http
GET /drives/{drive-id}/items/{item-id}/analytics
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a3933-125">C#</span><span class="sxs-lookup"><span data-stu-id="a3933-125">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-analytics-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a3933-126">Javascript</span><span class="sxs-lookup"><span data-stu-id="a3933-126">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-analytics-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a3933-127">目的-C</span><span class="sxs-lookup"><span data-stu-id="a3933-127">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-analytics-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="a3933-128">Java</span><span class="sxs-lookup"><span data-stu-id="a3933-128">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-analytics-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a3933-129">応答</span><span class="sxs-lookup"><span data-stu-id="a3933-129">Response</span></span>

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
