---
title: ChartPoint リソースの種類
description: グラフの系列のポイントを表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 4fd50e2e0b0f289f719dd6636eab16544e6a80f5
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641968"
---
# <a name="chartpoint-resource-type"></a><span data-ttu-id="7a721-103">ChartPoint リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7a721-103">ChartPoint resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7a721-104">グラフの系列のポイントを表します。</span><span class="sxs-lookup"><span data-stu-id="7a721-104">Represents a point of a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="7a721-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="7a721-105">Methods</span></span>

| <span data-ttu-id="7a721-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="7a721-106">Method</span></span>           | <span data-ttu-id="7a721-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="7a721-107">Return Type</span></span>    |<span data-ttu-id="7a721-108">説明</span><span class="sxs-lookup"><span data-stu-id="7a721-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7a721-109">Get ChartPoint</span><span class="sxs-lookup"><span data-stu-id="7a721-109">Get ChartPoint</span></span>](../api/chartpoint-get.md) | [<span data-ttu-id="7a721-110">ChartPoint</span><span class="sxs-lookup"><span data-stu-id="7a721-110">ChartPoint</span></span>](chartpoint.md) |<span data-ttu-id="7a721-111">chartPoint オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="7a721-111">Read properties and relationships of chartPoint object.</span></span>|
|[<span data-ttu-id="7a721-112">List</span><span class="sxs-lookup"><span data-stu-id="7a721-112">List</span></span>](../api/chartpoint-list.md) | <span data-ttu-id="7a721-113">[ChartPoint](chartpoint.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="7a721-113">[ChartPoint](chartpoint.md) collection</span></span> |<span data-ttu-id="7a721-114">chartPoint オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="7a721-114">Get chartPoint object collection.</span></span> |
|[<span data-ttu-id="7a721-115">Itemat</span><span class="sxs-lookup"><span data-stu-id="7a721-115">Itemat</span></span>](../api/chartpointscollection-itemat.md)|[<span data-ttu-id="7a721-116">ChartPoint</span><span class="sxs-lookup"><span data-stu-id="7a721-116">ChartPoint</span></span>](chartpoint.md)|<span data-ttu-id="7a721-117">データ系列内の位置に基づくポイントを取得します。</span><span class="sxs-lookup"><span data-stu-id="7a721-117">Retrieve a point based on its position within the series.</span></span>|

## <a name="properties"></a><span data-ttu-id="7a721-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7a721-118">Properties</span></span>
| <span data-ttu-id="7a721-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7a721-119">Property</span></span>     | <span data-ttu-id="7a721-120">型</span><span class="sxs-lookup"><span data-stu-id="7a721-120">Type</span></span>   |<span data-ttu-id="7a721-121">説明</span><span class="sxs-lookup"><span data-stu-id="7a721-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7a721-122">value</span><span class="sxs-lookup"><span data-stu-id="7a721-122">value</span></span>|<span data-ttu-id="7a721-123">object</span><span class="sxs-lookup"><span data-stu-id="7a721-123">object</span></span>|<span data-ttu-id="7a721-p101">グラフのポイントの値を返します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="7a721-p101">Returns the value of a chart point. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7a721-126">関係</span><span class="sxs-lookup"><span data-stu-id="7a721-126">Relationships</span></span>
| <span data-ttu-id="7a721-127">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7a721-127">Relationship</span></span> | <span data-ttu-id="7a721-128">型</span><span class="sxs-lookup"><span data-stu-id="7a721-128">Type</span></span>   |<span data-ttu-id="7a721-129">説明</span><span class="sxs-lookup"><span data-stu-id="7a721-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7a721-130">format</span><span class="sxs-lookup"><span data-stu-id="7a721-130">format</span></span>|[<span data-ttu-id="7a721-131">ChartPointFormat</span><span class="sxs-lookup"><span data-stu-id="7a721-131">ChartPointFormat</span></span>](chartpointformat.md)|<span data-ttu-id="7a721-p102">グラフのポイントの書式設定プロパティをカプセル化します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="7a721-p102">Encapsulates the format properties chart point. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7a721-134">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7a721-134">JSON representation</span></span>

<span data-ttu-id="7a721-135">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7a721-135">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartPoint"
}-->

```json
{
  "value": "string"
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
  "suppressions": [
    "Error: /api-reference/beta/resources/chartpoint.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
