---
title: ChartPoint リソースの種類
description: グラフの系列のポイントを表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 66c58e08063bd9757ad9c174e81f35328dd2722b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912758"
---
# <a name="chartpoint-resource-type"></a><span data-ttu-id="000cc-103">ChartPoint リソースの種類</span><span class="sxs-lookup"><span data-stu-id="000cc-103">ChartPoint resource type</span></span>

> <span data-ttu-id="000cc-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="000cc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="000cc-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="000cc-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="000cc-106">グラフの系列のポイントを表します。</span><span class="sxs-lookup"><span data-stu-id="000cc-106">Represents a point of a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="000cc-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="000cc-107">Methods</span></span>

| <span data-ttu-id="000cc-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="000cc-108">Method</span></span>           | <span data-ttu-id="000cc-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="000cc-109">Return Type</span></span>    |<span data-ttu-id="000cc-110">説明</span><span class="sxs-lookup"><span data-stu-id="000cc-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="000cc-111">Get ChartPoint</span><span class="sxs-lookup"><span data-stu-id="000cc-111">Get ChartPoint</span></span>](../api/chartpoint-get.md) | [<span data-ttu-id="000cc-112">ChartPoint</span><span class="sxs-lookup"><span data-stu-id="000cc-112">ChartPoint</span></span>](chartpoint.md) |<span data-ttu-id="000cc-113">chartPoint オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="000cc-113">Read properties and relationships of chartPoint object.</span></span>|
|[<span data-ttu-id="000cc-114">List</span><span class="sxs-lookup"><span data-stu-id="000cc-114">List</span></span>](../api/chartpoint-list.md) | <span data-ttu-id="000cc-115">[ChartPoint](chartpoint.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="000cc-115">[ChartPoint](chartpoint.md) collection</span></span> |<span data-ttu-id="000cc-116">chartPoint オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="000cc-116">Get chartPoint object collection.</span></span> |
|[<span data-ttu-id="000cc-117">Itemat</span><span class="sxs-lookup"><span data-stu-id="000cc-117">Itemat</span></span>](../api/chartpointscollection-itemat.md)|[<span data-ttu-id="000cc-118">ChartPoint</span><span class="sxs-lookup"><span data-stu-id="000cc-118">ChartPoint</span></span>](chartpoint.md)|<span data-ttu-id="000cc-119">データ系列内の位置に基づくポイントを取得します。</span><span class="sxs-lookup"><span data-stu-id="000cc-119">Retrieve a point based on its position within the series.</span></span>|

## <a name="properties"></a><span data-ttu-id="000cc-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="000cc-120">Properties</span></span>
| <span data-ttu-id="000cc-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="000cc-121">Property</span></span>     | <span data-ttu-id="000cc-122">種類</span><span class="sxs-lookup"><span data-stu-id="000cc-122">Type</span></span>   |<span data-ttu-id="000cc-123">説明</span><span class="sxs-lookup"><span data-stu-id="000cc-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="000cc-124">value</span><span class="sxs-lookup"><span data-stu-id="000cc-124">value</span></span>|<span data-ttu-id="000cc-125">object</span><span class="sxs-lookup"><span data-stu-id="000cc-125">object</span></span>|<span data-ttu-id="000cc-p102">グラフのポイントの値を返します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="000cc-p102">Returns the value of a chart point. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="000cc-128">関係</span><span class="sxs-lookup"><span data-stu-id="000cc-128">Relationships</span></span>
| <span data-ttu-id="000cc-129">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="000cc-129">Relationship</span></span> | <span data-ttu-id="000cc-130">型</span><span class="sxs-lookup"><span data-stu-id="000cc-130">Type</span></span>   |<span data-ttu-id="000cc-131">説明</span><span class="sxs-lookup"><span data-stu-id="000cc-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="000cc-132">format</span><span class="sxs-lookup"><span data-stu-id="000cc-132">format</span></span>|[<span data-ttu-id="000cc-133">ChartPointFormat</span><span class="sxs-lookup"><span data-stu-id="000cc-133">ChartPointFormat</span></span>](chartpointformat.md)|<span data-ttu-id="000cc-p103">グラフのポイントの書式設定プロパティをカプセル化します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="000cc-p103">Encapsulates the format properties chart point. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="000cc-136">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="000cc-136">JSON representation</span></span>

<span data-ttu-id="000cc-137">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="000cc-137">Here is a JSON representation of the resource.</span></span>

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
