---
title: ChartPoint リソースの種類
description: グラフの系列のポイントを表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: e8ede39ef53bfc39574ebfc86c8138a70fc31ad6
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573068"
---
# <a name="chartpoint-resource-type"></a><span data-ttu-id="58685-103">ChartPoint リソースの種類</span><span class="sxs-lookup"><span data-stu-id="58685-103">ChartPoint resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="58685-104">グラフの系列のポイントを表します。</span><span class="sxs-lookup"><span data-stu-id="58685-104">Represents a point of a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="58685-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="58685-105">Methods</span></span>

| <span data-ttu-id="58685-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="58685-106">Method</span></span>           | <span data-ttu-id="58685-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="58685-107">Return Type</span></span>    |<span data-ttu-id="58685-108">説明</span><span class="sxs-lookup"><span data-stu-id="58685-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="58685-109">Get ChartPoint</span><span class="sxs-lookup"><span data-stu-id="58685-109">Get ChartPoint</span></span>](../api/chartpoint-get.md) | [<span data-ttu-id="58685-110">workbookChartPoint</span><span class="sxs-lookup"><span data-stu-id="58685-110">workbookChartPoint</span></span>](chartpoint.md) |<span data-ttu-id="58685-111">chartPoint オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="58685-111">Read properties and relationships of chartPoint object.</span></span>|
|[<span data-ttu-id="58685-112">List</span><span class="sxs-lookup"><span data-stu-id="58685-112">List</span></span>](../api/chartpoint-list.md) | <span data-ttu-id="58685-113">[workbookChartPoint](chartpoint.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="58685-113">[workbookChartPoint](chartpoint.md) collection</span></span> |<span data-ttu-id="58685-114">chartPoint オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="58685-114">Get chartPoint object collection.</span></span> |
|[<span data-ttu-id="58685-115">ItemAt</span><span class="sxs-lookup"><span data-stu-id="58685-115">ItemAt</span></span>](../api/chartpointscollection-itemat.md)|[<span data-ttu-id="58685-116">workbookChartPoint</span><span class="sxs-lookup"><span data-stu-id="58685-116">workbookChartPoint</span></span>](chartpoint.md)|<span data-ttu-id="58685-117">データ系列内の位置に基づくポイントを取得します。</span><span class="sxs-lookup"><span data-stu-id="58685-117">Retrieve a point based on its position within the series.</span></span>|

## <a name="properties"></a><span data-ttu-id="58685-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="58685-118">Properties</span></span>
| <span data-ttu-id="58685-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="58685-119">Property</span></span>     | <span data-ttu-id="58685-120">型</span><span class="sxs-lookup"><span data-stu-id="58685-120">Type</span></span>   |<span data-ttu-id="58685-121">説明</span><span class="sxs-lookup"><span data-stu-id="58685-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="58685-122">value</span><span class="sxs-lookup"><span data-stu-id="58685-122">value</span></span>|<span data-ttu-id="58685-123">Json</span><span class="sxs-lookup"><span data-stu-id="58685-123">Json</span></span>|<span data-ttu-id="58685-p101">グラフのポイントの値を返します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="58685-p101">Returns the value of a chart point. Read-only.</span></span>|
|<span data-ttu-id="58685-126">id</span><span class="sxs-lookup"><span data-stu-id="58685-126">id</span></span>|<span data-ttu-id="58685-127">文字列</span><span class="sxs-lookup"><span data-stu-id="58685-127">string</span></span>|<span data-ttu-id="58685-128">一意識別子</span><span class="sxs-lookup"><span data-stu-id="58685-128">unique identifier</span></span>|

## <a name="relationships"></a><span data-ttu-id="58685-129">関係</span><span class="sxs-lookup"><span data-stu-id="58685-129">Relationships</span></span>
| <span data-ttu-id="58685-130">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="58685-130">Relationship</span></span> | <span data-ttu-id="58685-131">型</span><span class="sxs-lookup"><span data-stu-id="58685-131">Type</span></span>   |<span data-ttu-id="58685-132">説明</span><span class="sxs-lookup"><span data-stu-id="58685-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="58685-133">format</span><span class="sxs-lookup"><span data-stu-id="58685-133">format</span></span>|[<span data-ttu-id="58685-134">workbookChartPointFormat</span><span class="sxs-lookup"><span data-stu-id="58685-134">workbookChartPointFormat</span></span>](chartpointformat.md)|<span data-ttu-id="58685-p102">グラフのポイントの書式設定プロパティをカプセル化します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="58685-p102">Encapsulates the format properties chart point. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="58685-137">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="58685-137">JSON representation</span></span>

<span data-ttu-id="58685-138">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="58685-138">Here is a JSON representation of the resource.</span></span>

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
