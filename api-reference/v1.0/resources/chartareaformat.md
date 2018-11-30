---
title: ChartAreaFormat リソースの種類
description: グラフ領域全体の書式設定プロパティをカプセル化します。
ms.openlocfilehash: 19f09ab735f6df4fe4cdc0ccbf13bc75a5ca834e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020541"
---
# <a name="chartareaformat-resource-type"></a><span data-ttu-id="47933-103">ChartAreaFormat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="47933-103">ChartAreaFormat resource type</span></span>

<span data-ttu-id="47933-104">グラフ領域全体の書式設定プロパティをカプセル化します。</span><span class="sxs-lookup"><span data-stu-id="47933-104">Encapsulates the format properties for the overall chart area.</span></span>


## <a name="methods"></a><span data-ttu-id="47933-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="47933-105">Methods</span></span>
<span data-ttu-id="47933-106">なし</span><span class="sxs-lookup"><span data-stu-id="47933-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="47933-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="47933-107">Properties</span></span>
<span data-ttu-id="47933-108">なし</span><span class="sxs-lookup"><span data-stu-id="47933-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="47933-109">関係</span><span class="sxs-lookup"><span data-stu-id="47933-109">Relationships</span></span>
| <span data-ttu-id="47933-110">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="47933-110">Relationship</span></span> | <span data-ttu-id="47933-111">型</span><span class="sxs-lookup"><span data-stu-id="47933-111">Type</span></span>   |<span data-ttu-id="47933-112">説明</span><span class="sxs-lookup"><span data-stu-id="47933-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="47933-113">fill</span><span class="sxs-lookup"><span data-stu-id="47933-113">fill</span></span>|[<span data-ttu-id="47933-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="47933-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="47933-p101">背景の書式設定情報を含む、オブジェクトの塗りつぶしの書式を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="47933-p101">Represents the fill format of an object, which includes background formatting information. Read-only.</span></span>|
|<span data-ttu-id="47933-117">font</span><span class="sxs-lookup"><span data-stu-id="47933-117">font</span></span>|[<span data-ttu-id="47933-118">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="47933-118">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="47933-p102">現在のオブジェクトのフォント属性 (フォント名、フォント サイズ、色など) を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="47933-p102">Represents the font attributes (font name, font size, color, etc.) for the current object. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="47933-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="47933-121">JSON representation</span></span>

<span data-ttu-id="47933-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="47933-122">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartAreaFormat"
}-->

```json
{
  "fill": {"@odata.type": "microsoft.graph.workbookChartFill"},
  "font": {"@odata.type": "microsoft.graph.workbookChartFont"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartAreaFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->