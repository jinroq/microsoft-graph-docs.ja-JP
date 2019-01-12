---
title: RangeBorder リソースの種類
description: オブジェクトの輪郭を表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 9c32264311400951152f892e6f88d70645f47064
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947611"
---
# <a name="rangeborder-resource-type"></a><span data-ttu-id="ca7d1-103">RangeBorder リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ca7d1-103">RangeBorder resource type</span></span>

<span data-ttu-id="ca7d1-104">オブジェクトの輪郭を表します。</span><span class="sxs-lookup"><span data-stu-id="ca7d1-104">Represents the border of an object.</span></span>


## <a name="methods"></a><span data-ttu-id="ca7d1-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="ca7d1-105">Methods</span></span>

| <span data-ttu-id="ca7d1-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="ca7d1-106">Method</span></span>           | <span data-ttu-id="ca7d1-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ca7d1-107">Return Type</span></span>    |<span data-ttu-id="ca7d1-108">説明</span><span class="sxs-lookup"><span data-stu-id="ca7d1-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ca7d1-109">RangeBorder を取得する</span><span class="sxs-lookup"><span data-stu-id="ca7d1-109">Get RangeBorder</span></span>](../api/rangeborder-get.md) | [<span data-ttu-id="ca7d1-110">WorkbookRangeBorder</span><span class="sxs-lookup"><span data-stu-id="ca7d1-110">WorkbookRangeBorder</span></span>](rangeborder.md) |<span data-ttu-id="ca7d1-111">rangeBorder オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="ca7d1-111">Read properties and relationships of rangeBorder object.</span></span>|
|[<span data-ttu-id="ca7d1-112">Update</span><span class="sxs-lookup"><span data-stu-id="ca7d1-112">Update</span></span>](../api/rangeborder-update.md) | [<span data-ttu-id="ca7d1-113">WorkbookRangeBorder</span><span class="sxs-lookup"><span data-stu-id="ca7d1-113">WorkbookRangeBorder</span></span>](rangeborder.md) |<span data-ttu-id="ca7d1-114">RangeBorder オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="ca7d1-114">Update RangeBorder object.</span></span> |
|[<span data-ttu-id="ca7d1-115">List</span><span class="sxs-lookup"><span data-stu-id="ca7d1-115">List</span></span>](../api/rangeborder-list.md) | <span data-ttu-id="ca7d1-116">[WorkbookRangeBorder](rangeborder.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="ca7d1-116">[WorkbookRangeBorder](rangeborder.md) collection</span></span> |<span data-ttu-id="ca7d1-117">rangeBorder オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="ca7d1-117">Get rangeBorder object collection.</span></span> |
|[<span data-ttu-id="ca7d1-118">Itemat</span><span class="sxs-lookup"><span data-stu-id="ca7d1-118">Itemat</span></span>](../api/rangebordercollection-itemat.md)|[<span data-ttu-id="ca7d1-119">WorkbookRangeBorder</span><span class="sxs-lookup"><span data-stu-id="ca7d1-119">WorkbookRangeBorder</span></span>](rangeborder.md)|<span data-ttu-id="ca7d1-120">オブジェクトのインデックスを使用して、境界線オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="ca7d1-120">Gets a border object using its index</span></span>|

## <a name="properties"></a><span data-ttu-id="ca7d1-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ca7d1-121">Properties</span></span>
| <span data-ttu-id="ca7d1-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ca7d1-122">Property</span></span>     | <span data-ttu-id="ca7d1-123">種類</span><span class="sxs-lookup"><span data-stu-id="ca7d1-123">Type</span></span>   |<span data-ttu-id="ca7d1-124">説明</span><span class="sxs-lookup"><span data-stu-id="ca7d1-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ca7d1-125">color</span><span class="sxs-lookup"><span data-stu-id="ca7d1-125">color</span></span>|<span data-ttu-id="ca7d1-126">文字列</span><span class="sxs-lookup"><span data-stu-id="ca7d1-126">string</span></span>|<span data-ttu-id="ca7d1-127">枠線の色を表す HTML カラー コード。形式は #RRGGBB (例: "FFA500")、または名前付きの HTML 色 (例: "オレンジ") です。</span><span class="sxs-lookup"><span data-stu-id="ca7d1-127">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange").</span></span>|
|<span data-ttu-id="ca7d1-128">ID</span><span class="sxs-lookup"><span data-stu-id="ca7d1-128">id</span></span>|<span data-ttu-id="ca7d1-129">文字列</span><span class="sxs-lookup"><span data-stu-id="ca7d1-129">string</span></span>|<span data-ttu-id="ca7d1-130">枠線の識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="ca7d1-130">Represents border identifier.</span></span> <span data-ttu-id="ca7d1-131">可能な値: `EdgeTop`、 `EdgeBottom`、 `EdgeLeft`、 `EdgeRight`、 `InsideVertical`、 `InsideHorizontal`、 `DiagonalDown`、 `DiagonalUp`。</span><span class="sxs-lookup"><span data-stu-id="ca7d1-131">The possible values are: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`.</span></span> <span data-ttu-id="ca7d1-132">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ca7d1-132">Read-only.</span></span>|
|<span data-ttu-id="ca7d1-133">sideIndex</span><span class="sxs-lookup"><span data-stu-id="ca7d1-133">sideIndex</span></span>|<span data-ttu-id="ca7d1-134">文字列</span><span class="sxs-lookup"><span data-stu-id="ca7d1-134">string</span></span>|<span data-ttu-id="ca7d1-135">罫線の特定の側面を示す定数値です。</span><span class="sxs-lookup"><span data-stu-id="ca7d1-135">Constant value that indicates the specific side of the border.</span></span> <span data-ttu-id="ca7d1-136">可能な値: `EdgeTop`、 `EdgeBottom`、 `EdgeLeft`、 `EdgeRight`、 `InsideVertical`、 `InsideHorizontal`、 `DiagonalDown`、 `DiagonalUp`。</span><span class="sxs-lookup"><span data-stu-id="ca7d1-136">The possible values are: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`.</span></span> <span data-ttu-id="ca7d1-137">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ca7d1-137">Read-only.</span></span>|
|<span data-ttu-id="ca7d1-138">style</span><span class="sxs-lookup"><span data-stu-id="ca7d1-138">style</span></span>|<span data-ttu-id="ca7d1-139">文字列</span><span class="sxs-lookup"><span data-stu-id="ca7d1-139">string</span></span>|<span data-ttu-id="ca7d1-140">境界線の線のスタイルを指定する線のスタイルの定数の 1 つです。</span><span class="sxs-lookup"><span data-stu-id="ca7d1-140">One of the constants of line style specifying the line style for the border.</span></span> <span data-ttu-id="ca7d1-141">可能な値: `None`、 `Continuous`、 `Dash`、 `DashDot`、 `DashDotDot`、 `Dot`、 `Double`、 `SlantDashDot`。</span><span class="sxs-lookup"><span data-stu-id="ca7d1-141">The possible values are: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`.</span></span>|
|<span data-ttu-id="ca7d1-142">weight</span><span class="sxs-lookup"><span data-stu-id="ca7d1-142">weight</span></span>|<span data-ttu-id="ca7d1-143">文字列</span><span class="sxs-lookup"><span data-stu-id="ca7d1-143">string</span></span>|<span data-ttu-id="ca7d1-144">範囲周辺の罫線の太さを指定します。</span><span class="sxs-lookup"><span data-stu-id="ca7d1-144">Specifies the weight of the border around a range.</span></span> <span data-ttu-id="ca7d1-145">可能な値: `Hairline`、 `Thin`、 `Medium`、 `Thick`。</span><span class="sxs-lookup"><span data-stu-id="ca7d1-145">The possible values are: `Hairline`, `Thin`, `Medium`, `Thick`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ca7d1-146">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ca7d1-146">Relationships</span></span>
<span data-ttu-id="ca7d1-147">なし</span><span class="sxs-lookup"><span data-stu-id="ca7d1-147">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="ca7d1-148">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ca7d1-148">JSON representation</span></span>

<span data-ttu-id="ca7d1-149">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ca7d1-149">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookRangeBorder"
}-->

```json
{
  "color": "string",
  "id": "string",
  "sideIndex": "string",
  "style": "string",
  "weight": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeBorder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
