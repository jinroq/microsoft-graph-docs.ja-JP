---
title: workbookChartGridlinesFormat リソースの種類
description: グラフの目盛線の書式設定プロパティをカプセル化します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 6d32e916b3156082b45cbcaa105fd55e1c377b2e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007278"
---
# <a name="workbookchartgridlinesformat-resource-type"></a><span data-ttu-id="20f6e-103">workbookChartGridlinesFormat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="20f6e-103">workbookChartGridlinesFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="20f6e-104">グラフの目盛線の書式設定プロパティをカプセル化します。</span><span class="sxs-lookup"><span data-stu-id="20f6e-104">Encapsulates the format properties for chart gridlines.</span></span>

## <a name="methods"></a><span data-ttu-id="20f6e-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="20f6e-105">Methods</span></span>
<span data-ttu-id="20f6e-106">None</span><span class="sxs-lookup"><span data-stu-id="20f6e-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="20f6e-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="20f6e-107">Properties</span></span>
<span data-ttu-id="20f6e-108">なし</span><span class="sxs-lookup"><span data-stu-id="20f6e-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="20f6e-109">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="20f6e-109">Relationships</span></span>
| <span data-ttu-id="20f6e-110">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="20f6e-110">Relationship</span></span> | <span data-ttu-id="20f6e-111">型</span><span class="sxs-lookup"><span data-stu-id="20f6e-111">Type</span></span>   |<span data-ttu-id="20f6e-112">説明</span><span class="sxs-lookup"><span data-stu-id="20f6e-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="20f6e-113">line</span><span class="sxs-lookup"><span data-stu-id="20f6e-113">line</span></span>|[<span data-ttu-id="20f6e-114">workbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="20f6e-114">workbookChartLineFormat</span></span>](workbookchartlineformat.md)|<span data-ttu-id="20f6e-115">グラフの線の書式設定を表します。</span><span class="sxs-lookup"><span data-stu-id="20f6e-115">Represents chart line formatting.</span></span> <span data-ttu-id="20f6e-116">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="20f6e-116">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="20f6e-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="20f6e-117">JSON representation</span></span>

<span data-ttu-id="20f6e-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="20f6e-118">Here is a JSON representation of the resource.</span></span>

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
