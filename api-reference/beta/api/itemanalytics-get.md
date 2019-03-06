---
author: daspek
ms.author: dspektor
ms.date: 10/06/2017
title: 分析を取得します。
localization_priority: Normal
ms.openlocfilehash: d1f6b255747cffe7fdccb5d098e73a56151b6245
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516260"
---
# <a name="get-analytics"></a><span data-ttu-id="d954a-102">分析を取得します。</span><span class="sxs-lookup"><span data-stu-id="d954a-102">Get analytics</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d954a-103">このリソースに行われたビューの[itemAnalytics][]を取得します。</span><span class="sxs-lookup"><span data-stu-id="d954a-103">Get [itemAnalytics][] about the views that took place under this resource.</span></span>
<span data-ttu-id="d954a-104">**ItemAnalytics**リソースの利用状況の統計 (stats) を取得する便利な方法では`allTime`と`lastSevenDays`。</span><span class="sxs-lookup"><span data-stu-id="d954a-104">The **itemAnalytics** resource is a convenient way to get activity stats for `allTime` and the `lastSevenDays`.</span></span>
<span data-ttu-id="d954a-105">ユーザー設定の時刻の範囲または間隔では、 [getActivitiesByInterval][] API を使用します。</span><span class="sxs-lookup"><span data-stu-id="d954a-105">For a custom time range or interval, use the [getActivitiesByInterval][] API.</span></span>

><span data-ttu-id="d954a-106">**注:** **ItemAnalytics**リソースはまだすべての[国内展開](/graph/deployments)で使用可能ではありません。</span><span class="sxs-lookup"><span data-stu-id="d954a-106">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

[itemAnalytics]: ../resources/itemanalytics.md
[getActivitiesByInterval]: ../api/itemactivity-getbyinterval.md

## <a name="permissions"></a><span data-ttu-id="d954a-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d954a-109">Permissions</span></span>

<span data-ttu-id="d954a-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d954a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d954a-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d954a-112">Permission type</span></span>                        | <span data-ttu-id="d954a-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d954a-113">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="d954a-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d954a-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="d954a-115">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d954a-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="d954a-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d954a-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d954a-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d954a-117">Not supported.</span></span>
|<span data-ttu-id="d954a-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d954a-118">Application</span></span>                            | <span data-ttu-id="d954a-119">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d954a-119">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="d954a-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d954a-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/analytics
GET /sites/{site-id}/analytics
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/analytics
```

## <a name="example"></a><span data-ttu-id="d954a-121">例</span><span class="sxs-lookup"><span data-stu-id="d954a-121">Example</span></span>

#### <a name="request"></a><span data-ttu-id="d954a-122">要求</span><span class="sxs-lookup"><span data-stu-id="d954a-122">Request</span></span>

<!-- { "blockType": "request", "name": "get-analytics" } -->

```http
GET /drives/{drive-id}/items/{item-id}/analytics
```

#### <a name="response"></a><span data-ttu-id="d954a-123">応答</span><span class="sxs-lookup"><span data-stu-id="d954a-123">Response</span></span>

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
    "Error: /api-reference/beta/api/itemanalytics-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
