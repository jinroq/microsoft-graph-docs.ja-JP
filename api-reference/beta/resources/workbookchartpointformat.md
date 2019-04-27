---
title: workbookChartPointFormat リソースの種類
description: グラフのポイントのオブジェクトの書式設定を表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: f0896001fda140ff1d2693b3463c472568f1d28e
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348884"
---
# <a name="workbookchartpointformat-resource-type"></a><span data-ttu-id="dc49f-103">workbookChartPointFormat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="dc49f-103">workbookChartPointFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dc49f-104">グラフのポイントのオブジェクトの書式設定を表します。</span><span class="sxs-lookup"><span data-stu-id="dc49f-104">Represents formatting object for chart points.</span></span>


## <a name="methods"></a><span data-ttu-id="dc49f-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="dc49f-105">Methods</span></span>
<span data-ttu-id="dc49f-106">なし</span><span class="sxs-lookup"><span data-stu-id="dc49f-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="dc49f-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dc49f-107">Properties</span></span>
<span data-ttu-id="dc49f-108">なし</span><span class="sxs-lookup"><span data-stu-id="dc49f-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="dc49f-109">関係</span><span class="sxs-lookup"><span data-stu-id="dc49f-109">Relationships</span></span>
| <span data-ttu-id="dc49f-110">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="dc49f-110">Relationship</span></span> | <span data-ttu-id="dc49f-111">型</span><span class="sxs-lookup"><span data-stu-id="dc49f-111">Type</span></span>   |<span data-ttu-id="dc49f-112">説明</span><span class="sxs-lookup"><span data-stu-id="dc49f-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dc49f-113">fill</span><span class="sxs-lookup"><span data-stu-id="dc49f-113">fill</span></span>|[<span data-ttu-id="dc49f-114">workbookChartFill</span><span class="sxs-lookup"><span data-stu-id="dc49f-114">workbookChartFill</span></span>](workbookchartfill.md)|<span data-ttu-id="dc49f-115">背景の書式設定情報を含むグラフの塗りつぶしの書式を表します。</span><span class="sxs-lookup"><span data-stu-id="dc49f-115">Represents the fill format of a chart, which includes background formating information.</span></span> <span data-ttu-id="dc49f-116">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="dc49f-116">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="dc49f-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="dc49f-117">JSON representation</span></span>

<span data-ttu-id="dc49f-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="dc49f-118">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "fill"
    ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartPointFormat"
}-->

```json
{
  "fill": {"@odata.type": "microsoft.graph.workbookChartFill"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartPointFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
