---
title: ChartGridlines リソースの種類
description: グラフの軸の目盛線または補助目盛線を表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 044af64a6b6d41d9d5407678d1bd1e49cbdffe8a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27928151"
---
# <a name="chartgridlines-resource-type"></a><span data-ttu-id="06e46-103">ChartGridlines リソースの種類</span><span class="sxs-lookup"><span data-stu-id="06e46-103">ChartGridlines resource type</span></span>

> <span data-ttu-id="06e46-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="06e46-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="06e46-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="06e46-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="06e46-106">グラフの軸の目盛線または補助目盛線を表します。</span><span class="sxs-lookup"><span data-stu-id="06e46-106">Represents major or minor gridlines on a chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="06e46-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="06e46-107">Methods</span></span>

| <span data-ttu-id="06e46-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="06e46-108">Method</span></span>           | <span data-ttu-id="06e46-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="06e46-109">Return Type</span></span>    |<span data-ttu-id="06e46-110">説明</span><span class="sxs-lookup"><span data-stu-id="06e46-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="06e46-111">Get ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="06e46-111">Get ChartGridlines</span></span>](../api/chartgridlines-get.md) | [<span data-ttu-id="06e46-112">ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="06e46-112">ChartGridlines</span></span>](chartgridlines.md) |<span data-ttu-id="06e46-113">chartGridlines オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="06e46-113">Read properties and relationships of chartGridlines object.</span></span>|
|[<span data-ttu-id="06e46-114">Update</span><span class="sxs-lookup"><span data-stu-id="06e46-114">Update</span></span>](../api/chartgridlines-update.md) | [<span data-ttu-id="06e46-115">ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="06e46-115">ChartGridlines</span></span>](chartgridlines.md)    |<span data-ttu-id="06e46-116">ChartGridlines オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="06e46-116">Update ChartGridlines object.</span></span> |

## <a name="properties"></a><span data-ttu-id="06e46-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="06e46-117">Properties</span></span>
| <span data-ttu-id="06e46-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="06e46-118">Property</span></span>     | <span data-ttu-id="06e46-119">種類</span><span class="sxs-lookup"><span data-stu-id="06e46-119">Type</span></span>   |<span data-ttu-id="06e46-120">説明</span><span class="sxs-lookup"><span data-stu-id="06e46-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="06e46-121">visible</span><span class="sxs-lookup"><span data-stu-id="06e46-121">visible</span></span>|<span data-ttu-id="06e46-122">ブール値</span><span class="sxs-lookup"><span data-stu-id="06e46-122">boolean</span></span>|<span data-ttu-id="06e46-123">軸の目盛線を表示するか非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="06e46-123">Boolean value representing if the axis gridlines are visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="06e46-124">関係</span><span class="sxs-lookup"><span data-stu-id="06e46-124">Relationships</span></span>
| <span data-ttu-id="06e46-125">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="06e46-125">Relationship</span></span> | <span data-ttu-id="06e46-126">型</span><span class="sxs-lookup"><span data-stu-id="06e46-126">Type</span></span>   |<span data-ttu-id="06e46-127">説明</span><span class="sxs-lookup"><span data-stu-id="06e46-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="06e46-128">format</span><span class="sxs-lookup"><span data-stu-id="06e46-128">format</span></span>|[<span data-ttu-id="06e46-129">ChartGridlinesFormat</span><span class="sxs-lookup"><span data-stu-id="06e46-129">ChartGridlinesFormat</span></span>](chartgridlinesformat.md)|<span data-ttu-id="06e46-p102">グラフの目盛線の書式設定を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="06e46-p102">Represents the formatting of chart gridlines. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="06e46-132">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="06e46-132">JSON representation</span></span>

<span data-ttu-id="06e46-133">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="06e46-133">Here is a JSON representation of the resource.</span></span>

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
