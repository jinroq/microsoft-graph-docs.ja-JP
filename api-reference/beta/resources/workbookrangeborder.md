---
title: workbookRangeBorder リソースの種類
description: オブジェクトの輪郭を表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 6457380b3027df8d99b97219ac2ae43e99e0620a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964038"
---
# <a name="workbookrangeborder-resource-type"></a><span data-ttu-id="18701-103">workbookRangeBorder リソースの種類</span><span class="sxs-lookup"><span data-stu-id="18701-103">workbookRangeBorder resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="18701-104">オブジェクトの輪郭を表します。</span><span class="sxs-lookup"><span data-stu-id="18701-104">Represents the border of an object.</span></span>


## <a name="methods"></a><span data-ttu-id="18701-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="18701-105">Methods</span></span>

| <span data-ttu-id="18701-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="18701-106">Method</span></span>           | <span data-ttu-id="18701-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="18701-107">Return Type</span></span>    |<span data-ttu-id="18701-108">説明</span><span class="sxs-lookup"><span data-stu-id="18701-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="18701-109">WorkbookRangeBorder を取得する</span><span class="sxs-lookup"><span data-stu-id="18701-109">Get workbookRangeBorder</span></span>](../api/rangeborder-get.md) | [<span data-ttu-id="18701-110">workbookRangeBorder</span><span class="sxs-lookup"><span data-stu-id="18701-110">workbookRangeBorder</span></span>](workbookrangeborder.md) |<span data-ttu-id="18701-111">rangeBorder オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="18701-111">Read properties and relationships of rangeBorder object.</span></span>|
|[<span data-ttu-id="18701-112">Update</span><span class="sxs-lookup"><span data-stu-id="18701-112">Update</span></span>](../api/rangeborder-update.md) | [<span data-ttu-id="18701-113">workbookRangeBorder</span><span class="sxs-lookup"><span data-stu-id="18701-113">workbookRangeBorder</span></span>](workbookrangeborder.md) |<span data-ttu-id="18701-114">RangeBorder オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="18701-114">Update RangeBorder object.</span></span> |
|[<span data-ttu-id="18701-115">List</span><span class="sxs-lookup"><span data-stu-id="18701-115">List</span></span>](../api/rangeborder-list.md) | <span data-ttu-id="18701-116">[workbookRangeBorder](workbookrangeborder.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="18701-116">[workbookRangeBorder](workbookrangeborder.md) collection</span></span> |<span data-ttu-id="18701-117">rangeBorder オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="18701-117">Get rangeBorder object collection.</span></span> |
|[<span data-ttu-id="18701-118">Itemat</span><span class="sxs-lookup"><span data-stu-id="18701-118">Itemat</span></span>](../api/rangebordercollection-itemat.md)|[<span data-ttu-id="18701-119">workbookRangeBorder</span><span class="sxs-lookup"><span data-stu-id="18701-119">workbookRangeBorder</span></span>](workbookrangeborder.md)|<span data-ttu-id="18701-120">インデックスに基づいて border オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="18701-120">Gets a border object using its index</span></span>|

## <a name="properties"></a><span data-ttu-id="18701-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="18701-121">Properties</span></span>
| <span data-ttu-id="18701-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="18701-122">Property</span></span>     | <span data-ttu-id="18701-123">型</span><span class="sxs-lookup"><span data-stu-id="18701-123">Type</span></span>   |<span data-ttu-id="18701-124">説明</span><span class="sxs-lookup"><span data-stu-id="18701-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="18701-125">color</span><span class="sxs-lookup"><span data-stu-id="18701-125">color</span></span>|<span data-ttu-id="18701-126">文字列</span><span class="sxs-lookup"><span data-stu-id="18701-126">string</span></span>|<span data-ttu-id="18701-127">枠線の色を表す HTML カラー コード。形式は #RRGGBB (例: "FFA500")、または名前付きの HTML 色 (例: "オレンジ") です。</span><span class="sxs-lookup"><span data-stu-id="18701-127">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange").</span></span>|
|<span data-ttu-id="18701-128">id</span><span class="sxs-lookup"><span data-stu-id="18701-128">id</span></span>|<span data-ttu-id="18701-129">string</span><span class="sxs-lookup"><span data-stu-id="18701-129">string</span></span>|<span data-ttu-id="18701-p101">罫線の識別子を表します。可能な値は、`EdgeTop`、`EdgeBottom`、`EdgeLeft`、`EdgeRight`、`InsideVertical`、`InsideHorizontal`、`DiagonalDown`、`DiagonalUp` です。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="18701-p101">Represents border identifier. Possible values are: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`. Read-only.</span></span>|
|<span data-ttu-id="18701-133">sideIndex</span><span class="sxs-lookup"><span data-stu-id="18701-133">sideIndex</span></span>|<span data-ttu-id="18701-134">string</span><span class="sxs-lookup"><span data-stu-id="18701-134">string</span></span>|<span data-ttu-id="18701-p102">罫線の特定の辺を表す定数値。可能な値は、`EdgeTop`、`EdgeBottom`、`EdgeLeft`、`EdgeRight`、`InsideVertical`、`InsideHorizontal`、`DiagonalDown`、`DiagonalUp` です。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="18701-p102">Constant value that indicates the specific side of the border. Possible values are: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`. Read-only.</span></span>|
|<span data-ttu-id="18701-138">style</span><span class="sxs-lookup"><span data-stu-id="18701-138">style</span></span>|<span data-ttu-id="18701-139">string</span><span class="sxs-lookup"><span data-stu-id="18701-139">string</span></span>|<span data-ttu-id="18701-p103">罫線の線スタイルを指定する、線スタイル定数のいずれか 1 つ。可能な値は、`None`、`Continuous`、`Dash`、`DashDot`、`DashDotDot`、`Dot`、`Double`、`SlantDashDot` です。</span><span class="sxs-lookup"><span data-stu-id="18701-p103">One of the constants of line style specifying the line style for the border. Possible values are: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`.</span></span>|
|<span data-ttu-id="18701-142">weight</span><span class="sxs-lookup"><span data-stu-id="18701-142">weight</span></span>|<span data-ttu-id="18701-143">string</span><span class="sxs-lookup"><span data-stu-id="18701-143">string</span></span>|<span data-ttu-id="18701-p104">範囲を取り囲む罫線の太さを指定します。可能な値は、`Hairline`、`Thin`、`Medium`、`Thick` です。</span><span class="sxs-lookup"><span data-stu-id="18701-p104">Specifies the weight of the border around a range. Possible values are: `Hairline`, `Thin`, `Medium`, `Thick`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="18701-146">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="18701-146">Relationships</span></span>
<span data-ttu-id="18701-147">なし</span><span class="sxs-lookup"><span data-stu-id="18701-147">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="18701-148">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="18701-148">JSON representation</span></span>

<span data-ttu-id="18701-149">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="18701-149">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
<!--
{
  "type": "#page.annotation",
  "description": "RangeBorder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
