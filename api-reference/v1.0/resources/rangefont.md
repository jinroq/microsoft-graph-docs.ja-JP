---
title: RangeFont リソースの種類
description: このオブジェクトは、オブジェクトのフォントの属性 (フォント名、フォント サイズ、色など) を表します。
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: fe49cc3209164778bbeed625b3c24c7cc8ee3238
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034903"
---
# <a name="rangefont-resource-type"></a><span data-ttu-id="ed16c-103">RangeFont リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ed16c-103">RangeFont resource type</span></span>

<span data-ttu-id="ed16c-104">このオブジェクトは、オブジェクトのフォントの属性 (フォント名、フォント サイズ、色など) を表します。</span><span class="sxs-lookup"><span data-stu-id="ed16c-104">This object represents the font attributes (font name, font size, color, etc.) for an object.</span></span>


## <a name="methods"></a><span data-ttu-id="ed16c-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="ed16c-105">Methods</span></span>

| <span data-ttu-id="ed16c-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="ed16c-106">Method</span></span>           | <span data-ttu-id="ed16c-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ed16c-107">Return Type</span></span>    |<span data-ttu-id="ed16c-108">説明</span><span class="sxs-lookup"><span data-stu-id="ed16c-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ed16c-109">RangeFont を取得する</span><span class="sxs-lookup"><span data-stu-id="ed16c-109">Get RangeFont</span></span>](../api/rangefont-get.md) | [<span data-ttu-id="ed16c-110">WorkbookRangeFont</span><span class="sxs-lookup"><span data-stu-id="ed16c-110">WorkbookRangeFont</span></span>](rangefont.md) |<span data-ttu-id="ed16c-111">rangeFont オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="ed16c-111">Read properties and relationships of rangeFont object.</span></span>|
|[<span data-ttu-id="ed16c-112">Update</span><span class="sxs-lookup"><span data-stu-id="ed16c-112">Update</span></span>](../api/rangefont-update.md) | [<span data-ttu-id="ed16c-113">WorkbookRangeFont</span><span class="sxs-lookup"><span data-stu-id="ed16c-113">WorkbookRangeFont</span></span>](rangefont.md)   |<span data-ttu-id="ed16c-114">RangeFont オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="ed16c-114">Update RangeFont object.</span></span> |

## <a name="properties"></a><span data-ttu-id="ed16c-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ed16c-115">Properties</span></span>
| <span data-ttu-id="ed16c-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ed16c-116">Property</span></span>     | <span data-ttu-id="ed16c-117">型</span><span class="sxs-lookup"><span data-stu-id="ed16c-117">Type</span></span>   |<span data-ttu-id="ed16c-118">説明</span><span class="sxs-lookup"><span data-stu-id="ed16c-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ed16c-119">bold</span><span class="sxs-lookup"><span data-stu-id="ed16c-119">bold</span></span>|<span data-ttu-id="ed16c-120">ブール値</span><span class="sxs-lookup"><span data-stu-id="ed16c-120">boolean</span></span>|<span data-ttu-id="ed16c-121">フォントの太字の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="ed16c-121">Represents the bold status of font.</span></span>|
|<span data-ttu-id="ed16c-122">color</span><span class="sxs-lookup"><span data-stu-id="ed16c-122">color</span></span>|<span data-ttu-id="ed16c-123">string</span><span class="sxs-lookup"><span data-stu-id="ed16c-123">string</span></span>|<span data-ttu-id="ed16c-p101">テキストの色の HTML カラー コード表記。たとえば、#FF0000 は赤を表します。</span><span class="sxs-lookup"><span data-stu-id="ed16c-p101">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="ed16c-127">italic</span><span class="sxs-lookup"><span data-stu-id="ed16c-127">italic</span></span>|<span data-ttu-id="ed16c-128">ブール値</span><span class="sxs-lookup"><span data-stu-id="ed16c-128">boolean</span></span>|<span data-ttu-id="ed16c-129">フォントの斜体の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="ed16c-129">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="ed16c-130">name</span><span class="sxs-lookup"><span data-stu-id="ed16c-130">name</span></span>|<span data-ttu-id="ed16c-131">string</span><span class="sxs-lookup"><span data-stu-id="ed16c-131">string</span></span>|<span data-ttu-id="ed16c-132">フォント名 (例: "Calibri")</span><span class="sxs-lookup"><span data-stu-id="ed16c-132">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="ed16c-133">size</span><span class="sxs-lookup"><span data-stu-id="ed16c-133">size</span></span>|<span data-ttu-id="ed16c-134">double</span><span class="sxs-lookup"><span data-stu-id="ed16c-134">double</span></span>|<span data-ttu-id="ed16c-135">フォント サイズ</span><span class="sxs-lookup"><span data-stu-id="ed16c-135">Font size.</span></span>|
|<span data-ttu-id="ed16c-136">underline</span><span class="sxs-lookup"><span data-stu-id="ed16c-136">underline</span></span>|<span data-ttu-id="ed16c-137">文字列</span><span class="sxs-lookup"><span data-stu-id="ed16c-137">string</span></span>|<span data-ttu-id="ed16c-138">フォントに適用する下線の種類。</span><span class="sxs-lookup"><span data-stu-id="ed16c-138">Type of underline applied to the font.</span></span> <span data-ttu-id="ed16c-139">使用可能な値: `None`、`Single`、`Double`、`SingleAccountant`、`DoubleAccountant`。</span><span class="sxs-lookup"><span data-stu-id="ed16c-139">The possible values are: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ed16c-140">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ed16c-140">Relationships</span></span>
<span data-ttu-id="ed16c-141">なし</span><span class="sxs-lookup"><span data-stu-id="ed16c-141">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="ed16c-142">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ed16c-142">JSON representation</span></span>

<span data-ttu-id="ed16c-143">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ed16c-143">Here is a JSON representation of the resource.</span></span>

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
