---
title: ChartGridlinesFormat リソースの種類
description: グラフの目盛線の書式設定プロパティをカプセル化します。
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 8fde51cc220b20c533c3af122375047dd3276a9c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826461"
---
# <a name="chartgridlinesformat-resource-type"></a><span data-ttu-id="46bae-103">ChartGridlinesFormat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="46bae-103">ChartGridlinesFormat resource type</span></span>

<span data-ttu-id="46bae-104">グラフの目盛線の書式設定プロパティをカプセル化します。</span><span class="sxs-lookup"><span data-stu-id="46bae-104">Encapsulates the format properties for chart gridlines.</span></span>


## <a name="methods"></a><span data-ttu-id="46bae-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="46bae-105">Methods</span></span>
<span data-ttu-id="46bae-106">なし</span><span class="sxs-lookup"><span data-stu-id="46bae-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="46bae-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="46bae-107">Properties</span></span>
<span data-ttu-id="46bae-108">なし</span><span class="sxs-lookup"><span data-stu-id="46bae-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="46bae-109">関係</span><span class="sxs-lookup"><span data-stu-id="46bae-109">Relationships</span></span>
| <span data-ttu-id="46bae-110">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="46bae-110">Relationship</span></span> | <span data-ttu-id="46bae-111">型</span><span class="sxs-lookup"><span data-stu-id="46bae-111">Type</span></span>   |<span data-ttu-id="46bae-112">説明</span><span class="sxs-lookup"><span data-stu-id="46bae-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="46bae-113">line</span><span class="sxs-lookup"><span data-stu-id="46bae-113">line</span></span>|[<span data-ttu-id="46bae-114">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="46bae-114">WorkbookChartLineFormat</span></span>](chartlineformat.md)|<span data-ttu-id="46bae-p101">グラフの線の書式設定を表します。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="46bae-p101">Represents chart line formatting. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="46bae-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="46bae-117">JSON representation</span></span>

<span data-ttu-id="46bae-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="46bae-118">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartGridlinesFormat"
}-->

```json
{
  "line": {"@odata.type": "microsoft.graph.workbookChartLineFormat"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartGridlinesFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
