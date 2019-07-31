---
author: daspek
description: このリソースの下で、指定された期間内に行われたアクティビティの itemActivityStats を取得します。
ms.date: 10/06/2017
title: 間隔ごとにアイテムアクティビティの統計情報を取得する
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 6d1f7a3b4e6a326f107a0d0ff33db59ed73f2794
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35979107"
---
# <a name="get-item-activity-stats-by-interval"></a><span data-ttu-id="4e241-103">間隔ごとにアイテムアクティビティの統計情報を取得する</span><span class="sxs-lookup"><span data-stu-id="4e241-103">Get item activity stats by interval</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4e241-104">このリソースの下で、指定された期間内に行われたアクティビティの[Itemactivitystats][]を取得します。</span><span class="sxs-lookup"><span data-stu-id="4e241-104">Get [itemActivityStats][] for the activities that took place under this resource within the specified time interval.</span></span>

><span data-ttu-id="4e241-105">**注:\*\*\*\*Itemanalytics**リソースは、すべての[国内展開](/graph/deployments)でまだ使用できません。</span><span class="sxs-lookup"><span data-stu-id="4e241-105">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

<span data-ttu-id="4e241-106">分析集約は、すべてのアクションの種類では使用できない場合があります。</span><span class="sxs-lookup"><span data-stu-id="4e241-106">Analytics aggregates might not be available for all action types.</span></span>

[itemActivityStats]: ../resources/itemactivitystat.md

## <a name="permissions"></a><span data-ttu-id="4e241-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4e241-108">Permissions</span></span>

<span data-ttu-id="4e241-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4e241-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e241-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4e241-111">Permission type</span></span>                        | <span data-ttu-id="4e241-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4e241-112">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="4e241-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4e241-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="4e241-114">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e241-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="4e241-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4e241-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4e241-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4e241-116">Not supported.</span></span>
|<span data-ttu-id="4e241-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4e241-117">Application</span></span>                            | <span data-ttu-id="4e241-118">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e241-118">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="4e241-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4e241-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-01-01',endDateTime='2017-01-10',interval='day')
GET /sites/{site-id}/getActivitiesByInterval(startDateTime='2016',endDateTime='2017',interval='month')
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-05-01',interval='week')
```

## <a name="function-parameters"></a><span data-ttu-id="4e241-120">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="4e241-120">Function parameters</span></span>

| <span data-ttu-id="4e241-121">パラメーター</span><span class="sxs-lookup"><span data-stu-id="4e241-121">Parameter</span></span>      | <span data-ttu-id="4e241-122">型</span><span class="sxs-lookup"><span data-stu-id="4e241-122">Type</span></span>               | <span data-ttu-id="4e241-123">説明</span><span class="sxs-lookup"><span data-stu-id="4e241-123">Description</span></span>
|:---------------|:-------------------|:---------------------------------------
| <span data-ttu-id="4e241-124">startDateTime</span><span class="sxs-lookup"><span data-stu-id="4e241-124">startDateTime</span></span>  | <span data-ttu-id="4e241-125">string (タイムスタンプ)</span><span class="sxs-lookup"><span data-stu-id="4e241-125">string (timestamp)</span></span> | <span data-ttu-id="4e241-126">アクティビティを集計する開始時刻。</span><span class="sxs-lookup"><span data-stu-id="4e241-126">The start time over which to aggregate activities.</span></span>
| <span data-ttu-id="4e241-127">endDateTime</span><span class="sxs-lookup"><span data-stu-id="4e241-127">endDateTime</span></span>    | <span data-ttu-id="4e241-128">string (タイムスタンプ)</span><span class="sxs-lookup"><span data-stu-id="4e241-128">string (timestamp)</span></span> | <span data-ttu-id="4e241-129">アクティビティを集約する終了時刻。</span><span class="sxs-lookup"><span data-stu-id="4e241-129">The end time over which to aggregate activities.</span></span>
| <span data-ttu-id="4e241-130">interval</span><span class="sxs-lookup"><span data-stu-id="4e241-130">interval</span></span>       | <span data-ttu-id="4e241-131">string</span><span class="sxs-lookup"><span data-stu-id="4e241-131">string</span></span>             | <span data-ttu-id="4e241-132">集約間隔。</span><span class="sxs-lookup"><span data-stu-id="4e241-132">The aggregation interval.</span></span>

## <a name="example"></a><span data-ttu-id="4e241-133">例</span><span class="sxs-lookup"><span data-stu-id="4e241-133">Example</span></span>

#### <a name="request"></a><span data-ttu-id="4e241-134">要求</span><span class="sxs-lookup"><span data-stu-id="4e241-134">Request</span></span>

<!-- { "blockType": "request", "name": "get-activities-by-interval" } -->

```http
GET /drives/{drive-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-01-01',endDateTime='2017-01-3',interval='day')
```

#### <a name="response"></a><span data-ttu-id="4e241-135">応答</span><span class="sxs-lookup"><span data-stu-id="4e241-135">Response</span></span>

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

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "BaseItem/Get activities by interval",
  "suppressions": []
}
-->
