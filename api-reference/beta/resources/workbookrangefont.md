---
title: workbookRangeFont リソースの種類
description: このオブジェクトは、オブジェクトのフォントの属性 (フォント名、フォント サイズ、色など) を表します。
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: b3982a8026cd720fe614b11405a37bed8626042d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964051"
---
# <a name="workbookrangefont-resource-type"></a><span data-ttu-id="90465-103">workbookRangeFont リソースの種類</span><span class="sxs-lookup"><span data-stu-id="90465-103">workbookRangeFont resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="90465-104">このオブジェクトは、オブジェクトのフォントの属性 (フォント名、フォント サイズ、色など) を表します。</span><span class="sxs-lookup"><span data-stu-id="90465-104">This object represents the font attributes (font name, font size, color, etc.) for an object.</span></span>


## <a name="methods"></a><span data-ttu-id="90465-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="90465-105">Methods</span></span>

| <span data-ttu-id="90465-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="90465-106">Method</span></span>           | <span data-ttu-id="90465-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="90465-107">Return Type</span></span>    |<span data-ttu-id="90465-108">説明</span><span class="sxs-lookup"><span data-stu-id="90465-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="90465-109">WorkbookRangeFont を取得する</span><span class="sxs-lookup"><span data-stu-id="90465-109">Get workbookRangeFont</span></span>](../api/rangefont-get.md) | [<span data-ttu-id="90465-110">workbookRangeFont</span><span class="sxs-lookup"><span data-stu-id="90465-110">workbookRangeFont</span></span>](workbookrangefont.md) |<span data-ttu-id="90465-111">rangeFont オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="90465-111">Read properties and relationships of rangeFont object.</span></span>|
|[<span data-ttu-id="90465-112">Update</span><span class="sxs-lookup"><span data-stu-id="90465-112">Update</span></span>](../api/rangefont-update.md) | [<span data-ttu-id="90465-113">workbookRangeFont</span><span class="sxs-lookup"><span data-stu-id="90465-113">workbookRangeFont</span></span>](workbookrangefont.md)   |<span data-ttu-id="90465-114">RangeFont オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="90465-114">Update RangeFont object.</span></span> |

## <a name="properties"></a><span data-ttu-id="90465-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="90465-115">Properties</span></span>
| <span data-ttu-id="90465-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="90465-116">Property</span></span>     | <span data-ttu-id="90465-117">型</span><span class="sxs-lookup"><span data-stu-id="90465-117">Type</span></span>   |<span data-ttu-id="90465-118">説明</span><span class="sxs-lookup"><span data-stu-id="90465-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="90465-119">bold</span><span class="sxs-lookup"><span data-stu-id="90465-119">bold</span></span>|<span data-ttu-id="90465-120">ブール値</span><span class="sxs-lookup"><span data-stu-id="90465-120">boolean</span></span>|<span data-ttu-id="90465-121">フォントの太字の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="90465-121">Represents the bold status of font.</span></span>|
|<span data-ttu-id="90465-122">color</span><span class="sxs-lookup"><span data-stu-id="90465-122">color</span></span>|<span data-ttu-id="90465-123">string</span><span class="sxs-lookup"><span data-stu-id="90465-123">string</span></span>|<span data-ttu-id="90465-p101">テキストの色の HTML カラー コード表記。たとえば、#FF0000 は赤を表します。</span><span class="sxs-lookup"><span data-stu-id="90465-p101">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="90465-127">italic</span><span class="sxs-lookup"><span data-stu-id="90465-127">italic</span></span>|<span data-ttu-id="90465-128">ブール値</span><span class="sxs-lookup"><span data-stu-id="90465-128">boolean</span></span>|<span data-ttu-id="90465-129">フォントの斜体の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="90465-129">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="90465-130">name</span><span class="sxs-lookup"><span data-stu-id="90465-130">name</span></span>|<span data-ttu-id="90465-131">string</span><span class="sxs-lookup"><span data-stu-id="90465-131">string</span></span>|<span data-ttu-id="90465-132">フォント名 (例: "Calibri")</span><span class="sxs-lookup"><span data-stu-id="90465-132">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="90465-133">size</span><span class="sxs-lookup"><span data-stu-id="90465-133">size</span></span>|<span data-ttu-id="90465-134">double</span><span class="sxs-lookup"><span data-stu-id="90465-134">double</span></span>|<span data-ttu-id="90465-135">フォント サイズ</span><span class="sxs-lookup"><span data-stu-id="90465-135">Font size.</span></span>|
|<span data-ttu-id="90465-136">underline</span><span class="sxs-lookup"><span data-stu-id="90465-136">underline</span></span>| <span data-ttu-id="90465-137">String</span><span class="sxs-lookup"><span data-stu-id="90465-137">String</span></span> |<span data-ttu-id="90465-138">フォントに適用する下線の種類。</span><span class="sxs-lookup"><span data-stu-id="90465-138">Type of underline applied to the font.</span></span> <span data-ttu-id="90465-139">可能な値は、`None`、`Single`、`Double`、`SingleAccountant`、`DoubleAccountant` です。</span><span class="sxs-lookup"><span data-stu-id="90465-139">Possible values are: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="90465-140">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="90465-140">Relationships</span></span>
<span data-ttu-id="90465-141">なし</span><span class="sxs-lookup"><span data-stu-id="90465-141">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="90465-142">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="90465-142">JSON representation</span></span>

<span data-ttu-id="90465-143">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="90465-143">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookRangeFont"
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
  "suppressions": []
}
-->
