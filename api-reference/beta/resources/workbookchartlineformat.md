---
title: workbookChartLineFormat リソースの種類
description: 直線要素の書式設定オプションをカプセル化します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: fe36b0448d430566b51ee836e93d02f08cdbdbd5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007243"
---
# <a name="workbookchartlineformat-resource-type"></a><span data-ttu-id="ac0cd-103">workbookChartLineFormat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ac0cd-103">workbookChartLineFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ac0cd-104">直線要素の書式設定オプションをカプセル化します。</span><span class="sxs-lookup"><span data-stu-id="ac0cd-104">Enapsulates the formatting options for line elements.</span></span>


## <a name="methods"></a><span data-ttu-id="ac0cd-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="ac0cd-105">Methods</span></span>

| <span data-ttu-id="ac0cd-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="ac0cd-106">Method</span></span>           | <span data-ttu-id="ac0cd-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ac0cd-107">Return Type</span></span>    |<span data-ttu-id="ac0cd-108">説明</span><span class="sxs-lookup"><span data-stu-id="ac0cd-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ac0cd-109">WorkbookChartLineFormat を取得する</span><span class="sxs-lookup"><span data-stu-id="ac0cd-109">Get workbookChartLineFormat</span></span>](../api/chartlineformat-get.md) | [<span data-ttu-id="ac0cd-110">workbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="ac0cd-110">workbookChartLineFormat</span></span>](workbookchartlineformat.md) |<span data-ttu-id="ac0cd-111">chartLineFormat オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="ac0cd-111">Read properties and relationships of chartLineFormat object.</span></span>|
|[<span data-ttu-id="ac0cd-112">Update</span><span class="sxs-lookup"><span data-stu-id="ac0cd-112">Update</span></span>](../api/chartlineformat-update.md) | [<span data-ttu-id="ac0cd-113">workbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="ac0cd-113">workbookChartLineFormat</span></span>](workbookchartlineformat.md) |<span data-ttu-id="ac0cd-114">ChartLineFormat オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="ac0cd-114">Update ChartLineFormat object.</span></span> |
|[<span data-ttu-id="ac0cd-115">Clear</span><span class="sxs-lookup"><span data-stu-id="ac0cd-115">Clear</span></span>](../api/chartlineformat-clear.md)|<span data-ttu-id="ac0cd-116">なし</span><span class="sxs-lookup"><span data-stu-id="ac0cd-116">None</span></span>|<span data-ttu-id="ac0cd-117">グラフ要素の線の書式をクリアします。</span><span class="sxs-lookup"><span data-stu-id="ac0cd-117">Clear the line format of a chart element.</span></span>|

## <a name="properties"></a><span data-ttu-id="ac0cd-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ac0cd-118">Properties</span></span>
| <span data-ttu-id="ac0cd-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ac0cd-119">Property</span></span>     | <span data-ttu-id="ac0cd-120">型</span><span class="sxs-lookup"><span data-stu-id="ac0cd-120">Type</span></span>   |<span data-ttu-id="ac0cd-121">説明</span><span class="sxs-lookup"><span data-stu-id="ac0cd-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ac0cd-122">color</span><span class="sxs-lookup"><span data-stu-id="ac0cd-122">color</span></span>|<span data-ttu-id="ac0cd-123">string</span><span class="sxs-lookup"><span data-stu-id="ac0cd-123">string</span></span>|<span data-ttu-id="ac0cd-124">グラフの線の色を表す HTML カラー コード。</span><span class="sxs-lookup"><span data-stu-id="ac0cd-124">HTML color code representing the color of lines in the chart.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ac0cd-125">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ac0cd-125">Relationships</span></span>
<span data-ttu-id="ac0cd-126">なし</span><span class="sxs-lookup"><span data-stu-id="ac0cd-126">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="ac0cd-127">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ac0cd-127">JSON representation</span></span>

<span data-ttu-id="ac0cd-128">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ac0cd-128">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.workbookChartLineFormat"
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
  "description": "workbookChartLineFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
