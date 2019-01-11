---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: GeoCoordinates
localization_priority: Normal
ms.openlocfilehash: d49142ed414ad82ec149792e11e5a8c42d9837dc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27852641"
---
# <a name="geocoordinates-resource-type"></a><span data-ttu-id="397c2-102">GeoCoordinates リソースの種類</span><span class="sxs-lookup"><span data-stu-id="397c2-102">GeoCoordinates resource type</span></span>

> <span data-ttu-id="397c2-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="397c2-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="397c2-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="397c2-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="397c2-p102">**GeoCoordinates** リソースは、ファイル内に含まれるメタデータに基づいて場所の地理座標系と高度を提供します。[**DriveItem**](driveitem.md) に null でない**場所**のファセットがある場合は、アイテムは、それに関連付けられている既知の場所を含むファイルを表します。</span><span class="sxs-lookup"><span data-stu-id="397c2-p102">The **GeoCoordinates** resource provides geographic coordinates and elevation of a location based on metadata contained within the file. If a [**DriveItem**](driveitem.md) has a non-null **location** facet, the item represents a file with a known location assocaited with it.</span></span>

## <a name="json-representation"></a><span data-ttu-id="397c2-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="397c2-107">JSON representation</span></span>

<span data-ttu-id="397c2-108">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="397c2-108">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.geoCoordinates"
}-->

```json
{
  "altitude": 1024.13,
  "latitude": 26.13246,
  "longitude": 24.34616
}
```

## <a name="properties"></a><span data-ttu-id="397c2-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="397c2-109">Properties</span></span>

| <span data-ttu-id="397c2-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="397c2-110">Property</span></span>  | <span data-ttu-id="397c2-111">種類</span><span class="sxs-lookup"><span data-stu-id="397c2-111">Type</span></span>   | <span data-ttu-id="397c2-112">説明</span><span class="sxs-lookup"><span data-stu-id="397c2-112">Description</span></span>
|:----------|:-------|:--------------------------------------------------------
| <span data-ttu-id="397c2-113">altitude</span><span class="sxs-lookup"><span data-stu-id="397c2-113">altitude</span></span>  | <span data-ttu-id="397c2-114">倍精度浮動小数点数</span><span class="sxs-lookup"><span data-stu-id="397c2-114">Double</span></span> | <span data-ttu-id="397c2-p103">省略可能。アイテムの海抜をフィート単位で表した高度 (高さ)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="397c2-p103">Optional. The altitude (height), in feet,  above sea level for the item. Read-only.</span></span>
| <span data-ttu-id="397c2-118">latitude</span><span class="sxs-lookup"><span data-stu-id="397c2-118">latitude</span></span>  | <span data-ttu-id="397c2-119">倍精度浮動小数点数</span><span class="sxs-lookup"><span data-stu-id="397c2-119">Double</span></span> | <span data-ttu-id="397c2-p104">省略可能。アイテムの緯度 (10 進数)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="397c2-p104">Optional. The latitude, in decimal, for the item. Read-only.</span></span>
| <span data-ttu-id="397c2-123">longitude</span><span class="sxs-lookup"><span data-stu-id="397c2-123">longitude</span></span> | <span data-ttu-id="397c2-124">倍精度浮動小数点数</span><span class="sxs-lookup"><span data-stu-id="397c2-124">Double</span></span> | <span data-ttu-id="397c2-p105">省略可能。アイテムの経度 (10 進数)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="397c2-p105">Optional. The longitude, in decimal, for the item. Read-only.</span></span>

## <a name="remarks"></a><span data-ttu-id="397c2-128">注釈</span><span class="sxs-lookup"><span data-stu-id="397c2-128">Remarks</span></span>

<span data-ttu-id="397c2-129">DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="397c2-129">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The location facet provides geographic location related properties for an item",
  "keywords": "location,geographic,item,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Location"
} -->
