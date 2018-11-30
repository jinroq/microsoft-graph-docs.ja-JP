---
author: daspek
ms.author: dspektor
ms.date: 10/06/2017
title: 分析を取得します。
ms.openlocfilehash: 57f009e0d2a07a5bf8c9a0f3b3617083bc279545
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070733"
---
# <a name="get-analytics"></a><span data-ttu-id="cdbb8-102">分析を取得します。</span><span class="sxs-lookup"><span data-stu-id="cdbb8-102">Get analytics</span></span>

> <span data-ttu-id="cdbb8-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="cdbb8-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cdbb8-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cdbb8-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cdbb8-105">このリソースに行われたビューの[itemAnalytics][]を取得します。</span><span class="sxs-lookup"><span data-stu-id="cdbb8-105">Get [itemAnalytics][] about the views that took place under this resource.</span></span>
<span data-ttu-id="cdbb8-106">**ItemAnalytics**リソースの利用状況の統計 (stats) を取得する便利な方法では`allTime`と`lastSevenDays`。</span><span class="sxs-lookup"><span data-stu-id="cdbb8-106">The **itemAnalytics** resource is a convenient way to get activity stats for `allTime` and the `lastSevenDays`.</span></span>
<span data-ttu-id="cdbb8-107">ユーザー設定の時刻の範囲または間隔では、 [getActivitiesByInterval][] API を使用します。</span><span class="sxs-lookup"><span data-stu-id="cdbb8-107">For a custom time range or interval, use the [getActivitiesByInterval][] API.</span></span>

><span data-ttu-id="cdbb8-108">**注:\*\*\*\*ItemAnalytics**リソースはまだすべての[国内展開](/graph/deployments)で使用可能ではありません。</span><span class="sxs-lookup"><span data-stu-id="cdbb8-108">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

[itemAnalytics]: ../resources/itemanalytics.md
[getActivitiesByInterval]: ../api/itemactivity-getbyinterval.md

## <a name="permissions"></a><span data-ttu-id="cdbb8-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="cdbb8-111">Permissions</span></span>

<span data-ttu-id="cdbb8-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cdbb8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cdbb8-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cdbb8-114">Permission type</span></span>                        | <span data-ttu-id="cdbb8-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="cdbb8-115">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="cdbb8-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cdbb8-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="cdbb8-117">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cdbb8-117">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="cdbb8-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cdbb8-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cdbb8-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cdbb8-119">Not supported.</span></span>
|<span data-ttu-id="cdbb8-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cdbb8-120">Application</span></span>                            | <span data-ttu-id="cdbb8-121">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cdbb8-121">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="cdbb8-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cdbb8-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/analytics
GET /sites/{site-id}/analytics
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/analytics
```

## <a name="example"></a><span data-ttu-id="cdbb8-123">例</span><span class="sxs-lookup"><span data-stu-id="cdbb8-123">Example</span></span>

#### <a name="request"></a><span data-ttu-id="cdbb8-124">要求</span><span class="sxs-lookup"><span data-stu-id="cdbb8-124">Request</span></span>

<!-- { "blockType": "request", "name": "get-analytics" } -->

```http
GET /drives/{drive-id}/items/{item-id}/analytics
```

#### <a name="response"></a><span data-ttu-id="cdbb8-125">応答</span><span class="sxs-lookup"><span data-stu-id="cdbb8-125">Response</span></span>

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

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "BaseItem/Get analytics"
} -->
