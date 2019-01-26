---
title: ChartTitleFormat リソースの種類
description: グラフ タイトルの書式設定プロパティをカプセル化します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 7dd9400873234fd73ebe506a49caf6583d05b75b
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574013"
---
# <a name="charttitleformat-resource-type"></a><span data-ttu-id="25d48-103">ChartTitleFormat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="25d48-103">ChartTitleFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


## <a name="methods"></a><span data-ttu-id="25d48-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="25d48-104">Methods</span></span>
<span data-ttu-id="25d48-105">なし</span><span class="sxs-lookup"><span data-stu-id="25d48-105">None</span></span>

## <a name="properties"></a><span data-ttu-id="25d48-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="25d48-106">Properties</span></span>
<span data-ttu-id="25d48-107">なし</span><span class="sxs-lookup"><span data-stu-id="25d48-107">None</span></span>

## <a name="relationships"></a><span data-ttu-id="25d48-108">関係</span><span class="sxs-lookup"><span data-stu-id="25d48-108">Relationships</span></span>
| <span data-ttu-id="25d48-109">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="25d48-109">Relationship</span></span> | <span data-ttu-id="25d48-110">型</span><span class="sxs-lookup"><span data-stu-id="25d48-110">Type</span></span>   |<span data-ttu-id="25d48-111">説明</span><span class="sxs-lookup"><span data-stu-id="25d48-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="25d48-112">fill</span><span class="sxs-lookup"><span data-stu-id="25d48-112">fill</span></span>|[<span data-ttu-id="25d48-113">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="25d48-113">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="25d48-p101">背景の書式設定情報を含む、オブジェクトの塗りつぶしの書式を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="25d48-p101">Represents the fill format of an object, which includes background formatting information. Read-only.</span></span>|
|<span data-ttu-id="25d48-116">font</span><span class="sxs-lookup"><span data-stu-id="25d48-116">font</span></span>|[<span data-ttu-id="25d48-117">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="25d48-117">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="25d48-p102">現在のオブジェクトのフォント属性 (フォント名、フォント サイズ、色など) を表します。値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="25d48-p102">Represents the font attributes (font name, font size, color, etc.) for the current object. Read-only.</span></span>|



## <a name="json-representation"></a><span data-ttu-id="25d48-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="25d48-120">JSON representation</span></span>

<span data-ttu-id="25d48-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="25d48-121">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "ChartAreaFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/charttitleformat.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
