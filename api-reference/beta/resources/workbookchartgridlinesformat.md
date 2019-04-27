---
title: workbookChartGridlinesFormat リソースの種類
description: グラフの目盛線の書式設定プロパティをカプセル化します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 53c6561ef9d7695a0096b928b7be4c7a72432960
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348891"
---
# <a name="workbookchartgridlinesformat-resource-type"></a><span data-ttu-id="c9ce3-103">workbookChartGridlinesFormat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c9ce3-103">workbookChartGridlinesFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c9ce3-104">グラフの目盛線の書式設定プロパティをカプセル化します。</span><span class="sxs-lookup"><span data-stu-id="c9ce3-104">Encapsulates the format properties for chart gridlines.</span></span>

## <a name="methods"></a><span data-ttu-id="c9ce3-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="c9ce3-105">Methods</span></span>
<span data-ttu-id="c9ce3-106">なし</span><span class="sxs-lookup"><span data-stu-id="c9ce3-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="c9ce3-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c9ce3-107">Properties</span></span>
<span data-ttu-id="c9ce3-108">なし</span><span class="sxs-lookup"><span data-stu-id="c9ce3-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="c9ce3-109">関係</span><span class="sxs-lookup"><span data-stu-id="c9ce3-109">Relationships</span></span>
| <span data-ttu-id="c9ce3-110">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c9ce3-110">Relationship</span></span> | <span data-ttu-id="c9ce3-111">型</span><span class="sxs-lookup"><span data-stu-id="c9ce3-111">Type</span></span>   |<span data-ttu-id="c9ce3-112">説明</span><span class="sxs-lookup"><span data-stu-id="c9ce3-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c9ce3-113">line</span><span class="sxs-lookup"><span data-stu-id="c9ce3-113">line</span></span>|[<span data-ttu-id="c9ce3-114">workbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="c9ce3-114">workbookChartLineFormat</span></span>](workbookchartlineformat.md)|<span data-ttu-id="c9ce3-115">グラフの線の書式設定を表します。</span><span class="sxs-lookup"><span data-stu-id="c9ce3-115">Represents chart line formatting.</span></span> <span data-ttu-id="c9ce3-116">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="c9ce3-116">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="c9ce3-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c9ce3-117">JSON representation</span></span>

<span data-ttu-id="c9ce3-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c9ce3-118">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "line"
    ],
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
<!--
{
  "type": "#page.annotation",
  "description": "ChartGridlinesFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
