---
title: ChartGridlines リソースの種類
description: グラフの軸の目盛線または補助目盛線を表します。
author: lumine2008
ms.openlocfilehash: 2aaf044b09d061af4853e76e0f2ba118bd1b2321
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27353033"
---
# <a name="chartgridlines-resource-type"></a><span data-ttu-id="e2dae-103">ChartGridlines リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e2dae-103">ChartGridlines resource type</span></span>

<span data-ttu-id="e2dae-104">グラフの軸の目盛線または補助目盛線を表します。</span><span class="sxs-lookup"><span data-stu-id="e2dae-104">Represents major or minor gridlines on a chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="e2dae-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="e2dae-105">Methods</span></span>

| <span data-ttu-id="e2dae-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="e2dae-106">Method</span></span>           | <span data-ttu-id="e2dae-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="e2dae-107">Return Type</span></span>    |<span data-ttu-id="e2dae-108">説明</span><span class="sxs-lookup"><span data-stu-id="e2dae-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e2dae-109">Get ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="e2dae-109">Get ChartGridlines</span></span>](../api/chartgridlines-get.md) | [<span data-ttu-id="e2dae-110">WorkbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="e2dae-110">WorkbookChartGridlines</span></span>](chartgridlines.md) |<span data-ttu-id="e2dae-111">chartGridlines オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="e2dae-111">Read properties and relationships of chartGridlines object.</span></span>|
|[<span data-ttu-id="e2dae-112">Update</span><span class="sxs-lookup"><span data-stu-id="e2dae-112">Update</span></span>](../api/chartgridlines-update.md) | [<span data-ttu-id="e2dae-113">WorkbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="e2dae-113">WorkbookChartGridlines</span></span>](chartgridlines.md)    |<span data-ttu-id="e2dae-114">ChartGridlines オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="e2dae-114">Update ChartGridlines object.</span></span> |

## <a name="properties"></a><span data-ttu-id="e2dae-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e2dae-115">Properties</span></span>
| <span data-ttu-id="e2dae-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e2dae-116">Property</span></span>     | <span data-ttu-id="e2dae-117">種類</span><span class="sxs-lookup"><span data-stu-id="e2dae-117">Type</span></span>   |<span data-ttu-id="e2dae-118">説明</span><span class="sxs-lookup"><span data-stu-id="e2dae-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e2dae-119">visible</span><span class="sxs-lookup"><span data-stu-id="e2dae-119">visible</span></span>|<span data-ttu-id="e2dae-120">ブール値</span><span class="sxs-lookup"><span data-stu-id="e2dae-120">boolean</span></span>|<span data-ttu-id="e2dae-121">軸の目盛線を表示するか非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="e2dae-121">Boolean value representing if the axis gridlines are visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e2dae-122">関係</span><span class="sxs-lookup"><span data-stu-id="e2dae-122">Relationships</span></span>
| <span data-ttu-id="e2dae-123">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e2dae-123">Relationship</span></span> | <span data-ttu-id="e2dae-124">型</span><span class="sxs-lookup"><span data-stu-id="e2dae-124">Type</span></span>   |<span data-ttu-id="e2dae-125">説明</span><span class="sxs-lookup"><span data-stu-id="e2dae-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e2dae-126">format</span><span class="sxs-lookup"><span data-stu-id="e2dae-126">format</span></span>|[<span data-ttu-id="e2dae-127">WorkbookChartGridlinesFormat</span><span class="sxs-lookup"><span data-stu-id="e2dae-127">WorkbookChartGridlinesFormat</span></span>](chartgridlinesformat.md)|<span data-ttu-id="e2dae-p101">グラフの目盛線の書式設定を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="e2dae-p101">Represents the formatting of chart gridlines. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e2dae-130">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e2dae-130">JSON representation</span></span>

<span data-ttu-id="e2dae-131">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e2dae-131">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookChartGridlines"
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