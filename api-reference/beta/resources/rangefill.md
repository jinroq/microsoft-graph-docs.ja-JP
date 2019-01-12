---
title: RangeFill リソースの種類
description: 範囲オブジェクトの背景を表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 4043122f4c35c3e7f1c6f9d3919687833d35b9b3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27974344"
---
# <a name="rangefill-resource-type"></a><span data-ttu-id="f95fd-103">RangeFill リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f95fd-103">RangeFill resource type</span></span>

> <span data-ttu-id="f95fd-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f95fd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f95fd-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f95fd-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f95fd-106">範囲オブジェクトの背景を表します。</span><span class="sxs-lookup"><span data-stu-id="f95fd-106">Represents the background of a range object.</span></span>


## <a name="methods"></a><span data-ttu-id="f95fd-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="f95fd-107">Methods</span></span>

| <span data-ttu-id="f95fd-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="f95fd-108">Method</span></span>           | <span data-ttu-id="f95fd-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="f95fd-109">Return Type</span></span>    |<span data-ttu-id="f95fd-110">説明</span><span class="sxs-lookup"><span data-stu-id="f95fd-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f95fd-111">RangeFill を取得する</span><span class="sxs-lookup"><span data-stu-id="f95fd-111">Get RangeFill</span></span>](../api/rangefill-get.md) | [<span data-ttu-id="f95fd-112">RangeFill</span><span class="sxs-lookup"><span data-stu-id="f95fd-112">RangeFill</span></span>](rangefill.md) |<span data-ttu-id="f95fd-113">rangeFill オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="f95fd-113">Read properties and relationships of rangeFill object.</span></span>|
|[<span data-ttu-id="f95fd-114">Update</span><span class="sxs-lookup"><span data-stu-id="f95fd-114">Update</span></span>](../api/rangefill-update.md) | [<span data-ttu-id="f95fd-115">RangeFill</span><span class="sxs-lookup"><span data-stu-id="f95fd-115">RangeFill</span></span>](rangefill.md)   |<span data-ttu-id="f95fd-116">RangeFill オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="f95fd-116">Update RangeFill object.</span></span> |
|[<span data-ttu-id="f95fd-117">Clear</span><span class="sxs-lookup"><span data-stu-id="f95fd-117">Clear</span></span>](../api/rangefill-clear.md)|<span data-ttu-id="f95fd-118">なし</span><span class="sxs-lookup"><span data-stu-id="f95fd-118">None</span></span>|<span data-ttu-id="f95fd-119">範囲の背景をリセットします。</span><span class="sxs-lookup"><span data-stu-id="f95fd-119">Resets the range background.</span></span>|

## <a name="properties"></a><span data-ttu-id="f95fd-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f95fd-120">Properties</span></span>
| <span data-ttu-id="f95fd-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f95fd-121">Property</span></span>     | <span data-ttu-id="f95fd-122">種類</span><span class="sxs-lookup"><span data-stu-id="f95fd-122">Type</span></span>   |<span data-ttu-id="f95fd-123">説明</span><span class="sxs-lookup"><span data-stu-id="f95fd-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f95fd-124">color</span><span class="sxs-lookup"><span data-stu-id="f95fd-124">color</span></span>|<span data-ttu-id="f95fd-125">文字列</span><span class="sxs-lookup"><span data-stu-id="f95fd-125">string</span></span>|<span data-ttu-id="f95fd-126">枠線の色を表す HTML カラー コード。形式は #RRGGBB (例: "FFA500")、または名前付きの HTML 色 (例: "オレンジ")</span><span class="sxs-lookup"><span data-stu-id="f95fd-126">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange")</span></span>|

## <a name="relationships"></a><span data-ttu-id="f95fd-127">関係</span><span class="sxs-lookup"><span data-stu-id="f95fd-127">Relationships</span></span>
<span data-ttu-id="f95fd-128">なし</span><span class="sxs-lookup"><span data-stu-id="f95fd-128">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="f95fd-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f95fd-129">JSON representation</span></span>

<span data-ttu-id="f95fd-130">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f95fd-130">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "RangeFill resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
