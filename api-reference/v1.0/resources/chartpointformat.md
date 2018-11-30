---
title: ChartPointFormat リソースの種類
description: グラフのポイントの書式設定オブジェクトを表します。
ms.openlocfilehash: f06b31ad030dd587128f35667145f19d5cbd2e7e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022213"
---
# <a name="chartpointformat-resource-type"></a><span data-ttu-id="737ac-103">ChartPointFormat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="737ac-103">ChartPointFormat resource type</span></span>

<span data-ttu-id="737ac-104">グラフのポイントの書式設定オブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="737ac-104">Represents formatting object for chart points.</span></span>


## <a name="methods"></a><span data-ttu-id="737ac-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="737ac-105">Methods</span></span>
<span data-ttu-id="737ac-106">なし</span><span class="sxs-lookup"><span data-stu-id="737ac-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="737ac-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="737ac-107">Properties</span></span>
<span data-ttu-id="737ac-108">なし</span><span class="sxs-lookup"><span data-stu-id="737ac-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="737ac-109">関係</span><span class="sxs-lookup"><span data-stu-id="737ac-109">Relationships</span></span>
| <span data-ttu-id="737ac-110">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="737ac-110">Relationship</span></span> | <span data-ttu-id="737ac-111">型</span><span class="sxs-lookup"><span data-stu-id="737ac-111">Type</span></span>   |<span data-ttu-id="737ac-112">説明</span><span class="sxs-lookup"><span data-stu-id="737ac-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="737ac-113">fill</span><span class="sxs-lookup"><span data-stu-id="737ac-113">fill</span></span>|[<span data-ttu-id="737ac-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="737ac-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="737ac-p101">グラフの塗りつぶしの書式を表します。これには背景の書式設定情報などがあります。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="737ac-p101">Represents the fill format of a chart, which includes background formating information. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="737ac-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="737ac-117">JSON representation</span></span>

<span data-ttu-id="737ac-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="737ac-118">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartPointFormat"
}-->

```json
{
  "fill": {"@odata.type": "microsoft.graph.workbookChartFill"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartPointFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->