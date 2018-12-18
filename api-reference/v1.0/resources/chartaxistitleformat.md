---
title: ChartAxisTitleFormat リソースの種類
description: グラフ軸のタイトルの書式設定を表します。
author: lumine2008
ms.openlocfilehash: 7a160f02f06c74edeee09f91b2b117ea437291e8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343023"
---
# <a name="chartaxistitleformat-resource-type"></a><span data-ttu-id="7f8e5-103">ChartAxisTitleFormat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7f8e5-103">ChartAxisTitleFormat resource type</span></span>

<span data-ttu-id="7f8e5-104">グラフ軸のタイトルの書式設定を表します。</span><span class="sxs-lookup"><span data-stu-id="7f8e5-104">Represents the chart axis title formatting.</span></span>


## <a name="methods"></a><span data-ttu-id="7f8e5-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="7f8e5-105">Methods</span></span>
<span data-ttu-id="7f8e5-106">なし</span><span class="sxs-lookup"><span data-stu-id="7f8e5-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="7f8e5-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7f8e5-107">Properties</span></span>
<span data-ttu-id="7f8e5-108">なし</span><span class="sxs-lookup"><span data-stu-id="7f8e5-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="7f8e5-109">関係</span><span class="sxs-lookup"><span data-stu-id="7f8e5-109">Relationships</span></span>
| <span data-ttu-id="7f8e5-110">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7f8e5-110">Relationship</span></span> | <span data-ttu-id="7f8e5-111">型</span><span class="sxs-lookup"><span data-stu-id="7f8e5-111">Type</span></span>   |<span data-ttu-id="7f8e5-112">説明</span><span class="sxs-lookup"><span data-stu-id="7f8e5-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7f8e5-113">font</span><span class="sxs-lookup"><span data-stu-id="7f8e5-113">font</span></span>|[<span data-ttu-id="7f8e5-114">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="7f8e5-114">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="7f8e5-p101">グラフの軸タイトルのオブジェクトのフォント属性 (フォント名、フォント サイズ、色など) を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="7f8e5-p101">Represents the font attributes, such as font name, font size, color, etc. of chart axis title object. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7f8e5-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7f8e5-117">JSON representation</span></span>

<span data-ttu-id="7f8e5-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7f8e5-118">Here is a JSON representation of the resource.</span></span>

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