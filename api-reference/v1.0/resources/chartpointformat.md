---
title: ChartPointFormat リソースの種類
description: グラフのポイントのオブジェクトの書式設定を表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 1c1b0a4a7d9076771da11061723f275079d429cb
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32569068"
---
# <a name="chartpointformat-resource-type"></a><span data-ttu-id="0d5c7-103">ChartPointFormat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0d5c7-103">ChartPointFormat resource type</span></span>

<span data-ttu-id="0d5c7-104">グラフのポイントのオブジェクトの書式設定を表します。</span><span class="sxs-lookup"><span data-stu-id="0d5c7-104">Represents formatting object for chart points.</span></span>


## <a name="methods"></a><span data-ttu-id="0d5c7-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="0d5c7-105">Methods</span></span>
<span data-ttu-id="0d5c7-106">なし</span><span class="sxs-lookup"><span data-stu-id="0d5c7-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="0d5c7-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0d5c7-107">Properties</span></span>
<span data-ttu-id="0d5c7-108">なし</span><span class="sxs-lookup"><span data-stu-id="0d5c7-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="0d5c7-109">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0d5c7-109">Relationships</span></span>
| <span data-ttu-id="0d5c7-110">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0d5c7-110">Relationship</span></span> | <span data-ttu-id="0d5c7-111">型</span><span class="sxs-lookup"><span data-stu-id="0d5c7-111">Type</span></span>   |<span data-ttu-id="0d5c7-112">説明</span><span class="sxs-lookup"><span data-stu-id="0d5c7-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0d5c7-113">fill</span><span class="sxs-lookup"><span data-stu-id="0d5c7-113">fill</span></span>|[<span data-ttu-id="0d5c7-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="0d5c7-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="0d5c7-115">背景の書式設定情報を含むグラフの塗りつぶしの書式を表します。</span><span class="sxs-lookup"><span data-stu-id="0d5c7-115">Represents the fill format of a chart, which includes background formating information.</span></span> <span data-ttu-id="0d5c7-116">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="0d5c7-116">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="0d5c7-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0d5c7-117">JSON representation</span></span>

<span data-ttu-id="0d5c7-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0d5c7-118">Here is a JSON representation of the resource.</span></span>

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
