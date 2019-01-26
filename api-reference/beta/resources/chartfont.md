---
title: ChartFont リソースの種類
description: このオブジェクトは、グラフ オブジェクトのフォント属性 (フォント名、フォント サイズ、色など) を表します。
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 7e9815d5d6d9bf7e7b0ef4ae97881e12c7ba9181
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573628"
---
# <a name="chartfont-resource-type"></a><span data-ttu-id="60912-103">ChartFont リソースの種類</span><span class="sxs-lookup"><span data-stu-id="60912-103">ChartFont resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="60912-104">このオブジェクトは、グラフ オブジェクトのフォント属性 (フォント名、フォント サイズ、色など) を表します。</span><span class="sxs-lookup"><span data-stu-id="60912-104">This object represents the font attributes (font name, font size, color, etc.) for a chart object.</span></span>


## <a name="methods"></a><span data-ttu-id="60912-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="60912-105">Methods</span></span>

| <span data-ttu-id="60912-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="60912-106">Method</span></span>           | <span data-ttu-id="60912-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="60912-107">Return Type</span></span>    |<span data-ttu-id="60912-108">説明</span><span class="sxs-lookup"><span data-stu-id="60912-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="60912-109">Get ChartFont</span><span class="sxs-lookup"><span data-stu-id="60912-109">Get ChartFont</span></span>](../api/chartfont-get.md) | [<span data-ttu-id="60912-110">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="60912-110">WorkbookChartFont</span></span>](chartfont.md) |<span data-ttu-id="60912-111">chartFont オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="60912-111">Read properties and relationships of chartFont object.</span></span>|
|[<span data-ttu-id="60912-112">Update</span><span class="sxs-lookup"><span data-stu-id="60912-112">Update</span></span>](../api/chartfont-update.md) | [<span data-ttu-id="60912-113">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="60912-113">WorkbookChartFont</span></span>](chartfont.md)   |<span data-ttu-id="60912-114">ChartFont オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="60912-114">Update ChartFont object.</span></span> |

## <a name="properties"></a><span data-ttu-id="60912-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="60912-115">Properties</span></span>
| <span data-ttu-id="60912-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="60912-116">Property</span></span>     | <span data-ttu-id="60912-117">型</span><span class="sxs-lookup"><span data-stu-id="60912-117">Type</span></span>   |<span data-ttu-id="60912-118">説明</span><span class="sxs-lookup"><span data-stu-id="60912-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="60912-119">bold</span><span class="sxs-lookup"><span data-stu-id="60912-119">bold</span></span>|<span data-ttu-id="60912-120">boolean</span><span class="sxs-lookup"><span data-stu-id="60912-120">boolean</span></span>|<span data-ttu-id="60912-121">フォントの太字の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="60912-121">Represents the bold status of font.</span></span>|
|<span data-ttu-id="60912-122">color</span><span class="sxs-lookup"><span data-stu-id="60912-122">color</span></span>|<span data-ttu-id="60912-123">文字列</span><span class="sxs-lookup"><span data-stu-id="60912-123">string</span></span>|<span data-ttu-id="60912-p101">テキストの色の HTML カラー コード表記。たとえば、#FF0000 は赤を表します。</span><span class="sxs-lookup"><span data-stu-id="60912-p101">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="60912-127">italic</span><span class="sxs-lookup"><span data-stu-id="60912-127">italic</span></span>|<span data-ttu-id="60912-128">boolean</span><span class="sxs-lookup"><span data-stu-id="60912-128">boolean</span></span>|<span data-ttu-id="60912-129">フォントの斜体の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="60912-129">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="60912-130">name</span><span class="sxs-lookup"><span data-stu-id="60912-130">name</span></span>|<span data-ttu-id="60912-131">文字列</span><span class="sxs-lookup"><span data-stu-id="60912-131">string</span></span>|<span data-ttu-id="60912-132">フォント名 (例: "Calibri")</span><span class="sxs-lookup"><span data-stu-id="60912-132">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="60912-133">size</span><span class="sxs-lookup"><span data-stu-id="60912-133">size</span></span>|<span data-ttu-id="60912-134">double</span><span class="sxs-lookup"><span data-stu-id="60912-134">double</span></span>|<span data-ttu-id="60912-135">フォント サイズ (例: 11)</span><span class="sxs-lookup"><span data-stu-id="60912-135">Size of the font (e.g. 11)</span></span>|
|<span data-ttu-id="60912-136">underline</span><span class="sxs-lookup"><span data-stu-id="60912-136">underline</span></span>|<span data-ttu-id="60912-137">文字列</span><span class="sxs-lookup"><span data-stu-id="60912-137">string</span></span>|<span data-ttu-id="60912-138">フォントに適用する下線の種類です。</span><span class="sxs-lookup"><span data-stu-id="60912-138">Type of underline applied to the font.</span></span> <span data-ttu-id="60912-139">可能な値: `None`、 `Single`。</span><span class="sxs-lookup"><span data-stu-id="60912-139">The possible values are: `None`, `Single`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="60912-140">関係</span><span class="sxs-lookup"><span data-stu-id="60912-140">Relationships</span></span>
<span data-ttu-id="60912-141">なし</span><span class="sxs-lookup"><span data-stu-id="60912-141">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="60912-142">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="60912-142">JSON representation</span></span>

<span data-ttu-id="60912-143">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="60912-143">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.workbookChartFont"
}-->

```json
{
  "bold": true,
  "color": "string",
  "italic": true,
  "name": "string",
  "size": 1024,
  "underline": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartFont resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chartfont.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
