---
title: ChartPoint リソースの種類
description: グラフの系列のポイントを表します。
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: f9bf959407a93c6d58d088833e5e3e437ef41125
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876252"
---
# <a name="chartpoint-resource-type"></a><span data-ttu-id="ad039-103">ChartPoint リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ad039-103">ChartPoint resource type</span></span>

> <span data-ttu-id="ad039-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ad039-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ad039-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ad039-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ad039-106">グラフの系列のポイントを表します。</span><span class="sxs-lookup"><span data-stu-id="ad039-106">Represents a point of a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="ad039-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="ad039-107">Methods</span></span>

| <span data-ttu-id="ad039-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="ad039-108">Method</span></span>           | <span data-ttu-id="ad039-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ad039-109">Return Type</span></span>    |<span data-ttu-id="ad039-110">説明</span><span class="sxs-lookup"><span data-stu-id="ad039-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ad039-111">Get ChartPoint</span><span class="sxs-lookup"><span data-stu-id="ad039-111">Get ChartPoint</span></span>](../api/chartpoint-get.md) | [<span data-ttu-id="ad039-112">ChartPoint</span><span class="sxs-lookup"><span data-stu-id="ad039-112">ChartPoint</span></span>](chartpoint.md) |<span data-ttu-id="ad039-113">chartPoint オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="ad039-113">Read properties and relationships of chartPoint object.</span></span>|
|[<span data-ttu-id="ad039-114">List</span><span class="sxs-lookup"><span data-stu-id="ad039-114">List</span></span>](../api/chartpoint-list.md) | <span data-ttu-id="ad039-115">[ChartPoint](chartpoint.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ad039-115">[ChartPoint](chartpoint.md) collection</span></span> |<span data-ttu-id="ad039-116">chartPoint オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="ad039-116">Get chartPoint object collection.</span></span> |
|[<span data-ttu-id="ad039-117">Itemat</span><span class="sxs-lookup"><span data-stu-id="ad039-117">Itemat</span></span>](../api/chartpointscollection-itemat.md)|[<span data-ttu-id="ad039-118">ChartPoint</span><span class="sxs-lookup"><span data-stu-id="ad039-118">ChartPoint</span></span>](chartpoint.md)|<span data-ttu-id="ad039-119">データ系列内の位置に基づくポイントを取得します。</span><span class="sxs-lookup"><span data-stu-id="ad039-119">Retrieve a point based on its position within the series.</span></span>|

## <a name="properties"></a><span data-ttu-id="ad039-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ad039-120">Properties</span></span>
| <span data-ttu-id="ad039-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ad039-121">Property</span></span>     | <span data-ttu-id="ad039-122">種類</span><span class="sxs-lookup"><span data-stu-id="ad039-122">Type</span></span>   |<span data-ttu-id="ad039-123">説明</span><span class="sxs-lookup"><span data-stu-id="ad039-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ad039-124">value</span><span class="sxs-lookup"><span data-stu-id="ad039-124">value</span></span>|<span data-ttu-id="ad039-125">object</span><span class="sxs-lookup"><span data-stu-id="ad039-125">object</span></span>|<span data-ttu-id="ad039-p102">グラフのポイントの値を返します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="ad039-p102">Returns the value of a chart point. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ad039-128">関係</span><span class="sxs-lookup"><span data-stu-id="ad039-128">Relationships</span></span>
| <span data-ttu-id="ad039-129">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ad039-129">Relationship</span></span> | <span data-ttu-id="ad039-130">型</span><span class="sxs-lookup"><span data-stu-id="ad039-130">Type</span></span>   |<span data-ttu-id="ad039-131">説明</span><span class="sxs-lookup"><span data-stu-id="ad039-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ad039-132">format</span><span class="sxs-lookup"><span data-stu-id="ad039-132">format</span></span>|[<span data-ttu-id="ad039-133">ChartPointFormat</span><span class="sxs-lookup"><span data-stu-id="ad039-133">ChartPointFormat</span></span>](chartpointformat.md)|<span data-ttu-id="ad039-p103">グラフのポイントの書式設定プロパティをカプセル化します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="ad039-p103">Encapsulates the format properties chart point. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ad039-136">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ad039-136">JSON representation</span></span>

<span data-ttu-id="ad039-137">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ad039-137">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "ChartPoint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
