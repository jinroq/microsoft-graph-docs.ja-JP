---
author: daspek
ms.author: dspektor
title: 間隔ごとにアイテムアクティビティの統計情報を取得する
description: 指定された期間内にこのリソースに対して実行されたアクティビティのアイテム分析の統計情報を取得します。
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 30f06f9bcdfb96f61f39b81152f0c9cd23872e49
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36025534"
---
# <a name="get-item-activity-stats-by-interval"></a><span data-ttu-id="05573-103">間隔ごとにアイテムアクティビティの統計情報を取得する</span><span class="sxs-lookup"><span data-stu-id="05573-103">Get item activity stats by interval</span></span>

<span data-ttu-id="05573-104">指定された期間内にこのリソースに対して行われたアクティビティの[Itemactivitystats][]リソースのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="05573-104">Get a collection of [itemActivityStats][] resources for the activities that took place on this resource within the specified time interval.</span></span>

><span data-ttu-id="05573-105">**注:\*\*\*\*Itemanalytics**リソースは、すべての[国内展開](/graph/deployments)でまだ使用できません。</span><span class="sxs-lookup"><span data-stu-id="05573-105">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

<span data-ttu-id="05573-106">分析集約は、すべてのアクションの種類では使用できない場合があります。</span><span class="sxs-lookup"><span data-stu-id="05573-106">Analytics aggregates might not be available for all action types.</span></span>

## <a name="permissions"></a><span data-ttu-id="05573-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="05573-107">Permissions</span></span>

<span data-ttu-id="05573-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="05573-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="05573-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="05573-110">Permission type</span></span>                        | <span data-ttu-id="05573-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="05573-111">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="05573-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="05573-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="05573-113">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05573-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="05573-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="05573-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="05573-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="05573-115">Not supported.</span></span>
|<span data-ttu-id="05573-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="05573-116">Application</span></span>                            | <span data-ttu-id="05573-117">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05573-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="05573-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="05573-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-01-01',endDateTime='2017-01-10',interval='day')
GET /sites/{site-id}/getActivitiesByInterval(startDateTime='2016',endDateTime='2017',interval='month')
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-05-01',interval='week')
```

## <a name="function-parameters"></a><span data-ttu-id="05573-119">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="05573-119">Function parameters</span></span>

| <span data-ttu-id="05573-120">パラメーター</span><span class="sxs-lookup"><span data-stu-id="05573-120">Parameter</span></span>      | <span data-ttu-id="05573-121">型</span><span class="sxs-lookup"><span data-stu-id="05573-121">Type</span></span>               | <span data-ttu-id="05573-122">説明</span><span class="sxs-lookup"><span data-stu-id="05573-122">Description</span></span>
|:---------------|:-------------------|:---------------------------------------
| <span data-ttu-id="05573-123">startDateTime</span><span class="sxs-lookup"><span data-stu-id="05573-123">startDateTime</span></span>  | <span data-ttu-id="05573-124">string (タイムスタンプ)</span><span class="sxs-lookup"><span data-stu-id="05573-124">string (timestamp)</span></span> | <span data-ttu-id="05573-125">アクティビティを集計する開始時刻。</span><span class="sxs-lookup"><span data-stu-id="05573-125">The start time over which to aggregate activities.</span></span>
| <span data-ttu-id="05573-126">endDateTime</span><span class="sxs-lookup"><span data-stu-id="05573-126">endDateTime</span></span>    | <span data-ttu-id="05573-127">string (タイムスタンプ)</span><span class="sxs-lookup"><span data-stu-id="05573-127">string (timestamp)</span></span> | <span data-ttu-id="05573-128">アクティビティを集約する終了時刻。</span><span class="sxs-lookup"><span data-stu-id="05573-128">The end time over which to aggregate activities.</span></span>
| <span data-ttu-id="05573-129">interval</span><span class="sxs-lookup"><span data-stu-id="05573-129">interval</span></span>       | <span data-ttu-id="05573-130">string</span><span class="sxs-lookup"><span data-stu-id="05573-130">string</span></span>             | <span data-ttu-id="05573-131">集約間隔。</span><span class="sxs-lookup"><span data-stu-id="05573-131">The aggregation interval.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="05573-132">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="05573-132">Optional query parameters</span></span>
<span data-ttu-id="05573-133">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="05573-133">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="05573-134">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="05573-134">Request headers</span></span>

| <span data-ttu-id="05573-135">名前</span><span class="sxs-lookup"><span data-stu-id="05573-135">Name</span></span>      |<span data-ttu-id="05573-136">説明</span><span class="sxs-lookup"><span data-stu-id="05573-136">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="05573-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="05573-137">Authorization</span></span>  | <span data-ttu-id="05573-138">ベアラー {code}。</span><span class="sxs-lookup"><span data-stu-id="05573-138">Bearer {code}.</span></span> <span data-ttu-id="05573-139">必須です。</span><span class="sxs-lookup"><span data-stu-id="05573-139">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="05573-140">要求本文</span><span class="sxs-lookup"><span data-stu-id="05573-140">Request body</span></span>

<span data-ttu-id="05573-141">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="05573-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="05573-142">応答</span><span class="sxs-lookup"><span data-stu-id="05573-142">Response</span></span> 

<span data-ttu-id="05573-143">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[itemactivitystats][]オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="05573-143">If successful, this method returns a `200 OK` response code and a collection of [itemActivityStats][] object in the response body.</span></span> 

## <a name="example"></a><span data-ttu-id="05573-144">例</span><span class="sxs-lookup"><span data-stu-id="05573-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="05573-145">要求</span><span class="sxs-lookup"><span data-stu-id="05573-145">Request</span></span>

<!-- { "blockType": "request", "name": "get-activities-by-interval" } -->

```http
GET /drives/{drive-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-01-01',endDateTime='2017-01-3',interval='day')
```

### <a name="response"></a><span data-ttu-id="05573-146">応答</span><span class="sxs-lookup"><span data-stu-id="05573-146">Response</span></span>

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
[itemActivityStats]: ../resources/itemactivitystat.md

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
