---
title: RangeFill リソースの種類
description: Range オブジェクトの背景を表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: b884312f8c3a9e8e02242023556713be62f8529f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034910"
---
# <a name="rangefill-resource-type"></a><span data-ttu-id="3b701-103">RangeFill リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3b701-103">RangeFill resource type</span></span>

<span data-ttu-id="3b701-104">Range オブジェクトの背景を表します。</span><span class="sxs-lookup"><span data-stu-id="3b701-104">Represents the background of a range object.</span></span>


## <a name="methods"></a><span data-ttu-id="3b701-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="3b701-105">Methods</span></span>

| <span data-ttu-id="3b701-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="3b701-106">Method</span></span>           | <span data-ttu-id="3b701-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="3b701-107">Return Type</span></span>    |<span data-ttu-id="3b701-108">説明</span><span class="sxs-lookup"><span data-stu-id="3b701-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3b701-109">RangeFill を取得する</span><span class="sxs-lookup"><span data-stu-id="3b701-109">Get RangeFill</span></span>](../api/rangefill-get.md) | [<span data-ttu-id="3b701-110">WorkbookRangeFill</span><span class="sxs-lookup"><span data-stu-id="3b701-110">WorkbookRangeFill</span></span>](rangefill.md) |<span data-ttu-id="3b701-111">rangeFill オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="3b701-111">Read properties and relationships of rangeFill object.</span></span>|
|[<span data-ttu-id="3b701-112">Update</span><span class="sxs-lookup"><span data-stu-id="3b701-112">Update</span></span>](../api/rangefill-update.md) | [<span data-ttu-id="3b701-113">WorkbookRangeFill</span><span class="sxs-lookup"><span data-stu-id="3b701-113">WorkbookRangeFill</span></span>](rangefill.md)   |<span data-ttu-id="3b701-114">RangeFill オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="3b701-114">Update RangeFill object.</span></span> |
|[<span data-ttu-id="3b701-115">Clear</span><span class="sxs-lookup"><span data-stu-id="3b701-115">Clear</span></span>](../api/rangefill-clear.md)|<span data-ttu-id="3b701-116">なし</span><span class="sxs-lookup"><span data-stu-id="3b701-116">None</span></span>|<span data-ttu-id="3b701-117">範囲の背景をリセットします。</span><span class="sxs-lookup"><span data-stu-id="3b701-117">Resets the range background.</span></span>|

## <a name="properties"></a><span data-ttu-id="3b701-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3b701-118">Properties</span></span>
| <span data-ttu-id="3b701-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3b701-119">Property</span></span>     | <span data-ttu-id="3b701-120">型</span><span class="sxs-lookup"><span data-stu-id="3b701-120">Type</span></span>   |<span data-ttu-id="3b701-121">説明</span><span class="sxs-lookup"><span data-stu-id="3b701-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3b701-122">color</span><span class="sxs-lookup"><span data-stu-id="3b701-122">color</span></span>|<span data-ttu-id="3b701-123">string</span><span class="sxs-lookup"><span data-stu-id="3b701-123">string</span></span>|<span data-ttu-id="3b701-124">枠線の色を表す HTML カラー コード。形式は #RRGGBB (例: "FFA500")、または名前付きの HTML 色 (例: "オレンジ")</span><span class="sxs-lookup"><span data-stu-id="3b701-124">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange")</span></span>|

## <a name="relationships"></a><span data-ttu-id="3b701-125">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="3b701-125">Relationships</span></span>
<span data-ttu-id="3b701-126">なし</span><span class="sxs-lookup"><span data-stu-id="3b701-126">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="3b701-127">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3b701-127">JSON representation</span></span>

<span data-ttu-id="3b701-128">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3b701-128">Here is a JSON representation of the resource.</span></span>

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
