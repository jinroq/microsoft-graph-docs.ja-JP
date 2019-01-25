---
title: RangeFill リソースの種類
description: 範囲オブジェクトの背景を表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: d1ae60c0b362ba8593f374c5edd505121cd18587
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509673"
---
# <a name="rangefill-resource-type"></a><span data-ttu-id="d3c69-103">RangeFill リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d3c69-103">RangeFill resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d3c69-104">範囲オブジェクトの背景を表します。</span><span class="sxs-lookup"><span data-stu-id="d3c69-104">Represents the background of a range object.</span></span>


## <a name="methods"></a><span data-ttu-id="d3c69-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="d3c69-105">Methods</span></span>

| <span data-ttu-id="d3c69-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="d3c69-106">Method</span></span>           | <span data-ttu-id="d3c69-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="d3c69-107">Return Type</span></span>    |<span data-ttu-id="d3c69-108">説明</span><span class="sxs-lookup"><span data-stu-id="d3c69-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d3c69-109">RangeFill を取得する</span><span class="sxs-lookup"><span data-stu-id="d3c69-109">[Get RangeFill](../api/rangefill-get.md)</span></span> | <span data-ttu-id="d3c69-110">RangeFill</span><span class="sxs-lookup"><span data-stu-id="d3c69-110">[RangeFill](rangefill.md)</span></span> |<span data-ttu-id="d3c69-111">rangeFill オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="d3c69-111">Read properties and relationships of rangeFill object.</span></span>|
|[<span data-ttu-id="d3c69-112">Update</span><span class="sxs-lookup"><span data-stu-id="d3c69-112">Update</span></span>](../api/rangefill-update.md) | <span data-ttu-id="d3c69-113">RangeFill</span><span class="sxs-lookup"><span data-stu-id="d3c69-113">[RangeFill](rangefill.md)</span></span>   |<span data-ttu-id="d3c69-114">RangeFill オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="d3c69-114">Update RangeFill object.</span></span> |
|[<span data-ttu-id="d3c69-115">Clear</span><span class="sxs-lookup"><span data-stu-id="d3c69-115">Clear</span></span>](../api/rangefill-clear.md)|<span data-ttu-id="d3c69-116">なし</span><span class="sxs-lookup"><span data-stu-id="d3c69-116">None</span></span>|<span data-ttu-id="d3c69-117">範囲の背景をリセットします。</span><span class="sxs-lookup"><span data-stu-id="d3c69-117">Resets the range background.</span></span>|

## <a name="properties"></a><span data-ttu-id="d3c69-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d3c69-118">Properties</span></span>
| <span data-ttu-id="d3c69-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d3c69-119">Property</span></span>     | <span data-ttu-id="d3c69-120">型</span><span class="sxs-lookup"><span data-stu-id="d3c69-120">Type</span></span>   |<span data-ttu-id="d3c69-121">説明</span><span class="sxs-lookup"><span data-stu-id="d3c69-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d3c69-122">color</span><span class="sxs-lookup"><span data-stu-id="d3c69-122">color</span></span>|<span data-ttu-id="d3c69-123">文字列</span><span class="sxs-lookup"><span data-stu-id="d3c69-123">string</span></span>|<span data-ttu-id="d3c69-124">枠線の色を表す HTML カラー コード。形式は #RRGGBB (例: "FFA500")、または名前付きの HTML 色 (例: "オレンジ")</span><span class="sxs-lookup"><span data-stu-id="d3c69-124">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange")</span></span>|

## <a name="relationships"></a><span data-ttu-id="d3c69-125">関係</span><span class="sxs-lookup"><span data-stu-id="d3c69-125">Relationships</span></span>
<span data-ttu-id="d3c69-126">None</span><span class="sxs-lookup"><span data-stu-id="d3c69-126">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="d3c69-127">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d3c69-127">JSON representation</span></span>

<span data-ttu-id="d3c69-128">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d3c69-128">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.rangeFill"
}-->

```json
{
  "color": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "RangeFill resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/rangefill.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
