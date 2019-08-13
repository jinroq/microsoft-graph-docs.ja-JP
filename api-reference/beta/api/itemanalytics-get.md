---
author: daspek
description: このリソースの下で行われたビューに関する itemAnalytics を取得します。
ms.date: 10/06/2017
title: 分析を取得する
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 822664263be00f7a8a2d98a1b0815f693368cf3a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36343014"
---
# <a name="get-analytics"></a><span data-ttu-id="9fa85-103">分析を取得する</span><span class="sxs-lookup"><span data-stu-id="9fa85-103">Get analytics</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9fa85-104">このリソースの下で行われたビューに関する[Itemanalytics][]を取得します。</span><span class="sxs-lookup"><span data-stu-id="9fa85-104">Get [itemAnalytics][] about the views that took place under this resource.</span></span>
<span data-ttu-id="9fa85-105">**Itemanalytics**リソースは、およびのアクティビティの`allTime`統計を取得する便利な`lastSevenDays`方法です。</span><span class="sxs-lookup"><span data-stu-id="9fa85-105">The **itemAnalytics** resource is a convenient way to get activity stats for `allTime` and the `lastSevenDays`.</span></span>
<span data-ttu-id="9fa85-106">ユーザー設定の時間範囲または間隔の場合は、 [getActivitiesByInterval][] API を使用します。</span><span class="sxs-lookup"><span data-stu-id="9fa85-106">For a custom time range or interval, use the [getActivitiesByInterval][] API.</span></span>

><span data-ttu-id="9fa85-107">**注:\*\*\*\*Itemanalytics**リソースは、すべての[国内展開](/graph/deployments)でまだ使用できません。</span><span class="sxs-lookup"><span data-stu-id="9fa85-107">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

[itemAnalytics]: ../resources/itemanalytics.md
[getActivitiesByInterval]: ../api/itemactivity-getbyinterval.md

## <a name="permissions"></a><span data-ttu-id="9fa85-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9fa85-110">Permissions</span></span>

<span data-ttu-id="9fa85-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9fa85-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9fa85-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9fa85-113">Permission type</span></span>                        | <span data-ttu-id="9fa85-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9fa85-114">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="9fa85-115">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9fa85-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="9fa85-116">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9fa85-116">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="9fa85-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9fa85-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9fa85-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9fa85-118">Not supported.</span></span>
|<span data-ttu-id="9fa85-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9fa85-119">Application</span></span>                            | <span data-ttu-id="9fa85-120">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9fa85-120">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="9fa85-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9fa85-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/analytics
GET /sites/{site-id}/analytics
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/analytics
```

## <a name="example"></a><span data-ttu-id="9fa85-122">例</span><span class="sxs-lookup"><span data-stu-id="9fa85-122">Example</span></span>

#### <a name="request"></a><span data-ttu-id="9fa85-123">要求</span><span class="sxs-lookup"><span data-stu-id="9fa85-123">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="9fa85-124">プロトコル</span><span class="sxs-lookup"><span data-stu-id="9fa85-124">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-analytics" } -->

```http
GET /drives/{drive-id}/items/{item-id}/analytics
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9fa85-125">C#</span><span class="sxs-lookup"><span data-stu-id="9fa85-125">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-analytics-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9fa85-126">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9fa85-126">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-analytics-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9fa85-127">目的-C</span><span class="sxs-lookup"><span data-stu-id="9fa85-127">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-analytics-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="9fa85-128">Java</span><span class="sxs-lookup"><span data-stu-id="9fa85-128">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-analytics-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9fa85-129">応答</span><span class="sxs-lookup"><span data-stu-id="9fa85-129">Response</span></span>

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
