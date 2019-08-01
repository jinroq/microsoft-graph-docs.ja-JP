---
title: ChartPoint リソースの種類
description: グラフの系列のポイントを表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 5e0a9d9fe558f53fe87ae8e3a0a447a5bd93aa71
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032950"
---
# <a name="chartpoint-resource-type"></a><span data-ttu-id="fdb07-103">ChartPoint リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fdb07-103">ChartPoint resource type</span></span>

<span data-ttu-id="fdb07-104">グラフの系列のポイントを表します。</span><span class="sxs-lookup"><span data-stu-id="fdb07-104">Represents a point of a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="fdb07-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="fdb07-105">Methods</span></span>

| <span data-ttu-id="fdb07-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="fdb07-106">Method</span></span>           | <span data-ttu-id="fdb07-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="fdb07-107">Return Type</span></span>    |<span data-ttu-id="fdb07-108">説明</span><span class="sxs-lookup"><span data-stu-id="fdb07-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fdb07-109">Get ChartPoint</span><span class="sxs-lookup"><span data-stu-id="fdb07-109">Get ChartPoint</span></span>](../api/chartpoint-get.md) | [<span data-ttu-id="fdb07-110">WorkbookChartPoint</span><span class="sxs-lookup"><span data-stu-id="fdb07-110">WorkbookChartPoint</span></span>](chartpoint.md) |<span data-ttu-id="fdb07-111">chartPoint オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="fdb07-111">Read properties and relationships of chartPoint object.</span></span>|
|[<span data-ttu-id="fdb07-112">List</span><span class="sxs-lookup"><span data-stu-id="fdb07-112">List</span></span>](../api/chartpoint-list.md) | <span data-ttu-id="fdb07-113">[WorkbookChartPoint](chartpoint.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="fdb07-113">[WorkbookChartPoint](chartpoint.md) collection</span></span> |<span data-ttu-id="fdb07-114">chartPoint オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="fdb07-114">Get chartPoint object collection.</span></span> |
|[<span data-ttu-id="fdb07-115">ItemAt</span><span class="sxs-lookup"><span data-stu-id="fdb07-115">ItemAt</span></span>](../api/chartpointscollection-itemat.md)|[<span data-ttu-id="fdb07-116">WorkbookChartPoint</span><span class="sxs-lookup"><span data-stu-id="fdb07-116">WorkbookChartPoint</span></span>](chartpoint.md)|<span data-ttu-id="fdb07-117">データ系列内の位置に基づくポイントを取得します。</span><span class="sxs-lookup"><span data-stu-id="fdb07-117">Retrieve a point based on its position within the series.</span></span>|

## <a name="properties"></a><span data-ttu-id="fdb07-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fdb07-118">Properties</span></span>
| <span data-ttu-id="fdb07-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fdb07-119">Property</span></span>     | <span data-ttu-id="fdb07-120">型</span><span class="sxs-lookup"><span data-stu-id="fdb07-120">Type</span></span>   |<span data-ttu-id="fdb07-121">説明</span><span class="sxs-lookup"><span data-stu-id="fdb07-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fdb07-122">value</span><span class="sxs-lookup"><span data-stu-id="fdb07-122">value</span></span>|<span data-ttu-id="fdb07-123">Json</span><span class="sxs-lookup"><span data-stu-id="fdb07-123">Json</span></span>|<span data-ttu-id="fdb07-124">グラフのポイントの値を返します。</span><span class="sxs-lookup"><span data-stu-id="fdb07-124">Returns the value of a chart point.</span></span> <span data-ttu-id="fdb07-125">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="fdb07-125">Read-only.</span></span>|
|<span data-ttu-id="fdb07-126">id</span><span class="sxs-lookup"><span data-stu-id="fdb07-126">id</span></span>|<span data-ttu-id="fdb07-127">string</span><span class="sxs-lookup"><span data-stu-id="fdb07-127">string</span></span>|<span data-ttu-id="fdb07-128">一意識別子</span><span class="sxs-lookup"><span data-stu-id="fdb07-128">unique identifier</span></span>|

## <a name="relationships"></a><span data-ttu-id="fdb07-129">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="fdb07-129">Relationships</span></span>
| <span data-ttu-id="fdb07-130">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="fdb07-130">Relationship</span></span> | <span data-ttu-id="fdb07-131">型</span><span class="sxs-lookup"><span data-stu-id="fdb07-131">Type</span></span>   |<span data-ttu-id="fdb07-132">説明</span><span class="sxs-lookup"><span data-stu-id="fdb07-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fdb07-133">format</span><span class="sxs-lookup"><span data-stu-id="fdb07-133">format</span></span>|[<span data-ttu-id="fdb07-134">WorkbookChartPointFormat</span><span class="sxs-lookup"><span data-stu-id="fdb07-134">WorkbookChartPointFormat</span></span>](chartpointformat.md)|<span data-ttu-id="fdb07-135">グラフのポイントの書式設定プロパティをカプセル化します。</span><span class="sxs-lookup"><span data-stu-id="fdb07-135">Encapsulates the format properties chart point.</span></span> <span data-ttu-id="fdb07-136">値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="fdb07-136">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fdb07-137">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fdb07-137">JSON representation</span></span>

<span data-ttu-id="fdb07-138">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="fdb07-138">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartPoint"
}-->

```json
{
  "value": "string",
  "id": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartPoint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
