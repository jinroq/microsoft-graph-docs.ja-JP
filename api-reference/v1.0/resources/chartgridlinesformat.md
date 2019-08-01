---
title: ChartGridlinesFormat リソースの種類
description: グラフの目盛線の書式設定プロパティをカプセル化します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: c34a9e640589a0df537d5f13652552551ac00372
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029779"
---
# <a name="chartgridlinesformat-resource-type"></a><span data-ttu-id="49bd2-103">ChartGridlinesFormat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="49bd2-103">ChartGridlinesFormat resource type</span></span>

<span data-ttu-id="49bd2-104">グラフの目盛線の書式設定プロパティをカプセル化します。</span><span class="sxs-lookup"><span data-stu-id="49bd2-104">Encapsulates the format properties for chart gridlines.</span></span>


## <a name="methods"></a><span data-ttu-id="49bd2-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="49bd2-105">Methods</span></span>
<span data-ttu-id="49bd2-106">None</span><span class="sxs-lookup"><span data-stu-id="49bd2-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="49bd2-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="49bd2-107">Properties</span></span>
<span data-ttu-id="49bd2-108">なし</span><span class="sxs-lookup"><span data-stu-id="49bd2-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="49bd2-109">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="49bd2-109">Relationships</span></span>
| <span data-ttu-id="49bd2-110">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="49bd2-110">Relationship</span></span> | <span data-ttu-id="49bd2-111">型</span><span class="sxs-lookup"><span data-stu-id="49bd2-111">Type</span></span>   |<span data-ttu-id="49bd2-112">説明</span><span class="sxs-lookup"><span data-stu-id="49bd2-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="49bd2-113">line</span><span class="sxs-lookup"><span data-stu-id="49bd2-113">line</span></span>|[<span data-ttu-id="49bd2-114">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="49bd2-114">WorkbookChartLineFormat</span></span>](chartlineformat.md)|<span data-ttu-id="49bd2-115">グラフの線の書式設定を表します。</span><span class="sxs-lookup"><span data-stu-id="49bd2-115">Represents chart line formatting.</span></span> <span data-ttu-id="49bd2-116">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="49bd2-116">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="49bd2-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="49bd2-117">JSON representation</span></span>

<span data-ttu-id="49bd2-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="49bd2-118">Here is a JSON representation of the resource.</span></span>

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
