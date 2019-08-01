---
title: ChartGridlines リソースの種類
description: グラフの軸の目盛線または補助目盛線を表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: af1f9576c486174b6aa78dd3196c813e744a1552
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029800"
---
# <a name="chartgridlines-resource-type"></a><span data-ttu-id="49635-103">ChartGridlines リソースの種類</span><span class="sxs-lookup"><span data-stu-id="49635-103">ChartGridlines resource type</span></span>

<span data-ttu-id="49635-104">グラフの軸の目盛線または補助目盛線を表します。</span><span class="sxs-lookup"><span data-stu-id="49635-104">Represents major or minor gridlines on a chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="49635-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="49635-105">Methods</span></span>

| <span data-ttu-id="49635-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="49635-106">Method</span></span>           | <span data-ttu-id="49635-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="49635-107">Return Type</span></span>    |<span data-ttu-id="49635-108">説明</span><span class="sxs-lookup"><span data-stu-id="49635-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="49635-109">Get ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="49635-109">Get ChartGridlines</span></span>](../api/chartgridlines-get.md) | [<span data-ttu-id="49635-110">WorkbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="49635-110">WorkbookChartGridlines</span></span>](chartgridlines.md) |<span data-ttu-id="49635-111">chartGridlines オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="49635-111">Read properties and relationships of chartGridlines object.</span></span>|
|[<span data-ttu-id="49635-112">Update</span><span class="sxs-lookup"><span data-stu-id="49635-112">Update</span></span>](../api/chartgridlines-update.md) | [<span data-ttu-id="49635-113">WorkbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="49635-113">WorkbookChartGridlines</span></span>](chartgridlines.md)    |<span data-ttu-id="49635-114">ChartGridlines オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="49635-114">Update ChartGridlines object.</span></span> |

## <a name="properties"></a><span data-ttu-id="49635-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="49635-115">Properties</span></span>
| <span data-ttu-id="49635-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="49635-116">Property</span></span>     | <span data-ttu-id="49635-117">型</span><span class="sxs-lookup"><span data-stu-id="49635-117">Type</span></span>   |<span data-ttu-id="49635-118">説明</span><span class="sxs-lookup"><span data-stu-id="49635-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="49635-119">visible</span><span class="sxs-lookup"><span data-stu-id="49635-119">visible</span></span>|<span data-ttu-id="49635-120">ブール値</span><span class="sxs-lookup"><span data-stu-id="49635-120">boolean</span></span>|<span data-ttu-id="49635-121">軸の目盛線を表示するか非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="49635-121">Boolean value representing if the axis gridlines are visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="49635-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="49635-122">Relationships</span></span>
| <span data-ttu-id="49635-123">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="49635-123">Relationship</span></span> | <span data-ttu-id="49635-124">型</span><span class="sxs-lookup"><span data-stu-id="49635-124">Type</span></span>   |<span data-ttu-id="49635-125">説明</span><span class="sxs-lookup"><span data-stu-id="49635-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="49635-126">format</span><span class="sxs-lookup"><span data-stu-id="49635-126">format</span></span>|[<span data-ttu-id="49635-127">WorkbookChartGridlinesFormat</span><span class="sxs-lookup"><span data-stu-id="49635-127">WorkbookChartGridlinesFormat</span></span>](chartgridlinesformat.md)|<span data-ttu-id="49635-128">グラフの目盛線の書式設定を表します。</span><span class="sxs-lookup"><span data-stu-id="49635-128">Represents the formatting of chart gridlines.</span></span> <span data-ttu-id="49635-129">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="49635-129">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="49635-130">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="49635-130">JSON representation</span></span>

<span data-ttu-id="49635-131">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="49635-131">Here is a JSON representation of the resource.</span></span>

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
