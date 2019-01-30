---
title: ChartFont リソースの種類
description: このオブジェクトは、グラフ オブジェクトのフォント属性 (フォント名、フォント サイズ、色など) を表します。
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: c507a966dc6b29e46935c5c77a85b557a84cc69c
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641170"
---
# <a name="chartfont-resource-type"></a><span data-ttu-id="61923-103">ChartFont リソースの種類</span><span class="sxs-lookup"><span data-stu-id="61923-103">ChartFont resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="61923-104">このオブジェクトは、グラフ オブジェクトのフォント属性 (フォント名、フォント サイズ、色など) を表します。</span><span class="sxs-lookup"><span data-stu-id="61923-104">This object represents the font attributes (font name, font size, color, etc.) for a chart object.</span></span>


## <a name="methods"></a><span data-ttu-id="61923-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="61923-105">Methods</span></span>

| <span data-ttu-id="61923-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="61923-106">Method</span></span>           | <span data-ttu-id="61923-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="61923-107">Return Type</span></span>    |<span data-ttu-id="61923-108">説明</span><span class="sxs-lookup"><span data-stu-id="61923-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="61923-109">Get ChartFont</span><span class="sxs-lookup"><span data-stu-id="61923-109">Get ChartFont</span></span>](../api/chartfont-get.md) | [<span data-ttu-id="61923-110">ChartFont</span><span class="sxs-lookup"><span data-stu-id="61923-110">ChartFont</span></span>](chartfont.md) |<span data-ttu-id="61923-111">chartFont オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="61923-111">Read properties and relationships of chartFont object.</span></span>|
|[<span data-ttu-id="61923-112">更新する</span><span class="sxs-lookup"><span data-stu-id="61923-112">Update</span></span>](../api/chartfont-update.md) | [<span data-ttu-id="61923-113">ChartFont</span><span class="sxs-lookup"><span data-stu-id="61923-113">ChartFont</span></span>](chartfont.md)   |<span data-ttu-id="61923-114">ChartFont オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="61923-114">Update ChartFont object.</span></span> |

## <a name="properties"></a><span data-ttu-id="61923-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="61923-115">Properties</span></span>
| <span data-ttu-id="61923-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="61923-116">Property</span></span>     | <span data-ttu-id="61923-117">型</span><span class="sxs-lookup"><span data-stu-id="61923-117">Type</span></span>   |<span data-ttu-id="61923-118">説明</span><span class="sxs-lookup"><span data-stu-id="61923-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="61923-119">bold</span><span class="sxs-lookup"><span data-stu-id="61923-119">bold</span></span>|<span data-ttu-id="61923-120">ブール値</span><span class="sxs-lookup"><span data-stu-id="61923-120">boolean</span></span>|<span data-ttu-id="61923-121">フォントの太字の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="61923-121">Represents the bold status of font.</span></span>|
|<span data-ttu-id="61923-122">color</span><span class="sxs-lookup"><span data-stu-id="61923-122">color</span></span>|<span data-ttu-id="61923-123">文字列</span><span class="sxs-lookup"><span data-stu-id="61923-123">string</span></span>|<span data-ttu-id="61923-p101">テキストの色の HTML カラー コード表記。たとえば、#FF0000 は赤を表します。</span><span class="sxs-lookup"><span data-stu-id="61923-p101">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="61923-127">italic</span><span class="sxs-lookup"><span data-stu-id="61923-127">italic</span></span>|<span data-ttu-id="61923-128">ブール値</span><span class="sxs-lookup"><span data-stu-id="61923-128">boolean</span></span>|<span data-ttu-id="61923-129">フォントの斜体の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="61923-129">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="61923-130">name</span><span class="sxs-lookup"><span data-stu-id="61923-130">name</span></span>|<span data-ttu-id="61923-131">文字列</span><span class="sxs-lookup"><span data-stu-id="61923-131">string</span></span>|<span data-ttu-id="61923-132">フォント名 (例: "Calibri")</span><span class="sxs-lookup"><span data-stu-id="61923-132">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="61923-133">size</span><span class="sxs-lookup"><span data-stu-id="61923-133">size</span></span>|<span data-ttu-id="61923-134">double</span><span class="sxs-lookup"><span data-stu-id="61923-134">double</span></span>|<span data-ttu-id="61923-135">フォント サイズ (例: 11)</span><span class="sxs-lookup"><span data-stu-id="61923-135">Size of the font (e.g. 11)</span></span>|
|<span data-ttu-id="61923-136">underline</span><span class="sxs-lookup"><span data-stu-id="61923-136">underline</span></span>|<span data-ttu-id="61923-137">文字列</span><span class="sxs-lookup"><span data-stu-id="61923-137">string</span></span>|<span data-ttu-id="61923-p102">フォントに適用する下線の種類。可能な値は、`None`、`Single` です。</span><span class="sxs-lookup"><span data-stu-id="61923-p102">Type of underline applied to the font. Possible values are: `None`, `Single`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="61923-140">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="61923-140">Relationships</span></span>
<span data-ttu-id="61923-141">なし</span><span class="sxs-lookup"><span data-stu-id="61923-141">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="61923-142">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="61923-142">JSON representation</span></span>

<span data-ttu-id="61923-143">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="61923-143">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartFont"
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
