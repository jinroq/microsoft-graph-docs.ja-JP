---
author: daspek
ms.author: dspektor
ms.date: 10/06/2017
title: 間隔ごとにアイテムアクティビティの統計情報を取得する
localization_priority: Normal
ms.openlocfilehash: f9601538d825efe346ab57fdbecd6c74dc9978d7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32541312"
---
# <a name="get-item-activity-stats-by-interval"></a><span data-ttu-id="29fe9-102">間隔ごとにアイテムアクティビティの統計情報を取得する</span><span class="sxs-lookup"><span data-stu-id="29fe9-102">Get item activity stats by interval</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="29fe9-103">このリソースの下で、指定された期間内に行われたアクティビティの[itemactivitystats][]を取得します。</span><span class="sxs-lookup"><span data-stu-id="29fe9-103">Get [itemActivityStats][] for the activities that took place under this resource within the specified time interval.</span></span>

><span data-ttu-id="29fe9-104">**注:\*\*\*\*itemanalytics**リソースは、すべての[国内展開](/graph/deployments)でまだ使用できません。</span><span class="sxs-lookup"><span data-stu-id="29fe9-104">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

<span data-ttu-id="29fe9-105">分析集約は、すべてのアクションの種類では使用できない場合があります。</span><span class="sxs-lookup"><span data-stu-id="29fe9-105">Analytics aggregates might not be available for all action types.</span></span>

[itemactivitystats]: ../resources/itemactivitystat.md
[itemActivityStats]: ../resources/itemactivitystat.md

## <a name="permissions"></a><span data-ttu-id="29fe9-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="29fe9-107">Permissions</span></span>

<span data-ttu-id="29fe9-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="29fe9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="29fe9-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="29fe9-110">Permission type</span></span>                        | <span data-ttu-id="29fe9-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="29fe9-111">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="29fe9-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="29fe9-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="29fe9-113">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29fe9-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="29fe9-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="29fe9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="29fe9-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="29fe9-115">Not supported.</span></span>
|<span data-ttu-id="29fe9-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="29fe9-116">Application</span></span>                            | <span data-ttu-id="29fe9-117">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29fe9-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="29fe9-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="29fe9-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-01-01',endDateTime='2017-01-10',interval='day')
GET /sites/{site-id}/getActivitiesByInterval(startDateTime='2016',endDateTime='2017',interval='month')
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-05-01',interval='week')
```

## <a name="function-parameters"></a><span data-ttu-id="29fe9-119">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="29fe9-119">Function parameters</span></span>

| <span data-ttu-id="29fe9-120">パラメーター</span><span class="sxs-lookup"><span data-stu-id="29fe9-120">Parameter</span></span>      | <span data-ttu-id="29fe9-121">型</span><span class="sxs-lookup"><span data-stu-id="29fe9-121">Type</span></span>               | <span data-ttu-id="29fe9-122">説明</span><span class="sxs-lookup"><span data-stu-id="29fe9-122">Description</span></span>
|:---------------|:-------------------|:---------------------------------------
| <span data-ttu-id="29fe9-123">startDateTime</span><span class="sxs-lookup"><span data-stu-id="29fe9-123">startDateTime</span></span>  | <span data-ttu-id="29fe9-124">string (タイムスタンプ)</span><span class="sxs-lookup"><span data-stu-id="29fe9-124">string (timestamp)</span></span> | <span data-ttu-id="29fe9-125">アクティビティを集計する開始時刻。</span><span class="sxs-lookup"><span data-stu-id="29fe9-125">The start time over which to aggregate activities.</span></span>
| <span data-ttu-id="29fe9-126">endDateTime</span><span class="sxs-lookup"><span data-stu-id="29fe9-126">endDateTime</span></span>    | <span data-ttu-id="29fe9-127">string (タイムスタンプ)</span><span class="sxs-lookup"><span data-stu-id="29fe9-127">string (timestamp)</span></span> | <span data-ttu-id="29fe9-128">アクティビティを集約する終了時刻。</span><span class="sxs-lookup"><span data-stu-id="29fe9-128">The end time over which to aggregate activities.</span></span>
| <span data-ttu-id="29fe9-129">interval</span><span class="sxs-lookup"><span data-stu-id="29fe9-129">interval</span></span>       | <span data-ttu-id="29fe9-130">string</span><span class="sxs-lookup"><span data-stu-id="29fe9-130">string</span></span>             | <span data-ttu-id="29fe9-131">集約間隔。</span><span class="sxs-lookup"><span data-stu-id="29fe9-131">The aggregation interval.</span></span>

## <a name="example"></a><span data-ttu-id="29fe9-132">例</span><span class="sxs-lookup"><span data-stu-id="29fe9-132">Example</span></span>

#### <a name="request"></a><span data-ttu-id="29fe9-133">要求</span><span class="sxs-lookup"><span data-stu-id="29fe9-133">Request</span></span>

<!-- { "blockType": "request", "name": "get-activities-by-interval" } -->

```http
GET /drives/{drive-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-01-01',endDateTime='2017-01-3',interval='day')
```

#### <a name="response"></a><span data-ttu-id="29fe9-134">応答</span><span class="sxs-lookup"><span data-stu-id="29fe9-134">Response</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/api/itemactivity-getbyinterval.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
