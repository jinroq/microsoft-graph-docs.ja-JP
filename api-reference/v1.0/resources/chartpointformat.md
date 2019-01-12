---
title: ChartPointFormat リソースの種類
description: グラフのポイントの書式設定オブジェクトを表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 1c1b0a4a7d9076771da11061723f275079d429cb
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27976997"
---
# <a name="chartpointformat-resource-type"></a><span data-ttu-id="9d8b6-103">ChartPointFormat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9d8b6-103">ChartPointFormat resource type</span></span>

<span data-ttu-id="9d8b6-104">グラフのポイントの書式設定オブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="9d8b6-104">Represents formatting object for chart points.</span></span>


## <a name="methods"></a><span data-ttu-id="9d8b6-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="9d8b6-105">Methods</span></span>
<span data-ttu-id="9d8b6-106">なし</span><span class="sxs-lookup"><span data-stu-id="9d8b6-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="9d8b6-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9d8b6-107">Properties</span></span>
<span data-ttu-id="9d8b6-108">なし</span><span class="sxs-lookup"><span data-stu-id="9d8b6-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="9d8b6-109">関係</span><span class="sxs-lookup"><span data-stu-id="9d8b6-109">Relationships</span></span>
| <span data-ttu-id="9d8b6-110">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="9d8b6-110">Relationship</span></span> | <span data-ttu-id="9d8b6-111">型</span><span class="sxs-lookup"><span data-stu-id="9d8b6-111">Type</span></span>   |<span data-ttu-id="9d8b6-112">説明</span><span class="sxs-lookup"><span data-stu-id="9d8b6-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9d8b6-113">fill</span><span class="sxs-lookup"><span data-stu-id="9d8b6-113">fill</span></span>|[<span data-ttu-id="9d8b6-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="9d8b6-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="9d8b6-p101">グラフの塗りつぶしの書式を表します。これには背景の書式設定情報などがあります。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="9d8b6-p101">Represents the fill format of a chart, which includes background formating information. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="9d8b6-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9d8b6-117">JSON representation</span></span>

<span data-ttu-id="9d8b6-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="9d8b6-118">Here is a JSON representation of the resource.</span></span>

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
