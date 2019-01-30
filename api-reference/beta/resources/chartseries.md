---
title: ChartSeries リソースの種類
description: グラフのデータ系列を表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: e5606516092633ff14d23947f73626adc6d83c2c
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643116"
---
# <a name="chartseries-resource-type"></a><span data-ttu-id="e313a-103">ChartSeries リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e313a-103">ChartSeries resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e313a-104">グラフのデータ系列を表します。</span><span class="sxs-lookup"><span data-stu-id="e313a-104">Represents a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="e313a-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="e313a-105">Methods</span></span>

| <span data-ttu-id="e313a-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="e313a-106">Method</span></span>           | <span data-ttu-id="e313a-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="e313a-107">Return Type</span></span>    |<span data-ttu-id="e313a-108">説明</span><span class="sxs-lookup"><span data-stu-id="e313a-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e313a-109">Get ChartSeries</span><span class="sxs-lookup"><span data-stu-id="e313a-109">Get ChartSeries</span></span>](../api/chartseries-get.md) | [<span data-ttu-id="e313a-110">ChartSeries</span><span class="sxs-lookup"><span data-stu-id="e313a-110">ChartSeries</span></span>](chartseries.md) |<span data-ttu-id="e313a-111">chartSeries オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="e313a-111">Read properties and relationships of chartSeries object.</span></span>|
|[<span data-ttu-id="e313a-112">ChartPoints を作成する</span><span class="sxs-lookup"><span data-stu-id="e313a-112">Create ChartPoints</span></span>](../api/chartseries-post-points.md) |[<span data-ttu-id="e313a-113">ChartPoints</span><span class="sxs-lookup"><span data-stu-id="e313a-113">ChartPoints</span></span>](chartpoint.md)| <span data-ttu-id="e313a-114">ポイント コレクションに投稿して、新しい ChartPoints を作成します。</span><span class="sxs-lookup"><span data-stu-id="e313a-114">Create a new ChartPoints by posting to the points collection.</span></span>|
|[<span data-ttu-id="e313a-115">ポイントを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="e313a-115">List points</span></span>](../api/chartseries-list-points.md) |<span data-ttu-id="e313a-116">[ChartPoints](chartpoint.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e313a-116">[ChartPoints](chartpoint.md) collection</span></span>| <span data-ttu-id="e313a-117">ChartPoints オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="e313a-117">Get a ChartPoints object collection.</span></span>|
|[<span data-ttu-id="e313a-118">更新する</span><span class="sxs-lookup"><span data-stu-id="e313a-118">Update</span></span>](../api/chartseries-update.md) | [<span data-ttu-id="e313a-119">ChartSeries</span><span class="sxs-lookup"><span data-stu-id="e313a-119">ChartSeries</span></span>](chartseries.md) |<span data-ttu-id="e313a-120">ChartSeries オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="e313a-120">Update ChartSeries object.</span></span> |
|[<span data-ttu-id="e313a-121">List</span><span class="sxs-lookup"><span data-stu-id="e313a-121">List</span></span>](../api/chartseries-list.md) | <span data-ttu-id="e313a-122">[ChartSeries](chartseries.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e313a-122">[ChartSeries](chartseries.md) collection</span></span> |<span data-ttu-id="e313a-123">chartSeries オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="e313a-123">Get chartSeries object collection.</span></span> |
|[<span data-ttu-id="e313a-124">Itemat</span><span class="sxs-lookup"><span data-stu-id="e313a-124">Itemat</span></span>](../api/chartseriescollection-itemat.md)|[<span data-ttu-id="e313a-125">ChartSeries</span><span class="sxs-lookup"><span data-stu-id="e313a-125">ChartSeries</span></span>](chartseries.md)|<span data-ttu-id="e313a-126">コレクション内の位置に基づいてデータ系列を取得します。</span><span class="sxs-lookup"><span data-stu-id="e313a-126">Retrieves a series based on its position in the collection</span></span>|

## <a name="properties"></a><span data-ttu-id="e313a-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e313a-127">Properties</span></span>
| <span data-ttu-id="e313a-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e313a-128">Property</span></span>     | <span data-ttu-id="e313a-129">型</span><span class="sxs-lookup"><span data-stu-id="e313a-129">Type</span></span>   |<span data-ttu-id="e313a-130">説明</span><span class="sxs-lookup"><span data-stu-id="e313a-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e313a-131">name</span><span class="sxs-lookup"><span data-stu-id="e313a-131">name</span></span>|<span data-ttu-id="e313a-132">文字列</span><span class="sxs-lookup"><span data-stu-id="e313a-132">string</span></span>|<span data-ttu-id="e313a-133">グラフのデータ系列の名前を表します。</span><span class="sxs-lookup"><span data-stu-id="e313a-133">Represents the name of a series in a chart.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e313a-134">関係</span><span class="sxs-lookup"><span data-stu-id="e313a-134">Relationships</span></span>
| <span data-ttu-id="e313a-135">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e313a-135">Relationship</span></span> | <span data-ttu-id="e313a-136">型</span><span class="sxs-lookup"><span data-stu-id="e313a-136">Type</span></span>   |<span data-ttu-id="e313a-137">説明</span><span class="sxs-lookup"><span data-stu-id="e313a-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e313a-138">format</span><span class="sxs-lookup"><span data-stu-id="e313a-138">format</span></span>|[<span data-ttu-id="e313a-139">ChartSeriesFormat</span><span class="sxs-lookup"><span data-stu-id="e313a-139">ChartSeriesFormat</span></span>](chartseriesformat.md)|<span data-ttu-id="e313a-p101">グラフ の系列の書式設定を表します。これには塗りつぶしと線の書式設定などがあります。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="e313a-p101">Represents the formatting of a chart series, which includes fill and line formatting. Read-only.</span></span>|
|<span data-ttu-id="e313a-142">points</span><span class="sxs-lookup"><span data-stu-id="e313a-142">points</span></span>|<span data-ttu-id="e313a-143">[ChartPoints](chartpoint.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e313a-143">[ChartPoints](chartpoint.md) collection</span></span>|<span data-ttu-id="e313a-p102">データ系列にあるすべてのポイントのコレクションを返します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="e313a-p102">Represents a collection of all points in the series. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e313a-146">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e313a-146">JSON representation</span></span>

<span data-ttu-id="e313a-147">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e313a-147">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartSeries"
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
  "suppressions": [
    "Error: /api-reference/beta/resources/chartseries.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
