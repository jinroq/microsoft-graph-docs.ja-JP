---
title: ChartSeries リソースの種類
description: グラフのデータ系列を表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: e5606516092633ff14d23947f73626adc6d83c2c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519662"
---
# <a name="chartseries-resource-type"></a><span data-ttu-id="e1430-103">ChartSeries リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e1430-103">ChartSeries resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e1430-104">グラフのデータ系列を表します。</span><span class="sxs-lookup"><span data-stu-id="e1430-104">Represents a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="e1430-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="e1430-105">Methods</span></span>

| <span data-ttu-id="e1430-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="e1430-106">Method</span></span>           | <span data-ttu-id="e1430-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="e1430-107">Return Type</span></span>    |<span data-ttu-id="e1430-108">説明</span><span class="sxs-lookup"><span data-stu-id="e1430-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e1430-109">Get ChartSeries</span><span class="sxs-lookup"><span data-stu-id="e1430-109">[Get ChartSeries](../api/chartseries-get.md)</span></span> | [<span data-ttu-id="e1430-110">chartSeries</span><span class="sxs-lookup"><span data-stu-id="e1430-110">ChartSeries</span></span>](chartseries.md) |<span data-ttu-id="e1430-111">chartSeries オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="e1430-111">Read properties and relationships of chartSeries object.</span></span>|
|<span data-ttu-id="e1430-112">ChartPoints を作成する</span><span class="sxs-lookup"><span data-stu-id="e1430-112">[Create ChartPoints](../api/chartseries-post-points.md)</span></span> |<span data-ttu-id="e1430-113">ChartPoints</span><span class="sxs-lookup"><span data-stu-id="e1430-113">[ChartPoints](chartpoint.md)</span></span>| <span data-ttu-id="e1430-114">ポイント コレクションに投稿して、新しい ChartPoints を作成します。</span><span class="sxs-lookup"><span data-stu-id="e1430-114">Create a new ChartPoints by posting to the points collection.</span></span>|
|<span data-ttu-id="e1430-115">ポイントを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="e1430-115">[List points](../api/chartseries-list-points.md)</span></span> |<span data-ttu-id="e1430-116">ChartPoints コレクション</span><span class="sxs-lookup"><span data-stu-id="e1430-116">[ChartPoints](chartpoint.md) collection</span></span>| <span data-ttu-id="e1430-117">ChartPoints オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="e1430-117">Get a ChartPoints object collection.</span></span>|
|[<span data-ttu-id="e1430-118">Update</span><span class="sxs-lookup"><span data-stu-id="e1430-118">Update</span></span>](../api/chartseries-update.md) | [<span data-ttu-id="e1430-119">chartSeries</span><span class="sxs-lookup"><span data-stu-id="e1430-119">ChartSeries</span></span>](chartseries.md) |<span data-ttu-id="e1430-120">ChartSeries オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="e1430-120">Update ChartSeries object.</span></span> |
|[<span data-ttu-id="e1430-121">List</span><span class="sxs-lookup"><span data-stu-id="e1430-121">List</span></span>](../api/chartseries-list.md) | <span data-ttu-id="e1430-122">ChartSeries コレクション</span><span class="sxs-lookup"><span data-stu-id="e1430-122">[ChartSeries](chartseries.md) collection</span></span> |<span data-ttu-id="e1430-123">chartSeries オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="e1430-123">Get chartSeries object collection.</span></span> |
|[<span data-ttu-id="e1430-124">Itemat</span><span class="sxs-lookup"><span data-stu-id="e1430-124">Itemat</span></span>](../api/chartseriescollection-itemat.md)|<span data-ttu-id="e1430-125">ChartSeries</span><span class="sxs-lookup"><span data-stu-id="e1430-125">[ChartSeries](chartseries.md)</span></span>|<span data-ttu-id="e1430-126">コレクション内の位置に基づいてデータ系列を取得します。</span><span class="sxs-lookup"><span data-stu-id="e1430-126">Retrieves a series based on its position in the collection</span></span>|

## <a name="properties"></a><span data-ttu-id="e1430-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e1430-127">Properties</span></span>
| <span data-ttu-id="e1430-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e1430-128">Property</span></span>     | <span data-ttu-id="e1430-129">型</span><span class="sxs-lookup"><span data-stu-id="e1430-129">Type</span></span>   |<span data-ttu-id="e1430-130">説明</span><span class="sxs-lookup"><span data-stu-id="e1430-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e1430-131">name</span><span class="sxs-lookup"><span data-stu-id="e1430-131">name</span></span>|<span data-ttu-id="e1430-132">文字列</span><span class="sxs-lookup"><span data-stu-id="e1430-132">string</span></span>|<span data-ttu-id="e1430-133">グラフのデータ系列の名前を表します。</span><span class="sxs-lookup"><span data-stu-id="e1430-133">Represents the name of a series in a chart.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e1430-134">関係</span><span class="sxs-lookup"><span data-stu-id="e1430-134">Relationships</span></span>
| <span data-ttu-id="e1430-135">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e1430-135">Relationship</span></span> | <span data-ttu-id="e1430-136">型</span><span class="sxs-lookup"><span data-stu-id="e1430-136">Type</span></span>   |<span data-ttu-id="e1430-137">説明</span><span class="sxs-lookup"><span data-stu-id="e1430-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e1430-138">format</span><span class="sxs-lookup"><span data-stu-id="e1430-138">format</span></span>|[<span data-ttu-id="e1430-139">ChartSeriesFormat</span><span class="sxs-lookup"><span data-stu-id="e1430-139">ChartSeriesFormat</span></span>](chartseriesformat.md)|<span data-ttu-id="e1430-p101">グラフ の系列の書式設定を表します。これには塗りつぶしと線の書式設定などがあります。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="e1430-p101">Represents the formatting of a chart series, which includes fill and line formatting. Read-only.</span></span>|
|<span data-ttu-id="e1430-142">points</span><span class="sxs-lookup"><span data-stu-id="e1430-142">points</span></span>|<span data-ttu-id="e1430-143">[ChartPoints](chartpoint.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e1430-143">[ChartPoints](chartpoint.md) collection</span></span>|<span data-ttu-id="e1430-p102">データ系列にあるすべてのポイントのコレクションを返します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="e1430-p102">Represents a collection of all points in the series. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e1430-146">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e1430-146">JSON representation</span></span>

<span data-ttu-id="e1430-147">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e1430-147">Here is a JSON representation of the resource.</span></span>

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
