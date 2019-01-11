---
title: ChartSeries リソースの種類
description: グラフのデータ系列を表します。
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: a3a19793629a5e100830565e224541930e2180de
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834896"
---
# <a name="chartseries-resource-type"></a><span data-ttu-id="1afc5-103">ChartSeries リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1afc5-103">ChartSeries resource type</span></span>

<span data-ttu-id="1afc5-104">グラフのデータ系列を表します。</span><span class="sxs-lookup"><span data-stu-id="1afc5-104">Represents a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="1afc5-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="1afc5-105">Methods</span></span>

| <span data-ttu-id="1afc5-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="1afc5-106">Method</span></span>           | <span data-ttu-id="1afc5-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="1afc5-107">Return Type</span></span>    |<span data-ttu-id="1afc5-108">説明</span><span class="sxs-lookup"><span data-stu-id="1afc5-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1afc5-109">Get ChartSeries</span><span class="sxs-lookup"><span data-stu-id="1afc5-109">Get ChartSeries</span></span>](../api/chartseries-get.md) | [<span data-ttu-id="1afc5-110">WorkbookChartSeries</span><span class="sxs-lookup"><span data-stu-id="1afc5-110">WorkbookChartSeries</span></span>](chartseries.md) |<span data-ttu-id="1afc5-111">chartSeries オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="1afc5-111">Read properties and relationships of chartSeries object.</span></span>|
|[<span data-ttu-id="1afc5-112">ChartPoints を作成する</span><span class="sxs-lookup"><span data-stu-id="1afc5-112">Create ChartPoints</span></span>](../api/chartseries-post-points.md) |[<span data-ttu-id="1afc5-113">ChartPoints</span><span class="sxs-lookup"><span data-stu-id="1afc5-113">ChartPoints</span></span>](chartpoint.md)| <span data-ttu-id="1afc5-114">ポイント コレクションに投稿して、新しい ChartPoints を作成します。</span><span class="sxs-lookup"><span data-stu-id="1afc5-114">Create a new ChartPoints by posting to the points collection.</span></span>|
|[<span data-ttu-id="1afc5-115">ポイントを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="1afc5-115">List points</span></span>](../api/chartseries-list-points.md) |<span data-ttu-id="1afc5-116">[ChartPoints](chartpoint.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="1afc5-116">[ChartPoints](chartpoint.md) collection</span></span>| <span data-ttu-id="1afc5-117">ChartPoints オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="1afc5-117">Get a ChartPoints object collection.</span></span>|
|[<span data-ttu-id="1afc5-118">Update</span><span class="sxs-lookup"><span data-stu-id="1afc5-118">Update</span></span>](../api/chartseries-update.md) | [<span data-ttu-id="1afc5-119">WorkbookChartSeries</span><span class="sxs-lookup"><span data-stu-id="1afc5-119">WorkbookChartSeries</span></span>](chartseries.md) |<span data-ttu-id="1afc5-120">ChartSeries オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="1afc5-120">Update ChartSeries object.</span></span> |
|[<span data-ttu-id="1afc5-121">List</span><span class="sxs-lookup"><span data-stu-id="1afc5-121">List</span></span>](../api/chartseries-list.md) | <span data-ttu-id="1afc5-122">[WorkbookChartSeries](chartseries.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="1afc5-122">[WorkbookChartSeries](chartseries.md) collection</span></span> |<span data-ttu-id="1afc5-123">chartSeries オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="1afc5-123">Get chartSeries object collection.</span></span> |
|[<span data-ttu-id="1afc5-124">ItemAt</span><span class="sxs-lookup"><span data-stu-id="1afc5-124">ItemAt</span></span>](../api/chartseriescollection-itemat.md)|[<span data-ttu-id="1afc5-125">WorkbookChartSeries</span><span class="sxs-lookup"><span data-stu-id="1afc5-125">WorkbookChartSeries</span></span>](chartseries.md)|<span data-ttu-id="1afc5-126">コレクション内の位置に基づいてデータ系列を取得します。</span><span class="sxs-lookup"><span data-stu-id="1afc5-126">Retrieves a series based on its position in the collection</span></span>|

## <a name="properties"></a><span data-ttu-id="1afc5-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1afc5-127">Properties</span></span>
| <span data-ttu-id="1afc5-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1afc5-128">Property</span></span>     | <span data-ttu-id="1afc5-129">種類</span><span class="sxs-lookup"><span data-stu-id="1afc5-129">Type</span></span>   |<span data-ttu-id="1afc5-130">説明</span><span class="sxs-lookup"><span data-stu-id="1afc5-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1afc5-131">name</span><span class="sxs-lookup"><span data-stu-id="1afc5-131">name</span></span>|<span data-ttu-id="1afc5-132">文字列</span><span class="sxs-lookup"><span data-stu-id="1afc5-132">string</span></span>|<span data-ttu-id="1afc5-133">グラフのデータ系列の名前を表します。</span><span class="sxs-lookup"><span data-stu-id="1afc5-133">Represents the name of a series in a chart.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1afc5-134">関係</span><span class="sxs-lookup"><span data-stu-id="1afc5-134">Relationships</span></span>
| <span data-ttu-id="1afc5-135">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1afc5-135">Relationship</span></span> | <span data-ttu-id="1afc5-136">型</span><span class="sxs-lookup"><span data-stu-id="1afc5-136">Type</span></span>   |<span data-ttu-id="1afc5-137">説明</span><span class="sxs-lookup"><span data-stu-id="1afc5-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1afc5-138">format</span><span class="sxs-lookup"><span data-stu-id="1afc5-138">format</span></span>|[<span data-ttu-id="1afc5-139">WorkbookChartSeriesFormat</span><span class="sxs-lookup"><span data-stu-id="1afc5-139">WorkbookChartSeriesFormat</span></span>](chartseriesformat.md)|<span data-ttu-id="1afc5-p101">グラフ の系列の書式設定を表します。これには塗りつぶしと線の書式設定などがあります。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="1afc5-p101">Represents the formatting of a chart series, which includes fill and line formatting. Read-only.</span></span>|
|<span data-ttu-id="1afc5-142">points</span><span class="sxs-lookup"><span data-stu-id="1afc5-142">points</span></span>|<span data-ttu-id="1afc5-143">[WorkbookChartPoint](chartpoint.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="1afc5-143">[WorkbookChartPoint](chartpoint.md) collection</span></span>|<span data-ttu-id="1afc5-p102">データ系列にあるすべてのポイントのコレクションを返します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="1afc5-p102">Represents a collection of all points in the series. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1afc5-146">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1afc5-146">JSON representation</span></span>

<span data-ttu-id="1afc5-147">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1afc5-147">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "ChartSeries resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
