---
title: RangeBorder リソースの種類
description: オブジェクトの輪郭を表します。
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 33ed0410ab807cf9d9d6a0a49cb06b43d9966e46
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27853530"
---
# <a name="rangeborder-resource-type"></a><span data-ttu-id="46865-103">RangeBorder リソースの種類</span><span class="sxs-lookup"><span data-stu-id="46865-103">RangeBorder resource type</span></span>

> <span data-ttu-id="46865-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="46865-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="46865-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="46865-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="46865-106">オブジェクトの輪郭を表します。</span><span class="sxs-lookup"><span data-stu-id="46865-106">Represents the border of an object.</span></span>


## <a name="methods"></a><span data-ttu-id="46865-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="46865-107">Methods</span></span>

| <span data-ttu-id="46865-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="46865-108">Method</span></span>           | <span data-ttu-id="46865-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="46865-109">Return Type</span></span>    |<span data-ttu-id="46865-110">説明</span><span class="sxs-lookup"><span data-stu-id="46865-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="46865-111">RangeBorder を取得する</span><span class="sxs-lookup"><span data-stu-id="46865-111">Get RangeBorder</span></span>](../api/rangeborder-get.md) | [<span data-ttu-id="46865-112">RangeBorder</span><span class="sxs-lookup"><span data-stu-id="46865-112">RangeBorder</span></span>](rangeborder.md) |<span data-ttu-id="46865-113">rangeBorder オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="46865-113">Read properties and relationships of rangeBorder object.</span></span>|
|[<span data-ttu-id="46865-114">Update</span><span class="sxs-lookup"><span data-stu-id="46865-114">Update</span></span>](../api/rangeborder-update.md) | [<span data-ttu-id="46865-115">RangeBorder</span><span class="sxs-lookup"><span data-stu-id="46865-115">RangeBorder</span></span>](rangeborder.md) |<span data-ttu-id="46865-116">RangeBorder オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="46865-116">Update RangeBorder object.</span></span> |
|[<span data-ttu-id="46865-117">List</span><span class="sxs-lookup"><span data-stu-id="46865-117">List</span></span>](../api/rangeborder-list.md) | <span data-ttu-id="46865-118">[RangeBorder](rangeborder.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="46865-118">[RangeBorder](rangeborder.md) collection</span></span> |<span data-ttu-id="46865-119">rangeBorder オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="46865-119">Get rangeBorder object collection.</span></span> |
|[<span data-ttu-id="46865-120">Itemat</span><span class="sxs-lookup"><span data-stu-id="46865-120">Itemat</span></span>](../api/rangebordercollection-itemat.md)|[<span data-ttu-id="46865-121">RangeBorder</span><span class="sxs-lookup"><span data-stu-id="46865-121">RangeBorder</span></span>](rangeborder.md)|<span data-ttu-id="46865-122">オブジェクトのインデックスを使用して、境界線オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="46865-122">Gets a border object using its index</span></span>|

## <a name="properties"></a><span data-ttu-id="46865-123">プロパティ</span><span class="sxs-lookup"><span data-stu-id="46865-123">Properties</span></span>
| <span data-ttu-id="46865-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="46865-124">Property</span></span>     | <span data-ttu-id="46865-125">種類</span><span class="sxs-lookup"><span data-stu-id="46865-125">Type</span></span>   |<span data-ttu-id="46865-126">説明</span><span class="sxs-lookup"><span data-stu-id="46865-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="46865-127">color</span><span class="sxs-lookup"><span data-stu-id="46865-127">color</span></span>|<span data-ttu-id="46865-128">文字列</span><span class="sxs-lookup"><span data-stu-id="46865-128">string</span></span>|<span data-ttu-id="46865-129">枠線の色を表す HTML カラー コード。形式は #RRGGBB (例: "FFA500")、または名前付きの HTML 色 (例: "オレンジ") です。</span><span class="sxs-lookup"><span data-stu-id="46865-129">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange").</span></span>|
|<span data-ttu-id="46865-130">ID</span><span class="sxs-lookup"><span data-stu-id="46865-130">id</span></span>|<span data-ttu-id="46865-131">文字列</span><span class="sxs-lookup"><span data-stu-id="46865-131">string</span></span>|<span data-ttu-id="46865-p102">罫線の識別子を表します。可能な値は、`EdgeTop`、`EdgeBottom`、`EdgeLeft`、`EdgeRight`、`InsideVertical`、`InsideHorizontal`、`DiagonalDown`、`DiagonalUp` です。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="46865-p102">Represents border identifier. Possible values are: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`. Read-only.</span></span>|
|<span data-ttu-id="46865-135">sideIndex</span><span class="sxs-lookup"><span data-stu-id="46865-135">sideIndex</span></span>|<span data-ttu-id="46865-136">文字列</span><span class="sxs-lookup"><span data-stu-id="46865-136">string</span></span>|<span data-ttu-id="46865-p103">罫線の特定の辺を表す定数値。可能な値は、`EdgeTop`、`EdgeBottom`、`EdgeLeft`、`EdgeRight`、`InsideVertical`、`InsideHorizontal`、`DiagonalDown`、`DiagonalUp` です。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="46865-p103">Constant value that indicates the specific side of the border. Possible values are: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`. Read-only.</span></span>|
|<span data-ttu-id="46865-140">style</span><span class="sxs-lookup"><span data-stu-id="46865-140">style</span></span>|<span data-ttu-id="46865-141">文字列</span><span class="sxs-lookup"><span data-stu-id="46865-141">string</span></span>|<span data-ttu-id="46865-p104">罫線の線スタイルを指定する、線スタイル定数のいずれか 1 つ。可能な値は、`None`、`Continuous`、`Dash`、`DashDot`、`DashDotDot`、`Dot`、`Double`、`SlantDashDot` です。</span><span class="sxs-lookup"><span data-stu-id="46865-p104">One of the constants of line style specifying the line style for the border. Possible values are: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`.</span></span>|
|<span data-ttu-id="46865-144">weight</span><span class="sxs-lookup"><span data-stu-id="46865-144">weight</span></span>|<span data-ttu-id="46865-145">文字列</span><span class="sxs-lookup"><span data-stu-id="46865-145">string</span></span>|<span data-ttu-id="46865-p105">範囲を取り囲む罫線の太さを指定します。可能な値は、`Hairline`、`Thin`、`Medium`、`Thick` です。</span><span class="sxs-lookup"><span data-stu-id="46865-p105">Specifies the weight of the border around a range. Possible values are: `Hairline`, `Thin`, `Medium`, `Thick`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="46865-148">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="46865-148">Relationships</span></span>
<span data-ttu-id="46865-149">なし</span><span class="sxs-lookup"><span data-stu-id="46865-149">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="46865-150">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="46865-150">JSON representation</span></span>

<span data-ttu-id="46865-151">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="46865-151">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.rangeBorder"
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
