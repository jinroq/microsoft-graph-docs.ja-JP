---
title: workbookChartPoint リソースの種類
description: グラフの系列のポイントを表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: db0037e91f1ee9279a131c5a318c4425e7878aed
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007257"
---
# <a name="workbookchartpoint-resource-type"></a><span data-ttu-id="aea08-103">workbookChartPoint リソースの種類</span><span class="sxs-lookup"><span data-stu-id="aea08-103">workbookChartPoint resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aea08-104">グラフの系列のポイントを表します。</span><span class="sxs-lookup"><span data-stu-id="aea08-104">Represents a point of a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="aea08-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="aea08-105">Methods</span></span>

| <span data-ttu-id="aea08-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="aea08-106">Method</span></span>           | <span data-ttu-id="aea08-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="aea08-107">Return Type</span></span>    |<span data-ttu-id="aea08-108">説明</span><span class="sxs-lookup"><span data-stu-id="aea08-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="aea08-109">WorkbookChartPoint を取得する</span><span class="sxs-lookup"><span data-stu-id="aea08-109">Get workbookChartPoint</span></span>](../api/chartpoint-get.md) | [<span data-ttu-id="aea08-110">workbookChartPoint</span><span class="sxs-lookup"><span data-stu-id="aea08-110">workbookChartPoint</span></span>](workbookchartpoint.md) |<span data-ttu-id="aea08-111">chartPoint オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="aea08-111">Read properties and relationships of chartPoint object.</span></span>|
|[<span data-ttu-id="aea08-112">List</span><span class="sxs-lookup"><span data-stu-id="aea08-112">List</span></span>](../api/chartpoint-list.md) | <span data-ttu-id="aea08-113">[workbookChartPoint](workbookchartpoint.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="aea08-113">[workbookChartPoint](workbookchartpoint.md) collection</span></span> |<span data-ttu-id="aea08-114">chartPoint オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="aea08-114">Get chartPoint object collection.</span></span> |
|[<span data-ttu-id="aea08-115">ItemAt</span><span class="sxs-lookup"><span data-stu-id="aea08-115">ItemAt</span></span>](../api/chartpointscollection-itemat.md)|[<span data-ttu-id="aea08-116">workbookChartPoint</span><span class="sxs-lookup"><span data-stu-id="aea08-116">workbookChartPoint</span></span>](workbookchartpoint.md)|<span data-ttu-id="aea08-117">データ系列内の位置に基づくポイントを取得します。</span><span class="sxs-lookup"><span data-stu-id="aea08-117">Retrieve a point based on its position within the series.</span></span>|

## <a name="properties"></a><span data-ttu-id="aea08-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aea08-118">Properties</span></span>
| <span data-ttu-id="aea08-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aea08-119">Property</span></span>     | <span data-ttu-id="aea08-120">型</span><span class="sxs-lookup"><span data-stu-id="aea08-120">Type</span></span>   |<span data-ttu-id="aea08-121">説明</span><span class="sxs-lookup"><span data-stu-id="aea08-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aea08-122">value</span><span class="sxs-lookup"><span data-stu-id="aea08-122">value</span></span>|<span data-ttu-id="aea08-123">Json</span><span class="sxs-lookup"><span data-stu-id="aea08-123">Json</span></span>|<span data-ttu-id="aea08-124">グラフのポイントの値を返します。</span><span class="sxs-lookup"><span data-stu-id="aea08-124">Returns the value of a chart point.</span></span> <span data-ttu-id="aea08-125">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="aea08-125">Read-only.</span></span>|
|<span data-ttu-id="aea08-126">id</span><span class="sxs-lookup"><span data-stu-id="aea08-126">id</span></span>|<span data-ttu-id="aea08-127">string</span><span class="sxs-lookup"><span data-stu-id="aea08-127">string</span></span>|<span data-ttu-id="aea08-128">一意識別子</span><span class="sxs-lookup"><span data-stu-id="aea08-128">unique identifier</span></span>|

## <a name="relationships"></a><span data-ttu-id="aea08-129">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="aea08-129">Relationships</span></span>
| <span data-ttu-id="aea08-130">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="aea08-130">Relationship</span></span> | <span data-ttu-id="aea08-131">型</span><span class="sxs-lookup"><span data-stu-id="aea08-131">Type</span></span>   |<span data-ttu-id="aea08-132">説明</span><span class="sxs-lookup"><span data-stu-id="aea08-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aea08-133">format</span><span class="sxs-lookup"><span data-stu-id="aea08-133">format</span></span>|[<span data-ttu-id="aea08-134">workbookChartPointFormat</span><span class="sxs-lookup"><span data-stu-id="aea08-134">workbookChartPointFormat</span></span>](workbookchartpointformat.md)|<span data-ttu-id="aea08-135">グラフのポイントの書式設定プロパティをカプセル化します。</span><span class="sxs-lookup"><span data-stu-id="aea08-135">Encapsulates the format properties chart point.</span></span> <span data-ttu-id="aea08-136">値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="aea08-136">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="aea08-137">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="aea08-137">JSON representation</span></span>

<span data-ttu-id="aea08-138">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="aea08-138">Here is a JSON representation of the resource.</span></span>

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
