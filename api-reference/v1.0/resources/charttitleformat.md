---
title: ChartTitleFormat リソースの種類
description: グラフ タイトルの書式設定プロパティをカプセル化します。
ms.openlocfilehash: 7e84412adb46981a0a2b8570ed28c62d36936e36
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27021069"
---
# <a name="charttitleformat-resource-type"></a><span data-ttu-id="bdd5b-103">ChartTitleFormat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bdd5b-103">ChartTitleFormat resource type</span></span>

<span data-ttu-id="bdd5b-104">グラフ タイトルの書式設定プロパティをカプセル化します。</span><span class="sxs-lookup"><span data-stu-id="bdd5b-104">Encapsulates the format properties for the chart title.</span></span>


## <a name="methods"></a><span data-ttu-id="bdd5b-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="bdd5b-105">Methods</span></span>
<span data-ttu-id="bdd5b-106">なし</span><span class="sxs-lookup"><span data-stu-id="bdd5b-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="bdd5b-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bdd5b-107">Properties</span></span>
<span data-ttu-id="bdd5b-108">なし</span><span class="sxs-lookup"><span data-stu-id="bdd5b-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="bdd5b-109">関係</span><span class="sxs-lookup"><span data-stu-id="bdd5b-109">Relationships</span></span>
| <span data-ttu-id="bdd5b-110">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="bdd5b-110">Relationship</span></span> | <span data-ttu-id="bdd5b-111">型</span><span class="sxs-lookup"><span data-stu-id="bdd5b-111">Type</span></span>   |<span data-ttu-id="bdd5b-112">説明</span><span class="sxs-lookup"><span data-stu-id="bdd5b-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bdd5b-113">fill</span><span class="sxs-lookup"><span data-stu-id="bdd5b-113">fill</span></span>|[<span data-ttu-id="bdd5b-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="bdd5b-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="bdd5b-p101">背景の書式設定情報を含む、オブジェクトの塗りつぶしの書式を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="bdd5b-p101">Represents the fill format of an object, which includes background formatting information. Read-only.</span></span>|
|<span data-ttu-id="bdd5b-117">font</span><span class="sxs-lookup"><span data-stu-id="bdd5b-117">font</span></span>|[<span data-ttu-id="bdd5b-118">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="bdd5b-118">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="bdd5b-p102">現在のオブジェクトのフォント属性 (フォント名、フォント サイズ、色など) を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="bdd5b-p102">Represents the font attributes (font name, font size, color, etc.) for the current object. Read-only.</span></span>|



## <a name="json-representation"></a><span data-ttu-id="bdd5b-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bdd5b-121">JSON representation</span></span>

<span data-ttu-id="bdd5b-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="bdd5b-122">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartTitleFormat"
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
