---
title: workbookChartPoint リソースの種類
description: グラフの系列のポイントを表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: e12cc2f9a700ef66ec47a72aa88a2c30f2c2c3f6
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348907"
---
# <a name="workbookchartpoint-resource-type"></a><span data-ttu-id="c60ad-103">workbookChartPoint リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c60ad-103">workbookChartPoint resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c60ad-104">グラフの系列のポイントを表します。</span><span class="sxs-lookup"><span data-stu-id="c60ad-104">Represents a point of a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="c60ad-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="c60ad-105">Methods</span></span>

| <span data-ttu-id="c60ad-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="c60ad-106">Method</span></span>           | <span data-ttu-id="c60ad-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="c60ad-107">Return Type</span></span>    |<span data-ttu-id="c60ad-108">説明</span><span class="sxs-lookup"><span data-stu-id="c60ad-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c60ad-109">workbookChartPoint を取得する</span><span class="sxs-lookup"><span data-stu-id="c60ad-109">Get workbookChartPoint</span></span>](../api/chartpoint-get.md) | [<span data-ttu-id="c60ad-110">workbookChartPoint</span><span class="sxs-lookup"><span data-stu-id="c60ad-110">workbookChartPoint</span></span>](workbookchartpoint.md) |<span data-ttu-id="c60ad-111">chartPoint オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="c60ad-111">Read properties and relationships of chartPoint object.</span></span>|
|[<span data-ttu-id="c60ad-112">List</span><span class="sxs-lookup"><span data-stu-id="c60ad-112">List</span></span>](../api/chartpoint-list.md) | <span data-ttu-id="c60ad-113">[workbookChartPoint](workbookchartpoint.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="c60ad-113">[workbookChartPoint](workbookchartpoint.md) collection</span></span> |<span data-ttu-id="c60ad-114">chartPoint オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="c60ad-114">Get chartPoint object collection.</span></span> |
|[<span data-ttu-id="c60ad-115">ItemAt</span><span class="sxs-lookup"><span data-stu-id="c60ad-115">ItemAt</span></span>](../api/chartpointscollection-itemat.md)|[<span data-ttu-id="c60ad-116">workbookChartPoint</span><span class="sxs-lookup"><span data-stu-id="c60ad-116">workbookChartPoint</span></span>](workbookchartpoint.md)|<span data-ttu-id="c60ad-117">データ系列内の位置に基づくポイントを取得します。</span><span class="sxs-lookup"><span data-stu-id="c60ad-117">Retrieve a point based on its position within the series.</span></span>|

## <a name="properties"></a><span data-ttu-id="c60ad-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c60ad-118">Properties</span></span>
| <span data-ttu-id="c60ad-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c60ad-119">Property</span></span>     | <span data-ttu-id="c60ad-120">種類</span><span class="sxs-lookup"><span data-stu-id="c60ad-120">Type</span></span>   |<span data-ttu-id="c60ad-121">説明</span><span class="sxs-lookup"><span data-stu-id="c60ad-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c60ad-122">value</span><span class="sxs-lookup"><span data-stu-id="c60ad-122">value</span></span>|<span data-ttu-id="c60ad-123">Json</span><span class="sxs-lookup"><span data-stu-id="c60ad-123">Json</span></span>|<span data-ttu-id="c60ad-124">グラフのポイントの値を返します。</span><span class="sxs-lookup"><span data-stu-id="c60ad-124">Returns the value of a chart point.</span></span> <span data-ttu-id="c60ad-125">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="c60ad-125">Read-only.</span></span>|
|<span data-ttu-id="c60ad-126">id</span><span class="sxs-lookup"><span data-stu-id="c60ad-126">id</span></span>|<span data-ttu-id="c60ad-127">string</span><span class="sxs-lookup"><span data-stu-id="c60ad-127">string</span></span>|<span data-ttu-id="c60ad-128">一意識別子</span><span class="sxs-lookup"><span data-stu-id="c60ad-128">unique identifier</span></span>|

## <a name="relationships"></a><span data-ttu-id="c60ad-129">関係</span><span class="sxs-lookup"><span data-stu-id="c60ad-129">Relationships</span></span>
| <span data-ttu-id="c60ad-130">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c60ad-130">Relationship</span></span> | <span data-ttu-id="c60ad-131">型</span><span class="sxs-lookup"><span data-stu-id="c60ad-131">Type</span></span>   |<span data-ttu-id="c60ad-132">説明</span><span class="sxs-lookup"><span data-stu-id="c60ad-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c60ad-133">format</span><span class="sxs-lookup"><span data-stu-id="c60ad-133">format</span></span>|[<span data-ttu-id="c60ad-134">workbookChartPointFormat</span><span class="sxs-lookup"><span data-stu-id="c60ad-134">workbookChartPointFormat</span></span>](workbookchartpointformat.md)|<span data-ttu-id="c60ad-135">グラフのポイントの書式設定プロパティをカプセル化します。</span><span class="sxs-lookup"><span data-stu-id="c60ad-135">Encapsulates the format properties chart point.</span></span> <span data-ttu-id="c60ad-136">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="c60ad-136">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c60ad-137">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c60ad-137">JSON representation</span></span>

<span data-ttu-id="c60ad-138">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c60ad-138">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "format"
    ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartPoint"
}-->

```json
{
  "value": "string",
  "id": "string",
  "format": {"@odata.type": "microsoft.graph.workbookChartPointFormat"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartPoint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
