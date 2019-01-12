---
title: ChartGridlinesFormat リソースの種類
description: グラフの目盛線の書式設定プロパティをカプセル化します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: dd1e6d7f0a4ae9c17794035c8103cda8d189d5ca
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27959609"
---
# <a name="chartgridlinesformat-resource-type"></a><span data-ttu-id="24a86-103">ChartGridlinesFormat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="24a86-103">ChartGridlinesFormat resource type</span></span>

<span data-ttu-id="24a86-104">グラフの目盛線の書式設定プロパティをカプセル化します。</span><span class="sxs-lookup"><span data-stu-id="24a86-104">Encapsulates the format properties for chart gridlines.</span></span>


## <a name="methods"></a><span data-ttu-id="24a86-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="24a86-105">Methods</span></span>
<span data-ttu-id="24a86-106">なし</span><span class="sxs-lookup"><span data-stu-id="24a86-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="24a86-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="24a86-107">Properties</span></span>
<span data-ttu-id="24a86-108">なし</span><span class="sxs-lookup"><span data-stu-id="24a86-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="24a86-109">関係</span><span class="sxs-lookup"><span data-stu-id="24a86-109">Relationships</span></span>
| <span data-ttu-id="24a86-110">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="24a86-110">Relationship</span></span> | <span data-ttu-id="24a86-111">型</span><span class="sxs-lookup"><span data-stu-id="24a86-111">Type</span></span>   |<span data-ttu-id="24a86-112">説明</span><span class="sxs-lookup"><span data-stu-id="24a86-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="24a86-113">line</span><span class="sxs-lookup"><span data-stu-id="24a86-113">line</span></span>|[<span data-ttu-id="24a86-114">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="24a86-114">WorkbookChartLineFormat</span></span>](chartlineformat.md)|<span data-ttu-id="24a86-p101">グラフの線の書式設定を表します。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="24a86-p101">Represents chart line formatting. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="24a86-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="24a86-117">JSON representation</span></span>

<span data-ttu-id="24a86-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="24a86-118">Here is a JSON representation of the resource.</span></span>

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
