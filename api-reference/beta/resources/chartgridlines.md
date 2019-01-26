---
title: ChartGridlines リソースの種類
description: グラフの軸の目盛線または補助目盛線を表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 3c57c68e7d9dfcd26741d15e302dd5dddeaae378
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572536"
---
# <a name="chartgridlines-resource-type"></a><span data-ttu-id="67e07-103">ChartGridlines リソースの種類</span><span class="sxs-lookup"><span data-stu-id="67e07-103">ChartGridlines resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="67e07-104">グラフの軸の目盛線または補助目盛線を表します。</span><span class="sxs-lookup"><span data-stu-id="67e07-104">Represents major or minor gridlines on a chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="67e07-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="67e07-105">Methods</span></span>

| <span data-ttu-id="67e07-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="67e07-106">Method</span></span>           | <span data-ttu-id="67e07-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="67e07-107">Return Type</span></span>    |<span data-ttu-id="67e07-108">説明</span><span class="sxs-lookup"><span data-stu-id="67e07-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="67e07-109">Get ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="67e07-109">Get ChartGridlines</span></span>](../api/chartgridlines-get.md) | [<span data-ttu-id="67e07-110">WorkbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="67e07-110">WorkbookChartGridlines</span></span>](chartgridlines.md) |<span data-ttu-id="67e07-111">chartGridlines オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="67e07-111">Read properties and relationships of chartGridlines object.</span></span>|
|[<span data-ttu-id="67e07-112">Update</span><span class="sxs-lookup"><span data-stu-id="67e07-112">Update</span></span>](../api/chartgridlines-update.md) | [<span data-ttu-id="67e07-113">WorkbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="67e07-113">WorkbookChartGridlines</span></span>](chartgridlines.md)    |<span data-ttu-id="67e07-114">ChartGridlines オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="67e07-114">Update ChartGridlines object.</span></span> |

## <a name="properties"></a><span data-ttu-id="67e07-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="67e07-115">Properties</span></span>
| <span data-ttu-id="67e07-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="67e07-116">Property</span></span>     | <span data-ttu-id="67e07-117">型</span><span class="sxs-lookup"><span data-stu-id="67e07-117">Type</span></span>   |<span data-ttu-id="67e07-118">説明</span><span class="sxs-lookup"><span data-stu-id="67e07-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="67e07-119">visible</span><span class="sxs-lookup"><span data-stu-id="67e07-119">visible</span></span>|<span data-ttu-id="67e07-120">boolean</span><span class="sxs-lookup"><span data-stu-id="67e07-120">boolean</span></span>|<span data-ttu-id="67e07-121">軸の目盛線を表示するか非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="67e07-121">Boolean value representing if the axis gridlines are visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="67e07-122">関係</span><span class="sxs-lookup"><span data-stu-id="67e07-122">Relationships</span></span>
| <span data-ttu-id="67e07-123">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="67e07-123">Relationship</span></span> | <span data-ttu-id="67e07-124">型</span><span class="sxs-lookup"><span data-stu-id="67e07-124">Type</span></span>   |<span data-ttu-id="67e07-125">説明</span><span class="sxs-lookup"><span data-stu-id="67e07-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="67e07-126">format</span><span class="sxs-lookup"><span data-stu-id="67e07-126">format</span></span>|[<span data-ttu-id="67e07-127">WorkbookChartGridlinesFormat</span><span class="sxs-lookup"><span data-stu-id="67e07-127">WorkbookChartGridlinesFormat</span></span>](chartgridlinesformat.md)|<span data-ttu-id="67e07-p101">グラフの目盛線の書式設定を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="67e07-p101">Represents the formatting of chart gridlines. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="67e07-130">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="67e07-130">JSON representation</span></span>

<span data-ttu-id="67e07-131">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="67e07-131">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "ChartGridlines resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chartgridlines.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
