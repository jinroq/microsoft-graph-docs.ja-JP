---
title: ChartPoint リソースの種類
description: グラフの系列のポイントを表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 3318415094a36100851b1c604cba2507de31f558
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962507"
---
# <a name="chartpoint-resource-type"></a><span data-ttu-id="18fe6-103">ChartPoint リソースの種類</span><span class="sxs-lookup"><span data-stu-id="18fe6-103">ChartPoint resource type</span></span>

<span data-ttu-id="18fe6-104">グラフの系列のポイントを表します。</span><span class="sxs-lookup"><span data-stu-id="18fe6-104">Represents a point of a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="18fe6-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="18fe6-105">Methods</span></span>

| <span data-ttu-id="18fe6-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="18fe6-106">Method</span></span>           | <span data-ttu-id="18fe6-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="18fe6-107">Return Type</span></span>    |<span data-ttu-id="18fe6-108">説明</span><span class="sxs-lookup"><span data-stu-id="18fe6-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="18fe6-109">Get ChartPoint</span><span class="sxs-lookup"><span data-stu-id="18fe6-109">Get ChartPoint</span></span>](../api/chartpoint-get.md) | [<span data-ttu-id="18fe6-110">WorkbookChartPoint</span><span class="sxs-lookup"><span data-stu-id="18fe6-110">WorkbookChartPoint</span></span>](chartpoint.md) |<span data-ttu-id="18fe6-111">chartPoint オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="18fe6-111">Read properties and relationships of chartPoint object.</span></span>|
|[<span data-ttu-id="18fe6-112">List</span><span class="sxs-lookup"><span data-stu-id="18fe6-112">List</span></span>](../api/chartpoint-list.md) | <span data-ttu-id="18fe6-113">[WorkbookChartPoint](chartpoint.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="18fe6-113">[WorkbookChartPoint](chartpoint.md) collection</span></span> |<span data-ttu-id="18fe6-114">chartPoint オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="18fe6-114">Get chartPoint object collection.</span></span> |
|[<span data-ttu-id="18fe6-115">ItemAt</span><span class="sxs-lookup"><span data-stu-id="18fe6-115">ItemAt</span></span>](../api/chartpointscollection-itemat.md)|[<span data-ttu-id="18fe6-116">WorkbookChartPoint</span><span class="sxs-lookup"><span data-stu-id="18fe6-116">WorkbookChartPoint</span></span>](chartpoint.md)|<span data-ttu-id="18fe6-117">データ系列内の位置に基づくポイントを取得します。</span><span class="sxs-lookup"><span data-stu-id="18fe6-117">Retrieve a point based on its position within the series.</span></span>|

## <a name="properties"></a><span data-ttu-id="18fe6-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="18fe6-118">Properties</span></span>
| <span data-ttu-id="18fe6-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="18fe6-119">Property</span></span>     | <span data-ttu-id="18fe6-120">種類</span><span class="sxs-lookup"><span data-stu-id="18fe6-120">Type</span></span>   |<span data-ttu-id="18fe6-121">説明</span><span class="sxs-lookup"><span data-stu-id="18fe6-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="18fe6-122">value</span><span class="sxs-lookup"><span data-stu-id="18fe6-122">value</span></span>|<span data-ttu-id="18fe6-123">Json</span><span class="sxs-lookup"><span data-stu-id="18fe6-123">Json</span></span>|<span data-ttu-id="18fe6-p101">グラフのポイントの値を返します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="18fe6-p101">Returns the value of a chart point. Read-only.</span></span>|
|<span data-ttu-id="18fe6-126">ID</span><span class="sxs-lookup"><span data-stu-id="18fe6-126">id</span></span>|<span data-ttu-id="18fe6-127">文字列</span><span class="sxs-lookup"><span data-stu-id="18fe6-127">string</span></span>|<span data-ttu-id="18fe6-128">一意識別子</span><span class="sxs-lookup"><span data-stu-id="18fe6-128">unique identifier</span></span>|

## <a name="relationships"></a><span data-ttu-id="18fe6-129">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="18fe6-129">Relationships</span></span>
| <span data-ttu-id="18fe6-130">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="18fe6-130">Relationship</span></span> | <span data-ttu-id="18fe6-131">型</span><span class="sxs-lookup"><span data-stu-id="18fe6-131">Type</span></span>   |<span data-ttu-id="18fe6-132">説明</span><span class="sxs-lookup"><span data-stu-id="18fe6-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="18fe6-133">format</span><span class="sxs-lookup"><span data-stu-id="18fe6-133">format</span></span>|[<span data-ttu-id="18fe6-134">WorkbookChartPointFormat</span><span class="sxs-lookup"><span data-stu-id="18fe6-134">WorkbookChartPointFormat</span></span>](chartpointformat.md)|<span data-ttu-id="18fe6-p102">グラフのポイントの書式設定プロパティをカプセル化します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="18fe6-p102">Encapsulates the format properties chart point. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="18fe6-137">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="18fe6-137">JSON representation</span></span>

<span data-ttu-id="18fe6-138">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="18fe6-138">Here is a JSON representation of the resource.</span></span>

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
