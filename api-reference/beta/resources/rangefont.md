---
title: RangeFont リソースの種類
description: このオブジェクトは、オブジェクトのフォントの属性 (フォント名、フォント サイズ、色など) を表します。
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 2dee07b7d2573081650bdd15799e4884c774e171
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563414"
---
# <a name="rangefont-resource-type"></a><span data-ttu-id="a7c54-103">RangeFont リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a7c54-103">RangeFont resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a7c54-104">このオブジェクトは、オブジェクトのフォントの属性 (フォント名、フォント サイズ、色など) を表します。</span><span class="sxs-lookup"><span data-stu-id="a7c54-104">This object represents the font attributes (font name, font size, color, etc.) for an object.</span></span>


## <a name="methods"></a><span data-ttu-id="a7c54-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="a7c54-105">Methods</span></span>

| <span data-ttu-id="a7c54-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="a7c54-106">Method</span></span>           | <span data-ttu-id="a7c54-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="a7c54-107">Return Type</span></span>    |<span data-ttu-id="a7c54-108">説明</span><span class="sxs-lookup"><span data-stu-id="a7c54-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a7c54-109">RangeFont を取得する</span><span class="sxs-lookup"><span data-stu-id="a7c54-109">Get RangeFont</span></span>](../api/rangefont-get.md) | [<span data-ttu-id="a7c54-110">RangeFont</span><span class="sxs-lookup"><span data-stu-id="a7c54-110">RangeFont</span></span>](rangefont.md) |<span data-ttu-id="a7c54-111">rangeFont オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="a7c54-111">Read properties and relationships of rangeFont object.</span></span>|
|[<span data-ttu-id="a7c54-112">Update</span><span class="sxs-lookup"><span data-stu-id="a7c54-112">Update</span></span>](../api/rangefont-update.md) | [<span data-ttu-id="a7c54-113">RangeFont</span><span class="sxs-lookup"><span data-stu-id="a7c54-113">RangeFont</span></span>](rangefont.md)   |<span data-ttu-id="a7c54-114">RangeFont オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="a7c54-114">Update RangeFont object.</span></span> |

## <a name="properties"></a><span data-ttu-id="a7c54-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a7c54-115">Properties</span></span>
| <span data-ttu-id="a7c54-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a7c54-116">Property</span></span>     | <span data-ttu-id="a7c54-117">型</span><span class="sxs-lookup"><span data-stu-id="a7c54-117">Type</span></span>   |<span data-ttu-id="a7c54-118">説明</span><span class="sxs-lookup"><span data-stu-id="a7c54-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a7c54-119">bold</span><span class="sxs-lookup"><span data-stu-id="a7c54-119">bold</span></span>|<span data-ttu-id="a7c54-120">ブール値</span><span class="sxs-lookup"><span data-stu-id="a7c54-120">boolean</span></span>|<span data-ttu-id="a7c54-121">フォントの太字の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="a7c54-121">Represents the bold status of font.</span></span>|
|<span data-ttu-id="a7c54-122">color</span><span class="sxs-lookup"><span data-stu-id="a7c54-122">color</span></span>|<span data-ttu-id="a7c54-123">string</span><span class="sxs-lookup"><span data-stu-id="a7c54-123">string</span></span>|<span data-ttu-id="a7c54-p101">テキストの色の HTML カラー コード表記。たとえば、#FF0000 は赤を表します。</span><span class="sxs-lookup"><span data-stu-id="a7c54-p101">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="a7c54-127">italic</span><span class="sxs-lookup"><span data-stu-id="a7c54-127">italic</span></span>|<span data-ttu-id="a7c54-128">ブール値</span><span class="sxs-lookup"><span data-stu-id="a7c54-128">boolean</span></span>|<span data-ttu-id="a7c54-129">フォントの斜体の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="a7c54-129">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="a7c54-130">name</span><span class="sxs-lookup"><span data-stu-id="a7c54-130">name</span></span>|<span data-ttu-id="a7c54-131">string</span><span class="sxs-lookup"><span data-stu-id="a7c54-131">string</span></span>|<span data-ttu-id="a7c54-132">フォント名 (例: "Calibri")</span><span class="sxs-lookup"><span data-stu-id="a7c54-132">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="a7c54-133">size</span><span class="sxs-lookup"><span data-stu-id="a7c54-133">size</span></span>|<span data-ttu-id="a7c54-134">double</span><span class="sxs-lookup"><span data-stu-id="a7c54-134">double</span></span>|<span data-ttu-id="a7c54-135">フォント サイズ</span><span class="sxs-lookup"><span data-stu-id="a7c54-135">Font size.</span></span>|
|<span data-ttu-id="a7c54-136">underline</span><span class="sxs-lookup"><span data-stu-id="a7c54-136">underline</span></span>|<span data-ttu-id="a7c54-137">文字列</span><span class="sxs-lookup"><span data-stu-id="a7c54-137">string</span></span>|<span data-ttu-id="a7c54-p102">フォントに適用する下線の種類。可能な値は、`None`、`Single`、`Double`、`SingleAccountant`、`DoubleAccountant` です。</span><span class="sxs-lookup"><span data-stu-id="a7c54-p102">Type of underline applied to the font. Possible values are: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a7c54-140">関係</span><span class="sxs-lookup"><span data-stu-id="a7c54-140">Relationships</span></span>
<span data-ttu-id="a7c54-141">なし</span><span class="sxs-lookup"><span data-stu-id="a7c54-141">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="a7c54-142">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a7c54-142">JSON representation</span></span>

<span data-ttu-id="a7c54-143">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a7c54-143">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.rangeFont"
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
  "description": "RangeFont resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/rangefont.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
