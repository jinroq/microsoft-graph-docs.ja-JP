---
title: ChartLineFormat リソースの種類
description: 直線要素の書式設定オプションをカプセル化します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: b4409eb18dab41d43adc038b702a65fa8d63e4de
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640582"
---
# <a name="chartlineformat-resource-type"></a><span data-ttu-id="062ae-103">ChartLineFormat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="062ae-103">ChartLineFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="062ae-104">直線要素の書式設定オプションをカプセル化します。</span><span class="sxs-lookup"><span data-stu-id="062ae-104">Enapsulates the formatting options for line elements.</span></span>


## <a name="methods"></a><span data-ttu-id="062ae-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="062ae-105">Methods</span></span>

| <span data-ttu-id="062ae-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="062ae-106">Method</span></span>           | <span data-ttu-id="062ae-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="062ae-107">Return Type</span></span>    |<span data-ttu-id="062ae-108">説明</span><span class="sxs-lookup"><span data-stu-id="062ae-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="062ae-109">Get ChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="062ae-109">Get ChartLineFormat</span></span>](../api/chartlineformat-get.md) | [<span data-ttu-id="062ae-110">ChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="062ae-110">ChartLineFormat</span></span>](chartlineformat.md) |<span data-ttu-id="062ae-111">chartLineFormat オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="062ae-111">Read properties and relationships of chartLineFormat object.</span></span>|
|[<span data-ttu-id="062ae-112">更新する</span><span class="sxs-lookup"><span data-stu-id="062ae-112">Update</span></span>](../api/chartlineformat-update.md) | [<span data-ttu-id="062ae-113">ChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="062ae-113">ChartLineFormat</span></span>](chartlineformat.md) |<span data-ttu-id="062ae-114">ChartLineFormat オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="062ae-114">Update ChartLineFormat object.</span></span> |
|[<span data-ttu-id="062ae-115">Clear</span><span class="sxs-lookup"><span data-stu-id="062ae-115">Clear</span></span>](../api/chartlineformat-clear.md)|<span data-ttu-id="062ae-116">なし</span><span class="sxs-lookup"><span data-stu-id="062ae-116">None</span></span>|<span data-ttu-id="062ae-117">グラフ要素の線の書式をクリアします。</span><span class="sxs-lookup"><span data-stu-id="062ae-117">Clear the line format of a chart element.</span></span>|

## <a name="properties"></a><span data-ttu-id="062ae-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="062ae-118">Properties</span></span>
| <span data-ttu-id="062ae-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="062ae-119">Property</span></span>     | <span data-ttu-id="062ae-120">型</span><span class="sxs-lookup"><span data-stu-id="062ae-120">Type</span></span>   |<span data-ttu-id="062ae-121">説明</span><span class="sxs-lookup"><span data-stu-id="062ae-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="062ae-122">color</span><span class="sxs-lookup"><span data-stu-id="062ae-122">color</span></span>|<span data-ttu-id="062ae-123">文字列</span><span class="sxs-lookup"><span data-stu-id="062ae-123">string</span></span>|<span data-ttu-id="062ae-124">グラフの線の色を表す HTML カラー コード。</span><span class="sxs-lookup"><span data-stu-id="062ae-124">HTML color code representing the color of lines in the chart.</span></span>|

## <a name="relationships"></a><span data-ttu-id="062ae-125">関係</span><span class="sxs-lookup"><span data-stu-id="062ae-125">Relationships</span></span>
<span data-ttu-id="062ae-126">なし</span><span class="sxs-lookup"><span data-stu-id="062ae-126">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="062ae-127">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="062ae-127">JSON representation</span></span>

<span data-ttu-id="062ae-128">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="062ae-128">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartLineFormat"
}-->

```json
{
  "color": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartLineFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chartlineformat.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
