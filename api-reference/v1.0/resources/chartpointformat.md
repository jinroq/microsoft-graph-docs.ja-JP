---
title: ChartPointFormat リソースの種類
description: グラフのポイントの書式設定オブジェクトを表します。
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 5923252a9fce47eedc58751def301b6515560ddd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27883343"
---
# <a name="chartpointformat-resource-type"></a><span data-ttu-id="855a6-103">ChartPointFormat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="855a6-103">ChartPointFormat resource type</span></span>

<span data-ttu-id="855a6-104">グラフのポイントの書式設定オブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="855a6-104">Represents formatting object for chart points.</span></span>


## <a name="methods"></a><span data-ttu-id="855a6-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="855a6-105">Methods</span></span>
<span data-ttu-id="855a6-106">なし</span><span class="sxs-lookup"><span data-stu-id="855a6-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="855a6-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="855a6-107">Properties</span></span>
<span data-ttu-id="855a6-108">なし</span><span class="sxs-lookup"><span data-stu-id="855a6-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="855a6-109">関係</span><span class="sxs-lookup"><span data-stu-id="855a6-109">Relationships</span></span>
| <span data-ttu-id="855a6-110">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="855a6-110">Relationship</span></span> | <span data-ttu-id="855a6-111">型</span><span class="sxs-lookup"><span data-stu-id="855a6-111">Type</span></span>   |<span data-ttu-id="855a6-112">説明</span><span class="sxs-lookup"><span data-stu-id="855a6-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="855a6-113">fill</span><span class="sxs-lookup"><span data-stu-id="855a6-113">fill</span></span>|[<span data-ttu-id="855a6-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="855a6-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="855a6-p101">グラフの塗りつぶしの書式を表します。これには背景の書式設定情報などがあります。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="855a6-p101">Represents the fill format of a chart, which includes background formating information. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="855a6-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="855a6-117">JSON representation</span></span>

<span data-ttu-id="855a6-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="855a6-118">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
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
<!-- {
  "type": "#page.annotation",
  "description": "ChartPointFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
