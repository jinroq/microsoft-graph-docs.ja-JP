---
author: daspek
ms.author: dspektor
ms.date: 10/06/2017
title: 間隔によって項目のアクティビティの統計 (stats) を取得します。
ms.openlocfilehash: 0b5a9782528e75d4d50734dedc49460d30252410
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069414"
---
# <a name="get-item-activity-stats-by-interval"></a><span data-ttu-id="61e47-102">間隔によって項目のアクティビティの統計 (stats) を取得します。</span><span class="sxs-lookup"><span data-stu-id="61e47-102">Get item activity stats by interval</span></span>

> <span data-ttu-id="61e47-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="61e47-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="61e47-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="61e47-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="61e47-105">このリソース内の指定した時間間隔で行われた活動の[itemActivityStats][]を取得します。</span><span class="sxs-lookup"><span data-stu-id="61e47-105">Get [itemActivityStats][] for the activities that took place under this resource within the specified time interval.</span></span>

><span data-ttu-id="61e47-106">**注:\*\*\*\*ItemAnalytics**リソースはまだすべての[国内展開](/graph/deployments)で使用可能ではありません。</span><span class="sxs-lookup"><span data-stu-id="61e47-106">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

<span data-ttu-id="61e47-107">分析の集計は、すべてのアクション タイプにできない可能性があります。</span><span class="sxs-lookup"><span data-stu-id="61e47-107">Analytics aggregates might not be available for all action types.</span></span>

[itemActivityStats]: ../resources/itemactivitystat.md

## <a name="permissions"></a><span data-ttu-id="61e47-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="61e47-109">Permissions</span></span>

<span data-ttu-id="61e47-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="61e47-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="61e47-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="61e47-112">Permission type</span></span>                        | <span data-ttu-id="61e47-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="61e47-113">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="61e47-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="61e47-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="61e47-115">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61e47-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="61e47-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="61e47-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="61e47-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="61e47-117">Not supported.</span></span>
|<span data-ttu-id="61e47-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="61e47-118">Application</span></span>                            | <span data-ttu-id="61e47-119">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61e47-119">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="61e47-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="61e47-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-01-01',endDateTime='2017-01-10',interval='day')
GET /sites/{site-id}/getActivitiesByInterval(startDateTime='2016',endDateTime='2017',interval='month')
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-05-01',interval='week')
```

## <a name="function-parameters"></a><span data-ttu-id="61e47-121">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="61e47-121">Function parameters</span></span>

| <span data-ttu-id="61e47-122">名前</span><span class="sxs-lookup"><span data-stu-id="61e47-122">Name</span></span>           | <span data-ttu-id="61e47-123">値</span><span class="sxs-lookup"><span data-stu-id="61e47-123">Value</span></span>              | <span data-ttu-id="61e47-124">説明</span><span class="sxs-lookup"><span data-stu-id="61e47-124">Description</span></span>
|:---------------|:-------------------|:---------------------------------------
| <span data-ttu-id="61e47-125">startDateTime</span><span class="sxs-lookup"><span data-stu-id="61e47-125">startDateTime</span></span>  | <span data-ttu-id="61e47-126">文字列 (タイムスタンプ)</span><span class="sxs-lookup"><span data-stu-id="61e47-126">string (timestamp)</span></span> | <span data-ttu-id="61e47-127">集計の活動に使用される開始時刻。</span><span class="sxs-lookup"><span data-stu-id="61e47-127">The start time over which to aggregate activities.</span></span>
| <span data-ttu-id="61e47-128">endDateTime</span><span class="sxs-lookup"><span data-stu-id="61e47-128">endDateTime</span></span>    | <span data-ttu-id="61e47-129">文字列 (タイムスタンプ)</span><span class="sxs-lookup"><span data-stu-id="61e47-129">string (timestamp)</span></span> | <span data-ttu-id="61e47-130">集計の活動に使用される終了時間です。</span><span class="sxs-lookup"><span data-stu-id="61e47-130">The end time over which to aggregate activities.</span></span>
| <span data-ttu-id="61e47-131">interval</span><span class="sxs-lookup"><span data-stu-id="61e47-131">interval</span></span>       | <span data-ttu-id="61e47-132">文字列</span><span class="sxs-lookup"><span data-stu-id="61e47-132">string</span></span>             | <span data-ttu-id="61e47-133">集計間隔です。</span><span class="sxs-lookup"><span data-stu-id="61e47-133">The aggregation interval.</span></span>

## <a name="example"></a><span data-ttu-id="61e47-134">例</span><span class="sxs-lookup"><span data-stu-id="61e47-134">Example</span></span>

#### <a name="request"></a><span data-ttu-id="61e47-135">要求</span><span class="sxs-lookup"><span data-stu-id="61e47-135">Request</span></span>

<!-- { "blockType": "request", "name": "get-activities-by-interval" } -->

```http
GET /drives/{drive-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-01-01',endDateTime='2017-01-3',interval='day')
```

#### <a name="response"></a><span data-ttu-id="61e47-136">応答</span><span class="sxs-lookup"><span data-stu-id="61e47-136">Response</span></span>

<!-- { "blockType": "response", "@type": "Collection(microsoft.graph.itemActivityStat)", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "startDateTime": "2017-01-01T00:00:00.000Z",
            "endDateTime": "2017-01-02T00:00:00.000Z",
            "delete": {
                "actionCount": 1,
                "actorCount": 1
            },
            "access": {
                "actionCount": 5,
                "actorCount": 3
            }
        },
        {
            "startDateTime": "2017-01-02T00:00:00.000Z",
            "endDateTime": "2017-01-03T00:00:00.000Z",
            "edit": {
                "actionCount": 3,
                "actorCount": 1
            },
            "access": {
                "actionCount": 7,
                "actorCount": 6
            }
        }
    ]
}
```

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "BaseItem/Get activities by interval"
} -->