---
title: workbookChartSeries リソースの種類
description: グラフのデータ系列を表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: e9ff478a5f7e91c3d116ca2dbd78e20699077aab
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348885"
---
# <a name="workbookchartseries-resource-type"></a><span data-ttu-id="c9d0f-103">workbookChartSeries リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c9d0f-103">workbookChartSeries resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c9d0f-104">グラフのデータ系列を表します。</span><span class="sxs-lookup"><span data-stu-id="c9d0f-104">Represents a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="c9d0f-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="c9d0f-105">Methods</span></span>

| <span data-ttu-id="c9d0f-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="c9d0f-106">Method</span></span>           | <span data-ttu-id="c9d0f-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="c9d0f-107">Return Type</span></span>    |<span data-ttu-id="c9d0f-108">説明</span><span class="sxs-lookup"><span data-stu-id="c9d0f-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c9d0f-109">Get ChartSeries</span><span class="sxs-lookup"><span data-stu-id="c9d0f-109">Get ChartSeries</span></span>](../api/chartseries-get.md) | [<span data-ttu-id="c9d0f-110">workbookChartSeries</span><span class="sxs-lookup"><span data-stu-id="c9d0f-110">workbookChartSeries</span></span>](workbookchartseries.md) |<span data-ttu-id="c9d0f-111">chartSeries オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="c9d0f-111">Read properties and relationships of chartSeries object.</span></span>|
|[<span data-ttu-id="c9d0f-112">chartpoint を作成する</span><span class="sxs-lookup"><span data-stu-id="c9d0f-112">Create ChartPoint</span></span>](../api/chartseries-post-points.md) |[<span data-ttu-id="c9d0f-113">chartPoints</span><span class="sxs-lookup"><span data-stu-id="c9d0f-113">chartPoints</span></span>](workbookchartpoint.md)| <span data-ttu-id="c9d0f-114">points コレクションへの投稿によって、新しい chartpoint を作成します。</span><span class="sxs-lookup"><span data-stu-id="c9d0f-114">Create a new chartPoint by posting to the points collection.</span></span>|
|[<span data-ttu-id="c9d0f-115">ポイントを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="c9d0f-115">List points</span></span>](../api/chartseries-list-points.md) |<span data-ttu-id="c9d0f-116">[workbookChartPoints](workbookchartpoint.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="c9d0f-116">[workbookChartPoints](workbookchartpoint.md) collection</span></span>| <span data-ttu-id="c9d0f-117">chartpoints オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="c9d0f-117">Get a chartPoints object collection.</span></span>|
|[<span data-ttu-id="c9d0f-118">更新する</span><span class="sxs-lookup"><span data-stu-id="c9d0f-118">Update</span></span>](../api/chartseries-update.md) | [<span data-ttu-id="c9d0f-119">workbookChartSeries</span><span class="sxs-lookup"><span data-stu-id="c9d0f-119">workbookChartSeries</span></span>](workbookchartseries.md) |<span data-ttu-id="c9d0f-120">chartseries オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="c9d0f-120">Update chartSeries object.</span></span> |
|[<span data-ttu-id="c9d0f-121">List</span><span class="sxs-lookup"><span data-stu-id="c9d0f-121">List</span></span>](../api/chartseries-list.md) | <span data-ttu-id="c9d0f-122">[workbookChartSeries](workbookchartseries.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="c9d0f-122">[workbookChartSeries](workbookchartseries.md) collection</span></span> |<span data-ttu-id="c9d0f-123">chartSeries オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="c9d0f-123">Get chartSeries object collection.</span></span> |
|[<span data-ttu-id="c9d0f-124">ItemAt</span><span class="sxs-lookup"><span data-stu-id="c9d0f-124">ItemAt</span></span>](../api/chartseriescollection-itemat.md)|[<span data-ttu-id="c9d0f-125">workbookChartSeries</span><span class="sxs-lookup"><span data-stu-id="c9d0f-125">workbookChartSeries</span></span>](workbookchartseries.md)|<span data-ttu-id="c9d0f-126">コレクション内の位置に基づいてデータ系列を取得します。</span><span class="sxs-lookup"><span data-stu-id="c9d0f-126">Retrieves a series based on its position in the collection</span></span>|

## <a name="properties"></a><span data-ttu-id="c9d0f-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c9d0f-127">Properties</span></span>
| <span data-ttu-id="c9d0f-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c9d0f-128">Property</span></span>     | <span data-ttu-id="c9d0f-129">種類</span><span class="sxs-lookup"><span data-stu-id="c9d0f-129">Type</span></span>   |<span data-ttu-id="c9d0f-130">説明</span><span class="sxs-lookup"><span data-stu-id="c9d0f-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c9d0f-131">name</span><span class="sxs-lookup"><span data-stu-id="c9d0f-131">name</span></span>|<span data-ttu-id="c9d0f-132">string</span><span class="sxs-lookup"><span data-stu-id="c9d0f-132">string</span></span>|<span data-ttu-id="c9d0f-133">グラフのデータ系列の名前を表します。</span><span class="sxs-lookup"><span data-stu-id="c9d0f-133">Represents the name of a series in a chart.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c9d0f-134">関係</span><span class="sxs-lookup"><span data-stu-id="c9d0f-134">Relationships</span></span>
| <span data-ttu-id="c9d0f-135">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c9d0f-135">Relationship</span></span> | <span data-ttu-id="c9d0f-136">型</span><span class="sxs-lookup"><span data-stu-id="c9d0f-136">Type</span></span>   |<span data-ttu-id="c9d0f-137">説明</span><span class="sxs-lookup"><span data-stu-id="c9d0f-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c9d0f-138">format</span><span class="sxs-lookup"><span data-stu-id="c9d0f-138">format</span></span>|[<span data-ttu-id="c9d0f-139">workbookChartSeriesFormat</span><span class="sxs-lookup"><span data-stu-id="c9d0f-139">workbookChartSeriesFormat</span></span>](workbookchartseriesformat.md)|<span data-ttu-id="c9d0f-p101">グラフ の系列の書式設定を表します。これには塗りつぶしと線の書式設定などがあります。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="c9d0f-p101">Represents the formatting of a chart series, which includes fill and line formatting. Read-only.</span></span>|
|<span data-ttu-id="c9d0f-142">points</span><span class="sxs-lookup"><span data-stu-id="c9d0f-142">points</span></span>|<span data-ttu-id="c9d0f-143">[workbookChartPoint](workbookchartpoint.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="c9d0f-143">[workbookChartPoint](workbookchartpoint.md) collection</span></span>|<span data-ttu-id="c9d0f-144">データ系列にあるすべてのポイントのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="c9d0f-144">Represents a collection of all points in the series.</span></span> <span data-ttu-id="c9d0f-145">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="c9d0f-145">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c9d0f-146">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c9d0f-146">JSON representation</span></span>

<span data-ttu-id="c9d0f-147">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c9d0f-147">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookChartSeries"
}-->

```json
{
  "name": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartSeries resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
