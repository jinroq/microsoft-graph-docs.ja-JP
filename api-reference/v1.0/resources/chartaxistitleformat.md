---
title: ChartAxisTitleFormat リソースの種類
description: グラフ軸のタイトルの書式設定を表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 26d305d8bd4a0059123f77bd86cbbf5fd01dcea7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27959483"
---
# <a name="chartaxistitleformat-resource-type"></a><span data-ttu-id="a973b-103">ChartAxisTitleFormat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a973b-103">ChartAxisTitleFormat resource type</span></span>

<span data-ttu-id="a973b-104">グラフ軸のタイトルの書式設定を表します。</span><span class="sxs-lookup"><span data-stu-id="a973b-104">Represents the chart axis title formatting.</span></span>


## <a name="methods"></a><span data-ttu-id="a973b-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="a973b-105">Methods</span></span>
<span data-ttu-id="a973b-106">なし</span><span class="sxs-lookup"><span data-stu-id="a973b-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="a973b-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a973b-107">Properties</span></span>
<span data-ttu-id="a973b-108">なし</span><span class="sxs-lookup"><span data-stu-id="a973b-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="a973b-109">関係</span><span class="sxs-lookup"><span data-stu-id="a973b-109">Relationships</span></span>
| <span data-ttu-id="a973b-110">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a973b-110">Relationship</span></span> | <span data-ttu-id="a973b-111">型</span><span class="sxs-lookup"><span data-stu-id="a973b-111">Type</span></span>   |<span data-ttu-id="a973b-112">説明</span><span class="sxs-lookup"><span data-stu-id="a973b-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a973b-113">font</span><span class="sxs-lookup"><span data-stu-id="a973b-113">font</span></span>|[<span data-ttu-id="a973b-114">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="a973b-114">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="a973b-p101">グラフの軸タイトルのオブジェクトのフォント属性 (フォント名、フォント サイズ、色など) を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="a973b-p101">Represents the font attributes, such as font name, font size, color, etc. of chart axis title object. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a973b-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a973b-117">JSON representation</span></span>

<span data-ttu-id="a973b-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a973b-118">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartAxisTitleFormat"
}-->

```json
{
  "font": {"@odata.type": "microsoft.graph.workbookChartFont"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartAxisTitleFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
