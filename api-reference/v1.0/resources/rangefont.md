---
title: RangeFont リソースの種類
description: このオブジェクトは、オブジェクトのフォントの属性 (フォント名、フォント サイズ、色など) を表します。
localization_priority: Normal
ms.openlocfilehash: 32bbd29706966c4c4b15f038ebdbb872b1dd8193
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27856582"
---
# <a name="rangefont-resource-type"></a><span data-ttu-id="aecef-103">RangeFont リソースの種類</span><span class="sxs-lookup"><span data-stu-id="aecef-103">RangeFont resource type</span></span>

<span data-ttu-id="aecef-104">このオブジェクトは、オブジェクトのフォントの属性 (フォント名、フォント サイズ、色など) を表します。</span><span class="sxs-lookup"><span data-stu-id="aecef-104">This object represents the font attributes (font name, font size, color, etc.) for an object.</span></span>


## <a name="methods"></a><span data-ttu-id="aecef-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="aecef-105">Methods</span></span>

| <span data-ttu-id="aecef-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="aecef-106">Method</span></span>           | <span data-ttu-id="aecef-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="aecef-107">Return Type</span></span>    |<span data-ttu-id="aecef-108">説明</span><span class="sxs-lookup"><span data-stu-id="aecef-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="aecef-109">RangeFont を取得する</span><span class="sxs-lookup"><span data-stu-id="aecef-109">Get RangeFont</span></span>](../api/rangefont-get.md) | [<span data-ttu-id="aecef-110">WorkbookRangeFont</span><span class="sxs-lookup"><span data-stu-id="aecef-110">WorkbookRangeFont</span></span>](rangefont.md) |<span data-ttu-id="aecef-111">rangeFont オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="aecef-111">Read properties and relationships of rangeFont object.</span></span>|
|[<span data-ttu-id="aecef-112">Update</span><span class="sxs-lookup"><span data-stu-id="aecef-112">Update</span></span>](../api/rangefont-update.md) | [<span data-ttu-id="aecef-113">WorkbookRangeFont</span><span class="sxs-lookup"><span data-stu-id="aecef-113">WorkbookRangeFont</span></span>](rangefont.md)   |<span data-ttu-id="aecef-114">RangeFont オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="aecef-114">Update RangeFont object.</span></span> |

## <a name="properties"></a><span data-ttu-id="aecef-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aecef-115">Properties</span></span>
| <span data-ttu-id="aecef-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aecef-116">Property</span></span>     | <span data-ttu-id="aecef-117">種類</span><span class="sxs-lookup"><span data-stu-id="aecef-117">Type</span></span>   |<span data-ttu-id="aecef-118">説明</span><span class="sxs-lookup"><span data-stu-id="aecef-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aecef-119">bold</span><span class="sxs-lookup"><span data-stu-id="aecef-119">bold</span></span>|<span data-ttu-id="aecef-120">ブール値</span><span class="sxs-lookup"><span data-stu-id="aecef-120">boolean</span></span>|<span data-ttu-id="aecef-121">フォントの太字の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="aecef-121">Represents the bold status of font.</span></span>|
|<span data-ttu-id="aecef-122">color</span><span class="sxs-lookup"><span data-stu-id="aecef-122">color</span></span>|<span data-ttu-id="aecef-123">文字列</span><span class="sxs-lookup"><span data-stu-id="aecef-123">string</span></span>|<span data-ttu-id="aecef-p101">テキストの色の HTML カラー コード表記。たとえば、#FF0000 は赤を表します。</span><span class="sxs-lookup"><span data-stu-id="aecef-p101">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="aecef-127">italic</span><span class="sxs-lookup"><span data-stu-id="aecef-127">italic</span></span>|<span data-ttu-id="aecef-128">ブール値</span><span class="sxs-lookup"><span data-stu-id="aecef-128">boolean</span></span>|<span data-ttu-id="aecef-129">フォントの斜体の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="aecef-129">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="aecef-130">name</span><span class="sxs-lookup"><span data-stu-id="aecef-130">name</span></span>|<span data-ttu-id="aecef-131">文字列</span><span class="sxs-lookup"><span data-stu-id="aecef-131">string</span></span>|<span data-ttu-id="aecef-132">フォント名 (例: "Calibri")</span><span class="sxs-lookup"><span data-stu-id="aecef-132">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="aecef-133">size</span><span class="sxs-lookup"><span data-stu-id="aecef-133">size</span></span>|<span data-ttu-id="aecef-134">double</span><span class="sxs-lookup"><span data-stu-id="aecef-134">double</span></span>|<span data-ttu-id="aecef-135">フォント サイズ</span><span class="sxs-lookup"><span data-stu-id="aecef-135">Font size.</span></span>|
|<span data-ttu-id="aecef-136">underline</span><span class="sxs-lookup"><span data-stu-id="aecef-136">underline</span></span>|<span data-ttu-id="aecef-137">文字列</span><span class="sxs-lookup"><span data-stu-id="aecef-137">string</span></span>|<span data-ttu-id="aecef-138">フォントに適用する下線の種類です。</span><span class="sxs-lookup"><span data-stu-id="aecef-138">Type of underline applied to the font.</span></span> <span data-ttu-id="aecef-139">可能な値: `None`、 `Single`、 `Double`、 `SingleAccountant`、 `DoubleAccountant`。</span><span class="sxs-lookup"><span data-stu-id="aecef-139">The possible values are: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aecef-140">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="aecef-140">Relationships</span></span>
<span data-ttu-id="aecef-141">なし</span><span class="sxs-lookup"><span data-stu-id="aecef-141">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="aecef-142">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="aecef-142">JSON representation</span></span>

<span data-ttu-id="aecef-143">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="aecef-143">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
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
<!-- {
  "type": "#page.annotation",
  "description": "RangeFont resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
