---
title: ChartPoint リソースの種類
description: グラフの系列のポイントを表します。
ms.openlocfilehash: 3d1bcc26fdc78bd7b844c870d40346a5f1f0496f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071184"
---
# <a name="chartpoint-resource-type"></a><span data-ttu-id="d592a-103">ChartPoint リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d592a-103">ChartPoint resource type</span></span>

> <span data-ttu-id="d592a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d592a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d592a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d592a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d592a-106">グラフの系列のポイントを表します。</span><span class="sxs-lookup"><span data-stu-id="d592a-106">Represents a point of a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="d592a-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="d592a-107">Methods</span></span>

| <span data-ttu-id="d592a-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="d592a-108">Method</span></span>           | <span data-ttu-id="d592a-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="d592a-109">Return Type</span></span>    |<span data-ttu-id="d592a-110">説明</span><span class="sxs-lookup"><span data-stu-id="d592a-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d592a-111">Get ChartPoint</span><span class="sxs-lookup"><span data-stu-id="d592a-111">Get ChartPoint</span></span>](../api/chartpoint-get.md) | [<span data-ttu-id="d592a-112">ChartPoint</span><span class="sxs-lookup"><span data-stu-id="d592a-112">ChartPoint</span></span>](chartpoint.md) |<span data-ttu-id="d592a-113">chartPoint オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="d592a-113">Read properties and relationships of chartPoint object.</span></span>|
|[<span data-ttu-id="d592a-114">List</span><span class="sxs-lookup"><span data-stu-id="d592a-114">List</span></span>](../api/chartpoint-list.md) | <span data-ttu-id="d592a-115">[ChartPoint](chartpoint.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="d592a-115">[ChartPoint](chartpoint.md) collection</span></span> |<span data-ttu-id="d592a-116">chartPoint オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="d592a-116">Get chartPoint object collection.</span></span> |
|[<span data-ttu-id="d592a-117">Itemat</span><span class="sxs-lookup"><span data-stu-id="d592a-117">Itemat</span></span>](../api/chartpointscollection-itemat.md)|[<span data-ttu-id="d592a-118">ChartPoint</span><span class="sxs-lookup"><span data-stu-id="d592a-118">ChartPoint</span></span>](chartpoint.md)|<span data-ttu-id="d592a-119">データ系列内の位置に基づくポイントを取得します。</span><span class="sxs-lookup"><span data-stu-id="d592a-119">Retrieve a point based on its position within the series.</span></span>|

## <a name="properties"></a><span data-ttu-id="d592a-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d592a-120">Properties</span></span>
| <span data-ttu-id="d592a-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d592a-121">Property</span></span>     | <span data-ttu-id="d592a-122">型</span><span class="sxs-lookup"><span data-stu-id="d592a-122">Type</span></span>   |<span data-ttu-id="d592a-123">説明</span><span class="sxs-lookup"><span data-stu-id="d592a-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d592a-124">value</span><span class="sxs-lookup"><span data-stu-id="d592a-124">value</span></span>|<span data-ttu-id="d592a-125">object</span><span class="sxs-lookup"><span data-stu-id="d592a-125">object</span></span>|<span data-ttu-id="d592a-p102">グラフのポイントの値を返します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="d592a-p102">Returns the value of a chart point. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d592a-128">関係</span><span class="sxs-lookup"><span data-stu-id="d592a-128">Relationships</span></span>
| <span data-ttu-id="d592a-129">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d592a-129">Relationship</span></span> | <span data-ttu-id="d592a-130">型</span><span class="sxs-lookup"><span data-stu-id="d592a-130">Type</span></span>   |<span data-ttu-id="d592a-131">説明</span><span class="sxs-lookup"><span data-stu-id="d592a-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d592a-132">format</span><span class="sxs-lookup"><span data-stu-id="d592a-132">format</span></span>|[<span data-ttu-id="d592a-133">ChartPointFormat</span><span class="sxs-lookup"><span data-stu-id="d592a-133">ChartPointFormat</span></span>](chartpointformat.md)|<span data-ttu-id="d592a-p103">グラフのポイントの書式設定プロパティをカプセル化します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="d592a-p103">Encapsulates the format properties chart point. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d592a-136">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d592a-136">JSON representation</span></span>

<span data-ttu-id="d592a-137">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d592a-137">Here is a JSON representation of the resource.</span></span>

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