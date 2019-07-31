---
title: workbookChartSeries リソースの種類
description: グラフのデータ系列を表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: c7f7c8108ac17e6705b8bf5f69b0e87f0dc96b31
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007250"
---
# <a name="workbookchartseries-resource-type"></a><span data-ttu-id="74b16-103">workbookChartSeries リソースの種類</span><span class="sxs-lookup"><span data-stu-id="74b16-103">workbookChartSeries resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="74b16-104">グラフのデータ系列を表します。</span><span class="sxs-lookup"><span data-stu-id="74b16-104">Represents a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="74b16-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="74b16-105">Methods</span></span>

| <span data-ttu-id="74b16-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="74b16-106">Method</span></span>           | <span data-ttu-id="74b16-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="74b16-107">Return Type</span></span>    |<span data-ttu-id="74b16-108">説明</span><span class="sxs-lookup"><span data-stu-id="74b16-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="74b16-109">Get ChartSeries</span><span class="sxs-lookup"><span data-stu-id="74b16-109">Get ChartSeries</span></span>](../api/chartseries-get.md) | [<span data-ttu-id="74b16-110">workbookChartSeries</span><span class="sxs-lookup"><span data-stu-id="74b16-110">workbookChartSeries</span></span>](workbookchartseries.md) |<span data-ttu-id="74b16-111">chartSeries オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="74b16-111">Read properties and relationships of chartSeries object.</span></span>|
|[<span data-ttu-id="74b16-112">ChartPoint を作成する</span><span class="sxs-lookup"><span data-stu-id="74b16-112">Create ChartPoint</span></span>](../api/chartseries-post-points.md) |[<span data-ttu-id="74b16-113">chartPoints</span><span class="sxs-lookup"><span data-stu-id="74b16-113">chartPoints</span></span>](workbookchartpoint.md)| <span data-ttu-id="74b16-114">Points コレクションへの投稿によって、新しい chartPoint を作成します。</span><span class="sxs-lookup"><span data-stu-id="74b16-114">Create a new chartPoint by posting to the points collection.</span></span>|
|[<span data-ttu-id="74b16-115">ポイントを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="74b16-115">List points</span></span>](../api/chartseries-list-points.md) |<span data-ttu-id="74b16-116">[workbookChartPoints](workbookchartpoint.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="74b16-116">[workbookChartPoints](workbookchartpoint.md) collection</span></span>| <span data-ttu-id="74b16-117">ChartPoints オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="74b16-117">Get a chartPoints object collection.</span></span>|
|[<span data-ttu-id="74b16-118">Update</span><span class="sxs-lookup"><span data-stu-id="74b16-118">Update</span></span>](../api/chartseries-update.md) | [<span data-ttu-id="74b16-119">workbookChartSeries</span><span class="sxs-lookup"><span data-stu-id="74b16-119">workbookChartSeries</span></span>](workbookchartseries.md) |<span data-ttu-id="74b16-120">ChartSeries オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="74b16-120">Update chartSeries object.</span></span> |
|[<span data-ttu-id="74b16-121">List</span><span class="sxs-lookup"><span data-stu-id="74b16-121">List</span></span>](../api/chartseries-list.md) | <span data-ttu-id="74b16-122">[workbookChartSeries](workbookchartseries.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="74b16-122">[workbookChartSeries](workbookchartseries.md) collection</span></span> |<span data-ttu-id="74b16-123">chartSeries オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="74b16-123">Get chartSeries object collection.</span></span> |
|[<span data-ttu-id="74b16-124">ItemAt</span><span class="sxs-lookup"><span data-stu-id="74b16-124">ItemAt</span></span>](../api/chartseriescollection-itemat.md)|[<span data-ttu-id="74b16-125">workbookChartSeries</span><span class="sxs-lookup"><span data-stu-id="74b16-125">workbookChartSeries</span></span>](workbookchartseries.md)|<span data-ttu-id="74b16-126">コレクション内の位置に基づいてデータ系列を取得します。</span><span class="sxs-lookup"><span data-stu-id="74b16-126">Retrieves a series based on its position in the collection</span></span>|

## <a name="properties"></a><span data-ttu-id="74b16-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="74b16-127">Properties</span></span>
| <span data-ttu-id="74b16-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="74b16-128">Property</span></span>     | <span data-ttu-id="74b16-129">型</span><span class="sxs-lookup"><span data-stu-id="74b16-129">Type</span></span>   |<span data-ttu-id="74b16-130">説明</span><span class="sxs-lookup"><span data-stu-id="74b16-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="74b16-131">name</span><span class="sxs-lookup"><span data-stu-id="74b16-131">name</span></span>|<span data-ttu-id="74b16-132">string</span><span class="sxs-lookup"><span data-stu-id="74b16-132">string</span></span>|<span data-ttu-id="74b16-133">グラフのデータ系列の名前を表します。</span><span class="sxs-lookup"><span data-stu-id="74b16-133">Represents the name of a series in a chart.</span></span>|

## <a name="relationships"></a><span data-ttu-id="74b16-134">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="74b16-134">Relationships</span></span>
| <span data-ttu-id="74b16-135">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="74b16-135">Relationship</span></span> | <span data-ttu-id="74b16-136">型</span><span class="sxs-lookup"><span data-stu-id="74b16-136">Type</span></span>   |<span data-ttu-id="74b16-137">説明</span><span class="sxs-lookup"><span data-stu-id="74b16-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="74b16-138">format</span><span class="sxs-lookup"><span data-stu-id="74b16-138">format</span></span>|[<span data-ttu-id="74b16-139">workbookChartSeriesFormat</span><span class="sxs-lookup"><span data-stu-id="74b16-139">workbookChartSeriesFormat</span></span>](workbookchartseriesformat.md)|<span data-ttu-id="74b16-p101">グラフ の系列の書式設定を表します。これには塗りつぶしと線の書式設定などがあります。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="74b16-p101">Represents the formatting of a chart series, which includes fill and line formatting. Read-only.</span></span>|
|<span data-ttu-id="74b16-142">points</span><span class="sxs-lookup"><span data-stu-id="74b16-142">points</span></span>|<span data-ttu-id="74b16-143">[workbookChartPoint](workbookchartpoint.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="74b16-143">[workbookChartPoint](workbookchartpoint.md) collection</span></span>|<span data-ttu-id="74b16-144">データ系列にあるすべてのポイントのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="74b16-144">Represents a collection of all points in the series.</span></span> <span data-ttu-id="74b16-145">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="74b16-145">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="74b16-146">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="74b16-146">JSON representation</span></span>

<span data-ttu-id="74b16-147">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="74b16-147">Here is a JSON representation of the resource.</span></span>

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
