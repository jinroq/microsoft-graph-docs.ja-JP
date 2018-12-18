---
title: ChartSeries リソースの種類
description: グラフのデータ系列を表します。
author: lumine2008
ms.openlocfilehash: 443b6b3dfea54b59ff92babc2776d9624bd28b20
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27325285"
---
# <a name="chartseries-resource-type"></a><span data-ttu-id="17cb4-103">ChartSeries リソースの種類</span><span class="sxs-lookup"><span data-stu-id="17cb4-103">ChartSeries resource type</span></span>

> <span data-ttu-id="17cb4-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="17cb4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="17cb4-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="17cb4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="17cb4-106">グラフのデータ系列を表します。</span><span class="sxs-lookup"><span data-stu-id="17cb4-106">Represents a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="17cb4-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="17cb4-107">Methods</span></span>

| <span data-ttu-id="17cb4-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="17cb4-108">Method</span></span>           | <span data-ttu-id="17cb4-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="17cb4-109">Return Type</span></span>    |<span data-ttu-id="17cb4-110">説明</span><span class="sxs-lookup"><span data-stu-id="17cb4-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="17cb4-111">Get ChartSeries</span><span class="sxs-lookup"><span data-stu-id="17cb4-111">Get ChartSeries</span></span>](../api/chartseries-get.md) | [<span data-ttu-id="17cb4-112">ChartSeries</span><span class="sxs-lookup"><span data-stu-id="17cb4-112">ChartSeries</span></span>](chartseries.md) |<span data-ttu-id="17cb4-113">chartSeries オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="17cb4-113">Read properties and relationships of chartSeries object.</span></span>|
|[<span data-ttu-id="17cb4-114">ChartPoints を作成する</span><span class="sxs-lookup"><span data-stu-id="17cb4-114">Create ChartPoints</span></span>](../api/chartseries-post-points.md) |[<span data-ttu-id="17cb4-115">ChartPoints</span><span class="sxs-lookup"><span data-stu-id="17cb4-115">ChartPoints</span></span>](chartpoint.md)| <span data-ttu-id="17cb4-116">ポイント コレクションに投稿して、新しい ChartPoints を作成します。</span><span class="sxs-lookup"><span data-stu-id="17cb4-116">Create a new ChartPoints by posting to the points collection.</span></span>|
|[<span data-ttu-id="17cb4-117">ポイントを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="17cb4-117">List points</span></span>](../api/chartseries-list-points.md) |<span data-ttu-id="17cb4-118">[ChartPoints](chartpoint.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="17cb4-118">[ChartPoints](chartpoint.md) collection</span></span>| <span data-ttu-id="17cb4-119">ChartPoints オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="17cb4-119">Get a ChartPoints object collection.</span></span>|
|[<span data-ttu-id="17cb4-120">Update</span><span class="sxs-lookup"><span data-stu-id="17cb4-120">Update</span></span>](../api/chartseries-update.md) | [<span data-ttu-id="17cb4-121">ChartSeries</span><span class="sxs-lookup"><span data-stu-id="17cb4-121">ChartSeries</span></span>](chartseries.md) |<span data-ttu-id="17cb4-122">ChartSeries オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="17cb4-122">Update ChartSeries object.</span></span> |
|[<span data-ttu-id="17cb4-123">List</span><span class="sxs-lookup"><span data-stu-id="17cb4-123">List</span></span>](../api/chartseries-list.md) | <span data-ttu-id="17cb4-124">[ChartSeries](chartseries.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="17cb4-124">[ChartSeries](chartseries.md) collection</span></span> |<span data-ttu-id="17cb4-125">chartSeries オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="17cb4-125">Get chartSeries object collection.</span></span> |
|[<span data-ttu-id="17cb4-126">Itemat</span><span class="sxs-lookup"><span data-stu-id="17cb4-126">Itemat</span></span>](../api/chartseriescollection-itemat.md)|[<span data-ttu-id="17cb4-127">ChartSeries</span><span class="sxs-lookup"><span data-stu-id="17cb4-127">ChartSeries</span></span>](chartseries.md)|<span data-ttu-id="17cb4-128">コレクション内の位置に基づいてデータ系列を取得します。</span><span class="sxs-lookup"><span data-stu-id="17cb4-128">Retrieves a series based on its position in the collection</span></span>|

## <a name="properties"></a><span data-ttu-id="17cb4-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="17cb4-129">Properties</span></span>
| <span data-ttu-id="17cb4-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="17cb4-130">Property</span></span>     | <span data-ttu-id="17cb4-131">種類</span><span class="sxs-lookup"><span data-stu-id="17cb4-131">Type</span></span>   |<span data-ttu-id="17cb4-132">説明</span><span class="sxs-lookup"><span data-stu-id="17cb4-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="17cb4-133">name</span><span class="sxs-lookup"><span data-stu-id="17cb4-133">name</span></span>|<span data-ttu-id="17cb4-134">文字列</span><span class="sxs-lookup"><span data-stu-id="17cb4-134">string</span></span>|<span data-ttu-id="17cb4-135">グラフのデータ系列の名前を表します。</span><span class="sxs-lookup"><span data-stu-id="17cb4-135">Represents the name of a series in a chart.</span></span>|

## <a name="relationships"></a><span data-ttu-id="17cb4-136">関係</span><span class="sxs-lookup"><span data-stu-id="17cb4-136">Relationships</span></span>
| <span data-ttu-id="17cb4-137">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="17cb4-137">Relationship</span></span> | <span data-ttu-id="17cb4-138">型</span><span class="sxs-lookup"><span data-stu-id="17cb4-138">Type</span></span>   |<span data-ttu-id="17cb4-139">説明</span><span class="sxs-lookup"><span data-stu-id="17cb4-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="17cb4-140">format</span><span class="sxs-lookup"><span data-stu-id="17cb4-140">format</span></span>|[<span data-ttu-id="17cb4-141">ChartSeriesFormat</span><span class="sxs-lookup"><span data-stu-id="17cb4-141">ChartSeriesFormat</span></span>](chartseriesformat.md)|<span data-ttu-id="17cb4-p102">グラフ の系列の書式設定を表します。これには塗りつぶしと線の書式設定などがあります。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="17cb4-p102">Represents the formatting of a chart series, which includes fill and line formatting. Read-only.</span></span>|
|<span data-ttu-id="17cb4-144">points</span><span class="sxs-lookup"><span data-stu-id="17cb4-144">points</span></span>|<span data-ttu-id="17cb4-145">[ChartPoints](chartpoint.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="17cb4-145">[ChartPoints](chartpoint.md) collection</span></span>|<span data-ttu-id="17cb4-p103">データ系列にあるすべてのポイントのコレクションを返します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="17cb4-p103">Represents a collection of all points in the series. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="17cb4-148">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="17cb4-148">JSON representation</span></span>

<span data-ttu-id="17cb4-149">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="17cb4-149">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "ChartSeries resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->