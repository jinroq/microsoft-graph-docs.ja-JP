---
title: RangeFill リソースの種類
description: 範囲オブジェクトの背景を表します。
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: d1dc1bda19d725999f9a49644bee1e4cb1126ec2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27877190"
---
# <a name="rangefill-resource-type"></a><span data-ttu-id="cfca3-103">RangeFill リソースの種類</span><span class="sxs-lookup"><span data-stu-id="cfca3-103">RangeFill resource type</span></span>

<span data-ttu-id="cfca3-104">範囲オブジェクトの背景を表します。</span><span class="sxs-lookup"><span data-stu-id="cfca3-104">Represents the background of a range object.</span></span>


## <a name="methods"></a><span data-ttu-id="cfca3-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="cfca3-105">Methods</span></span>

| <span data-ttu-id="cfca3-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="cfca3-106">Method</span></span>           | <span data-ttu-id="cfca3-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="cfca3-107">Return Type</span></span>    |<span data-ttu-id="cfca3-108">説明</span><span class="sxs-lookup"><span data-stu-id="cfca3-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="cfca3-109">RangeFill を取得する</span><span class="sxs-lookup"><span data-stu-id="cfca3-109">Get RangeFill</span></span>](../api/rangefill-get.md) | [<span data-ttu-id="cfca3-110">WorkbookRangeFill</span><span class="sxs-lookup"><span data-stu-id="cfca3-110">WorkbookRangeFill</span></span>](rangefill.md) |<span data-ttu-id="cfca3-111">rangeFill オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="cfca3-111">Read properties and relationships of rangeFill object.</span></span>|
|[<span data-ttu-id="cfca3-112">Update</span><span class="sxs-lookup"><span data-stu-id="cfca3-112">Update</span></span>](../api/rangefill-update.md) | [<span data-ttu-id="cfca3-113">WorkbookRangeFill</span><span class="sxs-lookup"><span data-stu-id="cfca3-113">WorkbookRangeFill</span></span>](rangefill.md)   |<span data-ttu-id="cfca3-114">RangeFill オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="cfca3-114">Update RangeFill object.</span></span> |
|[<span data-ttu-id="cfca3-115">Clear</span><span class="sxs-lookup"><span data-stu-id="cfca3-115">Clear</span></span>](../api/rangefill-clear.md)|<span data-ttu-id="cfca3-116">なし</span><span class="sxs-lookup"><span data-stu-id="cfca3-116">None</span></span>|<span data-ttu-id="cfca3-117">範囲の背景をリセットします。</span><span class="sxs-lookup"><span data-stu-id="cfca3-117">Resets the range background.</span></span>|

## <a name="properties"></a><span data-ttu-id="cfca3-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cfca3-118">Properties</span></span>
| <span data-ttu-id="cfca3-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cfca3-119">Property</span></span>     | <span data-ttu-id="cfca3-120">種類</span><span class="sxs-lookup"><span data-stu-id="cfca3-120">Type</span></span>   |<span data-ttu-id="cfca3-121">説明</span><span class="sxs-lookup"><span data-stu-id="cfca3-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cfca3-122">color</span><span class="sxs-lookup"><span data-stu-id="cfca3-122">color</span></span>|<span data-ttu-id="cfca3-123">文字列</span><span class="sxs-lookup"><span data-stu-id="cfca3-123">string</span></span>|<span data-ttu-id="cfca3-124">枠線の色を表す HTML カラー コード。形式は #RRGGBB (例: "FFA500")、または名前付きの HTML 色 (例: "オレンジ")</span><span class="sxs-lookup"><span data-stu-id="cfca3-124">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange")</span></span>|

## <a name="relationships"></a><span data-ttu-id="cfca3-125">関係</span><span class="sxs-lookup"><span data-stu-id="cfca3-125">Relationships</span></span>
<span data-ttu-id="cfca3-126">なし</span><span class="sxs-lookup"><span data-stu-id="cfca3-126">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="cfca3-127">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cfca3-127">JSON representation</span></span>

<span data-ttu-id="cfca3-128">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="cfca3-128">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookRangeFill"
}-->

```json
{
  "color": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeFill resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
