---
title: ChartGridlines リソースの種類
description: グラフの軸の目盛線または補助目盛線を表します。
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 7747564b2f72287ef6ec2c6cc1f912695f58218e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27807827"
---
# <a name="chartgridlines-resource-type"></a><span data-ttu-id="c796d-103">ChartGridlines リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c796d-103">ChartGridlines resource type</span></span>

> <span data-ttu-id="c796d-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c796d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c796d-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c796d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c796d-106">グラフの軸の目盛線または補助目盛線を表します。</span><span class="sxs-lookup"><span data-stu-id="c796d-106">Represents major or minor gridlines on a chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="c796d-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="c796d-107">Methods</span></span>

| <span data-ttu-id="c796d-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="c796d-108">Method</span></span>           | <span data-ttu-id="c796d-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="c796d-109">Return Type</span></span>    |<span data-ttu-id="c796d-110">説明</span><span class="sxs-lookup"><span data-stu-id="c796d-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c796d-111">Get ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="c796d-111">Get ChartGridlines</span></span>](../api/chartgridlines-get.md) | [<span data-ttu-id="c796d-112">ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="c796d-112">ChartGridlines</span></span>](chartgridlines.md) |<span data-ttu-id="c796d-113">chartGridlines オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="c796d-113">Read properties and relationships of chartGridlines object.</span></span>|
|[<span data-ttu-id="c796d-114">Update</span><span class="sxs-lookup"><span data-stu-id="c796d-114">Update</span></span>](../api/chartgridlines-update.md) | [<span data-ttu-id="c796d-115">ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="c796d-115">ChartGridlines</span></span>](chartgridlines.md)    |<span data-ttu-id="c796d-116">ChartGridlines オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="c796d-116">Update ChartGridlines object.</span></span> |

## <a name="properties"></a><span data-ttu-id="c796d-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c796d-117">Properties</span></span>
| <span data-ttu-id="c796d-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c796d-118">Property</span></span>     | <span data-ttu-id="c796d-119">種類</span><span class="sxs-lookup"><span data-stu-id="c796d-119">Type</span></span>   |<span data-ttu-id="c796d-120">説明</span><span class="sxs-lookup"><span data-stu-id="c796d-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c796d-121">visible</span><span class="sxs-lookup"><span data-stu-id="c796d-121">visible</span></span>|<span data-ttu-id="c796d-122">ブール値</span><span class="sxs-lookup"><span data-stu-id="c796d-122">boolean</span></span>|<span data-ttu-id="c796d-123">軸の目盛線を表示するか非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="c796d-123">Boolean value representing if the axis gridlines are visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c796d-124">関係</span><span class="sxs-lookup"><span data-stu-id="c796d-124">Relationships</span></span>
| <span data-ttu-id="c796d-125">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c796d-125">Relationship</span></span> | <span data-ttu-id="c796d-126">型</span><span class="sxs-lookup"><span data-stu-id="c796d-126">Type</span></span>   |<span data-ttu-id="c796d-127">説明</span><span class="sxs-lookup"><span data-stu-id="c796d-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c796d-128">format</span><span class="sxs-lookup"><span data-stu-id="c796d-128">format</span></span>|[<span data-ttu-id="c796d-129">ChartGridlinesFormat</span><span class="sxs-lookup"><span data-stu-id="c796d-129">ChartGridlinesFormat</span></span>](chartgridlinesformat.md)|<span data-ttu-id="c796d-p102">グラフの目盛線の書式設定を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="c796d-p102">Represents the formatting of chart gridlines. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c796d-132">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c796d-132">JSON representation</span></span>

<span data-ttu-id="c796d-133">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c796d-133">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartGridLines"
}-->

```json
{
  "visible": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartGridlines resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
