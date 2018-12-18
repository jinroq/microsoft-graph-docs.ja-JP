---
title: ChartGridlinesFormat リソースの種類
description: グラフの目盛線の書式設定プロパティをカプセル化します。
author: lumine2008
ms.openlocfilehash: 61e75f644e70174bad04d5ae37b15cd07bc4d4bb
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27328960"
---
# <a name="chartgridlinesformat-resource-type"></a><span data-ttu-id="8de1b-103">ChartGridlinesFormat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8de1b-103">ChartGridlinesFormat resource type</span></span>

<span data-ttu-id="8de1b-104">グラフの目盛線の書式設定プロパティをカプセル化します。</span><span class="sxs-lookup"><span data-stu-id="8de1b-104">Encapsulates the format properties for chart gridlines.</span></span>


## <a name="methods"></a><span data-ttu-id="8de1b-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="8de1b-105">Methods</span></span>
<span data-ttu-id="8de1b-106">なし</span><span class="sxs-lookup"><span data-stu-id="8de1b-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="8de1b-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8de1b-107">Properties</span></span>
<span data-ttu-id="8de1b-108">なし</span><span class="sxs-lookup"><span data-stu-id="8de1b-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="8de1b-109">関係</span><span class="sxs-lookup"><span data-stu-id="8de1b-109">Relationships</span></span>
| <span data-ttu-id="8de1b-110">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8de1b-110">Relationship</span></span> | <span data-ttu-id="8de1b-111">型</span><span class="sxs-lookup"><span data-stu-id="8de1b-111">Type</span></span>   |<span data-ttu-id="8de1b-112">説明</span><span class="sxs-lookup"><span data-stu-id="8de1b-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8de1b-113">line</span><span class="sxs-lookup"><span data-stu-id="8de1b-113">line</span></span>|[<span data-ttu-id="8de1b-114">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="8de1b-114">WorkbookChartLineFormat</span></span>](chartlineformat.md)|<span data-ttu-id="8de1b-p101">グラフの線の書式設定を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="8de1b-p101">Represents chart line formatting. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="8de1b-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8de1b-117">JSON representation</span></span>

<span data-ttu-id="8de1b-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8de1b-118">Here is a JSON representation of the resource.</span></span>

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