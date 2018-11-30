---
title: ChartGridlinesFormat リソースの種類
description: グラフの目盛線の書式設定プロパティをカプセル化します。
ms.openlocfilehash: 8286cd1a03188e9f6267b0e4731689c18b868083
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023207"
---
# <a name="chartgridlinesformat-resource-type"></a><span data-ttu-id="fc5be-103">ChartGridlinesFormat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fc5be-103">ChartGridlinesFormat resource type</span></span>

<span data-ttu-id="fc5be-104">グラフの目盛線の書式設定プロパティをカプセル化します。</span><span class="sxs-lookup"><span data-stu-id="fc5be-104">Encapsulates the format properties for chart gridlines.</span></span>


## <a name="methods"></a><span data-ttu-id="fc5be-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="fc5be-105">Methods</span></span>
<span data-ttu-id="fc5be-106">なし</span><span class="sxs-lookup"><span data-stu-id="fc5be-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="fc5be-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fc5be-107">Properties</span></span>
<span data-ttu-id="fc5be-108">なし</span><span class="sxs-lookup"><span data-stu-id="fc5be-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="fc5be-109">関係</span><span class="sxs-lookup"><span data-stu-id="fc5be-109">Relationships</span></span>
| <span data-ttu-id="fc5be-110">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="fc5be-110">Relationship</span></span> | <span data-ttu-id="fc5be-111">型</span><span class="sxs-lookup"><span data-stu-id="fc5be-111">Type</span></span>   |<span data-ttu-id="fc5be-112">説明</span><span class="sxs-lookup"><span data-stu-id="fc5be-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fc5be-113">line</span><span class="sxs-lookup"><span data-stu-id="fc5be-113">line</span></span>|[<span data-ttu-id="fc5be-114">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="fc5be-114">WorkbookChartLineFormat</span></span>](chartlineformat.md)|<span data-ttu-id="fc5be-p101">グラフの線の書式設定を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="fc5be-p101">Represents chart line formatting. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="fc5be-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fc5be-117">JSON representation</span></span>

<span data-ttu-id="fc5be-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="fc5be-118">Here is a JSON representation of the resource.</span></span>

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