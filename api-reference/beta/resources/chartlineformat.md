---
title: ChartLineFormat リソースの種類
description: 直線要素の書式設定オプションをカプセル化します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: b4409eb18dab41d43adc038b702a65fa8d63e4de
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543811"
---
# <a name="chartlineformat-resource-type"></a><span data-ttu-id="bccc7-103">ChartLineFormat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bccc7-103">ChartLineFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bccc7-104">直線要素の書式設定オプションをカプセル化します。</span><span class="sxs-lookup"><span data-stu-id="bccc7-104">Enapsulates the formatting options for line elements.</span></span>


## <a name="methods"></a><span data-ttu-id="bccc7-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="bccc7-105">Methods</span></span>

| <span data-ttu-id="bccc7-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="bccc7-106">Method</span></span>           | <span data-ttu-id="bccc7-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="bccc7-107">Return Type</span></span>    |<span data-ttu-id="bccc7-108">説明</span><span class="sxs-lookup"><span data-stu-id="bccc7-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bccc7-109">Get ChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="bccc7-109">Get ChartLineFormat</span></span>](../api/chartlineformat-get.md) | [<span data-ttu-id="bccc7-110">ChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="bccc7-110">ChartLineFormat</span></span>](chartlineformat.md) |<span data-ttu-id="bccc7-111">chartLineFormat オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="bccc7-111">Read properties and relationships of chartLineFormat object.</span></span>|
|[<span data-ttu-id="bccc7-112">Update</span><span class="sxs-lookup"><span data-stu-id="bccc7-112">Update</span></span>](../api/chartlineformat-update.md) | [<span data-ttu-id="bccc7-113">ChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="bccc7-113">ChartLineFormat</span></span>](chartlineformat.md) |<span data-ttu-id="bccc7-114">ChartLineFormat オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="bccc7-114">Update ChartLineFormat object.</span></span> |
|[<span data-ttu-id="bccc7-115">Clear</span><span class="sxs-lookup"><span data-stu-id="bccc7-115">Clear</span></span>](../api/chartlineformat-clear.md)|<span data-ttu-id="bccc7-116">なし</span><span class="sxs-lookup"><span data-stu-id="bccc7-116">None</span></span>|<span data-ttu-id="bccc7-117">グラフ要素の線の書式をクリアします。</span><span class="sxs-lookup"><span data-stu-id="bccc7-117">Clear the line format of a chart element.</span></span>|

## <a name="properties"></a><span data-ttu-id="bccc7-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bccc7-118">Properties</span></span>
| <span data-ttu-id="bccc7-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bccc7-119">Property</span></span>     | <span data-ttu-id="bccc7-120">型</span><span class="sxs-lookup"><span data-stu-id="bccc7-120">Type</span></span>   |<span data-ttu-id="bccc7-121">説明</span><span class="sxs-lookup"><span data-stu-id="bccc7-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bccc7-122">color</span><span class="sxs-lookup"><span data-stu-id="bccc7-122">color</span></span>|<span data-ttu-id="bccc7-123">string</span><span class="sxs-lookup"><span data-stu-id="bccc7-123">string</span></span>|<span data-ttu-id="bccc7-124">グラフの線の色を表す HTML カラー コード。</span><span class="sxs-lookup"><span data-stu-id="bccc7-124">HTML color code representing the color of lines in the chart.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bccc7-125">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="bccc7-125">Relationships</span></span>
<span data-ttu-id="bccc7-126">なし</span><span class="sxs-lookup"><span data-stu-id="bccc7-126">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="bccc7-127">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bccc7-127">JSON representation</span></span>

<span data-ttu-id="bccc7-128">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="bccc7-128">Here is a JSON representation of the resource.</span></span>

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
