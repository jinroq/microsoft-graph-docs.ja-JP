---
title: ChartAxisTitleFormat リソースの種類
description: グラフ軸のタイトルの書式設定を表します。
ms.openlocfilehash: 417c594096ae19c0a223eaeaa543827f91306e8c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022827"
---
# <a name="chartaxistitleformat-resource-type"></a><span data-ttu-id="0bcfe-103">ChartAxisTitleFormat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0bcfe-103">ChartAxisTitleFormat resource type</span></span>

<span data-ttu-id="0bcfe-104">グラフ軸のタイトルの書式設定を表します。</span><span class="sxs-lookup"><span data-stu-id="0bcfe-104">Represents the chart axis title formatting.</span></span>


## <a name="methods"></a><span data-ttu-id="0bcfe-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="0bcfe-105">Methods</span></span>
<span data-ttu-id="0bcfe-106">なし</span><span class="sxs-lookup"><span data-stu-id="0bcfe-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="0bcfe-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0bcfe-107">Properties</span></span>
<span data-ttu-id="0bcfe-108">なし</span><span class="sxs-lookup"><span data-stu-id="0bcfe-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="0bcfe-109">関係</span><span class="sxs-lookup"><span data-stu-id="0bcfe-109">Relationships</span></span>
| <span data-ttu-id="0bcfe-110">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0bcfe-110">Relationship</span></span> | <span data-ttu-id="0bcfe-111">型</span><span class="sxs-lookup"><span data-stu-id="0bcfe-111">Type</span></span>   |<span data-ttu-id="0bcfe-112">説明</span><span class="sxs-lookup"><span data-stu-id="0bcfe-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0bcfe-113">font</span><span class="sxs-lookup"><span data-stu-id="0bcfe-113">font</span></span>|[<span data-ttu-id="0bcfe-114">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="0bcfe-114">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="0bcfe-p101">グラフの軸タイトルのオブジェクトのフォント属性 (フォント名、フォント サイズ、色など) を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="0bcfe-p101">Represents the font attributes, such as font name, font size, color, etc. of chart axis title object. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0bcfe-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0bcfe-117">JSON representation</span></span>

<span data-ttu-id="0bcfe-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0bcfe-118">Here is a JSON representation of the resource.</span></span>

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