---
title: workbookRangeFill リソースの種類
description: Range オブジェクトの背景を表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: cb61352964323b0ded8733aa52ddd19854e028d2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007096"
---
# <a name="workbookrangefill-resource-type"></a><span data-ttu-id="548a9-103">workbookRangeFill リソースの種類</span><span class="sxs-lookup"><span data-stu-id="548a9-103">workbookRangeFill resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="548a9-104">Range オブジェクトの背景を表します。</span><span class="sxs-lookup"><span data-stu-id="548a9-104">Represents the background of a range object.</span></span>


## <a name="methods"></a><span data-ttu-id="548a9-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="548a9-105">Methods</span></span>

| <span data-ttu-id="548a9-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="548a9-106">Method</span></span>           | <span data-ttu-id="548a9-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="548a9-107">Return Type</span></span>    |<span data-ttu-id="548a9-108">説明</span><span class="sxs-lookup"><span data-stu-id="548a9-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="548a9-109">WorkbookRangeFill を取得する</span><span class="sxs-lookup"><span data-stu-id="548a9-109">Get workbookRangeFill</span></span>](../api/rangefill-get.md) | [<span data-ttu-id="548a9-110">workbookRangeFill</span><span class="sxs-lookup"><span data-stu-id="548a9-110">workbookRangeFill</span></span>](workbookrangefill.md) |<span data-ttu-id="548a9-111">rangeFill オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="548a9-111">Read properties and relationships of rangeFill object.</span></span>|
|[<span data-ttu-id="548a9-112">Update</span><span class="sxs-lookup"><span data-stu-id="548a9-112">Update</span></span>](../api/rangefill-update.md) | [<span data-ttu-id="548a9-113">workbookRangeFill</span><span class="sxs-lookup"><span data-stu-id="548a9-113">workbookRangeFill</span></span>](workbookrangefill.md)   |<span data-ttu-id="548a9-114">RangeFill オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="548a9-114">Update RangeFill object.</span></span> |
|[<span data-ttu-id="548a9-115">Clear</span><span class="sxs-lookup"><span data-stu-id="548a9-115">Clear</span></span>](../api/rangefill-clear.md)|<span data-ttu-id="548a9-116">なし</span><span class="sxs-lookup"><span data-stu-id="548a9-116">None</span></span>|<span data-ttu-id="548a9-117">範囲の背景をリセットします。</span><span class="sxs-lookup"><span data-stu-id="548a9-117">Resets the range background.</span></span>|

## <a name="properties"></a><span data-ttu-id="548a9-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="548a9-118">Properties</span></span>
| <span data-ttu-id="548a9-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="548a9-119">Property</span></span>     | <span data-ttu-id="548a9-120">型</span><span class="sxs-lookup"><span data-stu-id="548a9-120">Type</span></span>   |<span data-ttu-id="548a9-121">説明</span><span class="sxs-lookup"><span data-stu-id="548a9-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="548a9-122">color</span><span class="sxs-lookup"><span data-stu-id="548a9-122">color</span></span>|<span data-ttu-id="548a9-123">string</span><span class="sxs-lookup"><span data-stu-id="548a9-123">string</span></span>|<span data-ttu-id="548a9-124">枠線の色を表す HTML カラー コード。形式は #RRGGBB (例: "FFA500")、または名前付きの HTML 色 (例: "オレンジ")</span><span class="sxs-lookup"><span data-stu-id="548a9-124">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange")</span></span>|

## <a name="relationships"></a><span data-ttu-id="548a9-125">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="548a9-125">Relationships</span></span>
<span data-ttu-id="548a9-126">なし</span><span class="sxs-lookup"><span data-stu-id="548a9-126">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="548a9-127">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="548a9-127">JSON representation</span></span>

<span data-ttu-id="548a9-128">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="548a9-128">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookRangeFill"
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
  "suppressions": []
}
-->
