---
title: RangeFill リソースの種類
description: Range オブジェクトの背景を表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 75aa4bd91ad6f1038fdc42460c6a3c9ab928a09d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32579474"
---
# <a name="rangefill-resource-type"></a><span data-ttu-id="84b67-103">RangeFill リソースの種類</span><span class="sxs-lookup"><span data-stu-id="84b67-103">RangeFill resource type</span></span>

<span data-ttu-id="84b67-104">Range オブジェクトの背景を表します。</span><span class="sxs-lookup"><span data-stu-id="84b67-104">Represents the background of a range object.</span></span>


## <a name="methods"></a><span data-ttu-id="84b67-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="84b67-105">Methods</span></span>

| <span data-ttu-id="84b67-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="84b67-106">Method</span></span>           | <span data-ttu-id="84b67-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="84b67-107">Return Type</span></span>    |<span data-ttu-id="84b67-108">説明</span><span class="sxs-lookup"><span data-stu-id="84b67-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="84b67-109">RangeFill を取得する</span><span class="sxs-lookup"><span data-stu-id="84b67-109">Get RangeFill</span></span>](../api/rangefill-get.md) | [<span data-ttu-id="84b67-110">WorkbookRangeFill</span><span class="sxs-lookup"><span data-stu-id="84b67-110">WorkbookRangeFill</span></span>](rangefill.md) |<span data-ttu-id="84b67-111">rangeFill オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="84b67-111">Read properties and relationships of rangeFill object.</span></span>|
|[<span data-ttu-id="84b67-112">Update</span><span class="sxs-lookup"><span data-stu-id="84b67-112">Update</span></span>](../api/rangefill-update.md) | [<span data-ttu-id="84b67-113">WorkbookRangeFill</span><span class="sxs-lookup"><span data-stu-id="84b67-113">WorkbookRangeFill</span></span>](rangefill.md)   |<span data-ttu-id="84b67-114">RangeFill オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="84b67-114">Update RangeFill object.</span></span> |
|[<span data-ttu-id="84b67-115">Clear</span><span class="sxs-lookup"><span data-stu-id="84b67-115">Clear</span></span>](../api/rangefill-clear.md)|<span data-ttu-id="84b67-116">なし</span><span class="sxs-lookup"><span data-stu-id="84b67-116">None</span></span>|<span data-ttu-id="84b67-117">範囲の背景をリセットします。</span><span class="sxs-lookup"><span data-stu-id="84b67-117">Resets the range background.</span></span>|

## <a name="properties"></a><span data-ttu-id="84b67-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="84b67-118">Properties</span></span>
| <span data-ttu-id="84b67-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="84b67-119">Property</span></span>     | <span data-ttu-id="84b67-120">型</span><span class="sxs-lookup"><span data-stu-id="84b67-120">Type</span></span>   |<span data-ttu-id="84b67-121">説明</span><span class="sxs-lookup"><span data-stu-id="84b67-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="84b67-122">color</span><span class="sxs-lookup"><span data-stu-id="84b67-122">color</span></span>|<span data-ttu-id="84b67-123">string</span><span class="sxs-lookup"><span data-stu-id="84b67-123">string</span></span>|<span data-ttu-id="84b67-124">枠線の色を表す HTML カラー コード。形式は #RRGGBB (例: "FFA500")、または名前付きの HTML 色 (例: "オレンジ")</span><span class="sxs-lookup"><span data-stu-id="84b67-124">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange")</span></span>|

## <a name="relationships"></a><span data-ttu-id="84b67-125">関係</span><span class="sxs-lookup"><span data-stu-id="84b67-125">Relationships</span></span>
<span data-ttu-id="84b67-126">なし</span><span class="sxs-lookup"><span data-stu-id="84b67-126">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="84b67-127">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="84b67-127">JSON representation</span></span>

<span data-ttu-id="84b67-128">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="84b67-128">Here is a JSON representation of the resource.</span></span>

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
