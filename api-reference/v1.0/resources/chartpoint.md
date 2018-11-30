---
title: ChartPoint リソースの種類
description: グラフの系列のポイントを表します。
ms.openlocfilehash: 93c89bca61f27924621df0376bdf50e925e25c86
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023545"
---
# <a name="chartpoint-resource-type"></a><span data-ttu-id="8247f-103">ChartPoint リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8247f-103">ChartPoint resource type</span></span>

<span data-ttu-id="8247f-104">グラフの系列のポイントを表します。</span><span class="sxs-lookup"><span data-stu-id="8247f-104">Represents a point of a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="8247f-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="8247f-105">Methods</span></span>

| <span data-ttu-id="8247f-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="8247f-106">Method</span></span>           | <span data-ttu-id="8247f-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="8247f-107">Return Type</span></span>    |<span data-ttu-id="8247f-108">説明</span><span class="sxs-lookup"><span data-stu-id="8247f-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8247f-109">Get ChartPoint</span><span class="sxs-lookup"><span data-stu-id="8247f-109">Get ChartPoint</span></span>](../api/chartpoint-get.md) | [<span data-ttu-id="8247f-110">WorkbookChartPoint</span><span class="sxs-lookup"><span data-stu-id="8247f-110">WorkbookChartPoint</span></span>](chartpoint.md) |<span data-ttu-id="8247f-111">chartPoint オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="8247f-111">Read properties and relationships of chartPoint object.</span></span>|
|[<span data-ttu-id="8247f-112">List</span><span class="sxs-lookup"><span data-stu-id="8247f-112">List</span></span>](../api/chartpoint-list.md) | <span data-ttu-id="8247f-113">[WorkbookChartPoint](chartpoint.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="8247f-113">[WorkbookChartPoint](chartpoint.md) collection</span></span> |<span data-ttu-id="8247f-114">chartPoint オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="8247f-114">Get chartPoint object collection.</span></span> |
|[<span data-ttu-id="8247f-115">ItemAt</span><span class="sxs-lookup"><span data-stu-id="8247f-115">ItemAt</span></span>](../api/chartpointscollection-itemat.md)|[<span data-ttu-id="8247f-116">WorkbookChartPoint</span><span class="sxs-lookup"><span data-stu-id="8247f-116">WorkbookChartPoint</span></span>](chartpoint.md)|<span data-ttu-id="8247f-117">データ系列内の位置に基づくポイントを取得します。</span><span class="sxs-lookup"><span data-stu-id="8247f-117">Retrieve a point based on its position within the series.</span></span>|

## <a name="properties"></a><span data-ttu-id="8247f-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8247f-118">Properties</span></span>
| <span data-ttu-id="8247f-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8247f-119">Property</span></span>     | <span data-ttu-id="8247f-120">型</span><span class="sxs-lookup"><span data-stu-id="8247f-120">Type</span></span>   |<span data-ttu-id="8247f-121">説明</span><span class="sxs-lookup"><span data-stu-id="8247f-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8247f-122">value</span><span class="sxs-lookup"><span data-stu-id="8247f-122">value</span></span>|<span data-ttu-id="8247f-123">Json</span><span class="sxs-lookup"><span data-stu-id="8247f-123">Json</span></span>|<span data-ttu-id="8247f-p101">グラフのポイントの値を返します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="8247f-p101">Returns the value of a chart point. Read-only.</span></span>|
|<span data-ttu-id="8247f-126">ID</span><span class="sxs-lookup"><span data-stu-id="8247f-126">id</span></span>|<span data-ttu-id="8247f-127">文字列</span><span class="sxs-lookup"><span data-stu-id="8247f-127">string</span></span>|<span data-ttu-id="8247f-128">一意識別子</span><span class="sxs-lookup"><span data-stu-id="8247f-128">unique identifier</span></span>|

## <a name="relationships"></a><span data-ttu-id="8247f-129">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8247f-129">Relationships</span></span>
| <span data-ttu-id="8247f-130">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8247f-130">Relationship</span></span> | <span data-ttu-id="8247f-131">型</span><span class="sxs-lookup"><span data-stu-id="8247f-131">Type</span></span>   |<span data-ttu-id="8247f-132">説明</span><span class="sxs-lookup"><span data-stu-id="8247f-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8247f-133">format</span><span class="sxs-lookup"><span data-stu-id="8247f-133">format</span></span>|[<span data-ttu-id="8247f-134">WorkbookChartPointFormat</span><span class="sxs-lookup"><span data-stu-id="8247f-134">WorkbookChartPointFormat</span></span>](chartpointformat.md)|<span data-ttu-id="8247f-p102">グラフのポイントの書式設定プロパティをカプセル化します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="8247f-p102">Encapsulates the format properties chart point. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8247f-137">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8247f-137">JSON representation</span></span>

<span data-ttu-id="8247f-138">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8247f-138">Here is a JSON representation of the resource.</span></span>

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