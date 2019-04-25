---
title: RangeBorder リソースの種類
description: オブジェクトの輪郭を表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 9c32264311400951152f892e6f88d70645f47064
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32579488"
---
# <a name="rangeborder-resource-type"></a><span data-ttu-id="58c36-103">RangeBorder リソースの種類</span><span class="sxs-lookup"><span data-stu-id="58c36-103">RangeBorder resource type</span></span>

<span data-ttu-id="58c36-104">オブジェクトの輪郭を表します。</span><span class="sxs-lookup"><span data-stu-id="58c36-104">Represents the border of an object.</span></span>


## <a name="methods"></a><span data-ttu-id="58c36-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="58c36-105">Methods</span></span>

| <span data-ttu-id="58c36-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="58c36-106">Method</span></span>           | <span data-ttu-id="58c36-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="58c36-107">Return Type</span></span>    |<span data-ttu-id="58c36-108">説明</span><span class="sxs-lookup"><span data-stu-id="58c36-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="58c36-109">RangeBorder を取得する</span><span class="sxs-lookup"><span data-stu-id="58c36-109">Get RangeBorder</span></span>](../api/rangeborder-get.md) | [<span data-ttu-id="58c36-110">WorkbookRangeBorder</span><span class="sxs-lookup"><span data-stu-id="58c36-110">WorkbookRangeBorder</span></span>](rangeborder.md) |<span data-ttu-id="58c36-111">rangeBorder オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="58c36-111">Read properties and relationships of rangeBorder object.</span></span>|
|[<span data-ttu-id="58c36-112">Update</span><span class="sxs-lookup"><span data-stu-id="58c36-112">Update</span></span>](../api/rangeborder-update.md) | [<span data-ttu-id="58c36-113">WorkbookRangeBorder</span><span class="sxs-lookup"><span data-stu-id="58c36-113">WorkbookRangeBorder</span></span>](rangeborder.md) |<span data-ttu-id="58c36-114">RangeBorder オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="58c36-114">Update RangeBorder object.</span></span> |
|[<span data-ttu-id="58c36-115">List</span><span class="sxs-lookup"><span data-stu-id="58c36-115">List</span></span>](../api/rangeborder-list.md) | <span data-ttu-id="58c36-116">[WorkbookRangeBorder](rangeborder.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="58c36-116">[WorkbookRangeBorder](rangeborder.md) collection</span></span> |<span data-ttu-id="58c36-117">rangeBorder オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="58c36-117">Get rangeBorder object collection.</span></span> |
|[<span data-ttu-id="58c36-118">Itemat</span><span class="sxs-lookup"><span data-stu-id="58c36-118">Itemat</span></span>](../api/rangebordercollection-itemat.md)|[<span data-ttu-id="58c36-119">WorkbookRangeBorder</span><span class="sxs-lookup"><span data-stu-id="58c36-119">WorkbookRangeBorder</span></span>](rangeborder.md)|<span data-ttu-id="58c36-120">インデックスに基づいて border オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="58c36-120">Gets a border object using its index</span></span>|

## <a name="properties"></a><span data-ttu-id="58c36-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="58c36-121">Properties</span></span>
| <span data-ttu-id="58c36-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="58c36-122">Property</span></span>     | <span data-ttu-id="58c36-123">型</span><span class="sxs-lookup"><span data-stu-id="58c36-123">Type</span></span>   |<span data-ttu-id="58c36-124">説明</span><span class="sxs-lookup"><span data-stu-id="58c36-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="58c36-125">color</span><span class="sxs-lookup"><span data-stu-id="58c36-125">color</span></span>|<span data-ttu-id="58c36-126">文字列</span><span class="sxs-lookup"><span data-stu-id="58c36-126">string</span></span>|<span data-ttu-id="58c36-127">枠線の色を表す HTML カラー コード。形式は #RRGGBB (例: "FFA500")、または名前付きの HTML 色 (例: "オレンジ") です。</span><span class="sxs-lookup"><span data-stu-id="58c36-127">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange").</span></span>|
|<span data-ttu-id="58c36-128">id</span><span class="sxs-lookup"><span data-stu-id="58c36-128">id</span></span>|<span data-ttu-id="58c36-129">string</span><span class="sxs-lookup"><span data-stu-id="58c36-129">string</span></span>|<span data-ttu-id="58c36-130">罫線の識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="58c36-130">Represents border identifier.</span></span> <span data-ttu-id="58c36-131">使用可能な値は`EdgeTop`、 `EdgeBottom`、 `EdgeLeft` `EdgeRight` `InsideVertical` `InsideHorizontal` `DiagonalDown`、、、、、 `DiagonalUp`、です。</span><span class="sxs-lookup"><span data-stu-id="58c36-131">The possible values are: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`.</span></span> <span data-ttu-id="58c36-132">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="58c36-132">Read-only.</span></span>|
|<span data-ttu-id="58c36-133">sideindex</span><span class="sxs-lookup"><span data-stu-id="58c36-133">sideIndex</span></span>|<span data-ttu-id="58c36-134">string</span><span class="sxs-lookup"><span data-stu-id="58c36-134">string</span></span>|<span data-ttu-id="58c36-135">罫線の特定の辺を表す定数値。</span><span class="sxs-lookup"><span data-stu-id="58c36-135">Constant value that indicates the specific side of the border.</span></span> <span data-ttu-id="58c36-136">使用可能な値は`EdgeTop`、 `EdgeBottom`、 `EdgeLeft` `EdgeRight` `InsideVertical` `InsideHorizontal` `DiagonalDown`、、、、、 `DiagonalUp`、です。</span><span class="sxs-lookup"><span data-stu-id="58c36-136">The possible values are: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`.</span></span> <span data-ttu-id="58c36-137">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="58c36-137">Read-only.</span></span>|
|<span data-ttu-id="58c36-138">style</span><span class="sxs-lookup"><span data-stu-id="58c36-138">style</span></span>|<span data-ttu-id="58c36-139">string</span><span class="sxs-lookup"><span data-stu-id="58c36-139">string</span></span>|<span data-ttu-id="58c36-140">罫線の線スタイルを指定する、線スタイル定数のいずれか 1 つ。</span><span class="sxs-lookup"><span data-stu-id="58c36-140">One of the constants of line style specifying the line style for the border.</span></span> <span data-ttu-id="58c36-141">使用可能な値は`None`、 `Continuous`、 `Dash` `DashDot` `DashDotDot` `Dot` `Double`、、、、、 `SlantDashDot`、です。</span><span class="sxs-lookup"><span data-stu-id="58c36-141">The possible values are: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`.</span></span>|
|<span data-ttu-id="58c36-142">weight</span><span class="sxs-lookup"><span data-stu-id="58c36-142">weight</span></span>|<span data-ttu-id="58c36-143">string</span><span class="sxs-lookup"><span data-stu-id="58c36-143">string</span></span>|<span data-ttu-id="58c36-144">範囲を取り囲む罫線の太さを指定します。</span><span class="sxs-lookup"><span data-stu-id="58c36-144">Specifies the weight of the border around a range.</span></span> <span data-ttu-id="58c36-145">使用可能な値は`Hairline`、 `Thin`、 `Medium`、 `Thick`、です。</span><span class="sxs-lookup"><span data-stu-id="58c36-145">The possible values are: `Hairline`, `Thin`, `Medium`, `Thick`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="58c36-146">関係</span><span class="sxs-lookup"><span data-stu-id="58c36-146">Relationships</span></span>
<span data-ttu-id="58c36-147">なし</span><span class="sxs-lookup"><span data-stu-id="58c36-147">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="58c36-148">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="58c36-148">JSON representation</span></span>

<span data-ttu-id="58c36-149">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="58c36-149">Here is a JSON representation of the resource.</span></span>

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
